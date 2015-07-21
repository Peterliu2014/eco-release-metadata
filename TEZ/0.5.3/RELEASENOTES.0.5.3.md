
<!---
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
-->
# Apache Tez  0.5.3 Release Notes

These release notes cover new developer and user-facing incompatibilities, features, and major improvements.


---

* [TEZ-1818](https://issues.apache.org/jira/browse/TEZ-1818) | *Major* | **Problem loading tez-api-version-info.properties in case current context classloader in not pointing to Tez jars**

TEZ-1664 (0.5.2) introduced loading of tez-api-version-info.properties which is packaged within the tez-api.jar. Its using the current context classloader to load it:
{code}
Thread.currentThread().getContextClassLoader()
          .getResourceAsStream(versionInfoFile);
{code}

In our environment we load the tez code as a plugin. Our context classloader doesn't have any reference to the Tez code. Thus when instantiating the tez client there is this exception:
{code}
 WARN [2014-12-03 17:30:30.971] (VersionInfo.java:60) - Could not read 'tez-api-version-info.properties', java.io.IOException: Resource not found
java.io.IOException: Resource not found
	at org.apache.tez.common.VersionInfo.<init>(VersionInfo.java:56)
	at org.apache.tez.client.TezApiVersionInfo.<init>(TezApiVersionInfo.java:26)
	at org.apache.tez.client.TezClient.<init>(TezClient.java:137)
	at org.apache.tez.client.TezClient.create(TezClient.java:213)
        ....
{code}

Is there any specific reason the context classloader is used to load the file ?
Since the properties file is usually bundled within the jar would TezApiVersionInfo.class.getResourceAsStream() not be a better fit ?


---

* [TEZ-1808](https://issues.apache.org/jira/browse/TEZ-1808) | *Major* | **Job can fail since name of intermediate files can be too long in specific situation**

I ran Hive 0.14 on Tez 0.5.2 and master with MemToMemMerger disabled - this configuration change is the diff between TEZ-1807 and this JIRA.  Data size is 100GB texts generated by RandomTextWriter.

{code}
create external table randomText100GB(
  text string
) location 'hdfs:///user/ozawa/randomText100GB';

CREATE TABLE wordcount AS
SELECT word, count(1) AS count
FROM (SELECT EXPLODE(SPLIT(LCASE(REGEXP\_REPLACE(text,'[\\p{Punct},\\p{Cntrl}]','')),' '))
AS word FROM randomText100GB) words
GROUP BY word;
{code}

As a result, an exception is thrown:

{quote}
--------------------------------------------------------------------------------
        VERTICES      STATUS  TOTAL  COMPLETED  RUNNING  PENDING  FAILED  KILLED
--------------------------------------------------------------------------------
Map 1 .........       KILLED    115        110        0        5       0       5
Reducer 2             FAILED      3          0        0        3       1       2
--------------------------------------------------------------------------------
VERTICES: 00/02  [========================>>--] 93%   ELAPSED TIME: 110.95 s   
--------------------------------------------------------------------------------
Status: Failed
Vertex failed, vertexName=Reducer 2, vertexId=vertex\_1417036912823\_0073\_1\_01, diagnostics=[Task failed, taskId=task\_1417036912823\_0073\_1\_01\_000000, diagnostics=[TaskAttempt 0 failed, info=[Error: exceptionThrown=org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$ShuffleError: error in shuffle in DiskToDiskMerger [Map\_1]
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$RunShuffleCallable.call(Shuffle.java:338)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$RunShuffleCallable.call(Shuffle.java:319)
        at java.util.concurrent.FutureTask.run(FutureTask.java:262)
        at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
        at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:615)
        at java.lang.Thread.run(Thread.java:745)
Caused by: java.io.FileNotFoundException: /hadoop1/tmp/nm-local-dir/usercache/ozawa/appcache/application\_1417036912823\_0073/attempt\_1417036912823\_0073\_1\_01\_000000\_0\_10026\_spill\_215.out.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged (File name too long)
        at java.io.FileOutputStream.open(Native Method)
        at java.io.FileOutputStream.<init>(FileOutputStream.java:221)
        at org.apache.hadoop.fs.RawLocalFileSystem$LocalFSFileOutputStream.<init>(RawLocalFileSystem.java:211)
        at org.apache.hadoop.fs.RawLocalFileSystem$LocalFSFileOutputStream.<init>(RawLocalFileSystem.java:207)
        at org.apache.hadoop.fs.RawLocalFileSystem.create(RawLocalFileSystem.java:270)
        at org.apache.hadoop.fs.RawLocalFileSystem.create(RawLocalFileSystem.java:257)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:887)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:784)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:773)
        at org.apache.tez.runtime.library.common.sort.impl.IFile$Writer.<init>(IFile.java:129)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.MergeManager$OnDiskMerger.merge(MergeManager.java:702)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.MergeThread.run(MergeThread.java:89)
, errorMessage=Shuffle Runner Failed:org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$ShuffleError: error in shuffle in DiskToDiskMerger [Map\_1]
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$RunShuffleCallable.call(Shuffle.java:338)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.Shuffle$RunShuffleCallable.call(Shuffle.java:319)
        at java.util.concurrent.FutureTask.run(FutureTask.java:262)
        at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
        at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:615)
        at java.lang.Thread.run(Thread.java:745)
Caused by: java.io.FileNotFoundException: /hadoop1/tmp/nm-local-dir/usercache/ozawa/appcache/application\_1417036912823\_0073/attempt\_1417036912823\_0073\_1\_01\_000000\_0\_10026\_spill\_215.out.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged (File name too long)
        at java.io.FileOutputStream.open(Native Method)
        at java.io.FileOutputStream.<init>(FileOutputStream.java:221)
        at org.apache.hadoop.fs.RawLocalFileSystem$LocalFSFileOutputStream.<init>(RawLocalFileSystem.java:211)
        at org.apache.hadoop.fs.RawLocalFileSystem$LocalFSFileOutputStream.<init>(RawLocalFileSystem.java:207)
        at org.apache.hadoop.fs.RawLocalFileSystem.create(RawLocalFileSystem.java:270)
        at org.apache.hadoop.fs.RawLocalFileSystem.create(RawLocalFileSystem.java:257)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:887)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:784)
        at org.apache.hadoop.fs.FileSystem.create(FileSystem.java:773)
        at org.apache.tez.runtime.library.common.sort.impl.IFile$Writer.<init>(IFile.java:129)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.MergeManager$OnDiskMerger.merge(MergeManager.java:702)
        at org.apache.tez.runtime.library.common.shuffle.orderedgrouped.MergeThread.run(MergeThread.java:89)
]], Vertex failed as one or more tasks failed. failedTasks:1, Vertex vertex\_1417036912823\_0073\_1\_01 [Reducer 2] killed/failed due to:null]
Vertex killed, vertexName=Map 1, vertexId=vertex\_1417036912823\_0073\_1\_00, diagnostics=[Vertex received Kill while in RUNNING state., Vertex killed as other vertex failed. failedTasks:0, Vertex vertex\_1417036912823\_0073\_1\_00 [Map 1] killed/failed due to:null]
DAG failed due to vertex failure. failedVertices:1 killedVertices:1
FAILED: Execution Error, return code 2 from org.apache.hadoop.hive.ql.exec.tez.TezTask
{quote}

The log message of this line looks strange:
{quote}
Caused by: java.io.FileNotFoundException: /hadoop1/tmp/nm-local-dir/usercache/ozawa/appcache/application\_1417036912823\_0073/attempt\_1417036912823\_0073\_1\_01\_000000\_0\_10026\_spill\_215.out.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged.merged (File name too long)
{quote}


---

* [TEZ-1780](https://issues.apache.org/jira/browse/TEZ-1780) | *Blocker* | **tez-api is missing jersey dependencies**

tez-api has DAGClientTimelineImpl which has jersey related dependencies but the pom.xml file was not changed.


---

* [TEZ-1770](https://issues.apache.org/jira/browse/TEZ-1770) | *Critical* | **Handle ConnectExceptions correctly when establishing connections to an NM which may be down**

Thanks [~sidharta-s] for reporting this.


---

* [TEZ-1761](https://issues.apache.org/jira/browse/TEZ-1761) | *Major* | **TestRecoveryParser::testGetLastInProgressDAG fails in similar manner to TEZ-1686**

Tests run: 2, Failures: 1, Errors: 0, Skipped: 0, Time elapsed: 0.713 sec <<< FAILURE!
testGetLastInProgressDAG(org.apache.tez.dag.app.TestRecoveryParser)  Time elapsed: 0.053 sec  <<< FAILURE!
java.lang.AssertionError: expected:<0> but was:<100>
	at org.junit.Assert.fail(Assert.java:88)
	at org.junit.Assert.failNotEquals(Assert.java:743)
	at org.junit.Assert.assertEquals(Assert.java:118)
	at org.junit.Assert.assertEquals(Assert.java:555)
	at org.junit.Assert.assertEquals(Assert.java:542)
	at org.apache.tez.dag.app.TestRecoveryParser.testGetLastInProgressDAG(TestRecoveryParser.java:93)


---

* [TEZ-1750](https://issues.apache.org/jira/browse/TEZ-1750) | *Critical* | **Add a DAGScheduler which schedules tasks only when sources have been scheduled**

Splitting out the patch on TEZ-1522 into a separate jira.

There's several scenarios in which we end up scheduling downstream tasks before their sources have been scheduled - and then get into a situation where the sources are starved. Currently, anywhere a ShuffleVertexManager is used can cause such behaviour - since it starts scheduling it's tasks after a certain number of sources are complete, but subsequen non-shuffle VertexManagers will scheduled immediately.
Disabling slow-start is one option to achieve this (or setting slow start on all vertices), but it doesn't work for the situation where dynamic reducer parallelism kicks in - since it has to wait for source tasks to complete.

The intent here is to add a DAGScheduler, which affectively negates the slow start, and in case of dynamic parallelism determination, waits for upstream tasks to be scheduled before scheduling downstream tasks.


---

* [TEZ-1749](https://issues.apache.org/jira/browse/TEZ-1749) | *Major* | **Increase test timeout for TestLocalMode.testMultipleClientsWithSession**

Times out in other platforms (windows).  Verified that it is successful at times and timesout at times due to slower hardware.


---

* [TEZ-1747](https://issues.apache.org/jira/browse/TEZ-1747) | *Major* | **Increase test timeout for TestSecureShuffle**

Fails intermittently on some other platforms (windows).


---

* [TEZ-1746](https://issues.apache.org/jira/browse/TEZ-1746) | *Major* | **Flaky test in TestVertexImpl and TestExceptionPropagation**

*TestVertexImpl*
{code}
Error Message

expected:<FAILED> but was:<INITIALIZING>
Stacktrace

java.lang.AssertionError: expected:<FAILED> but was:<INITIALIZING>
	at org.junit.Assert.fail(Assert.java:88)
	at org.junit.Assert.failNotEquals(Assert.java:743)
	at org.junit.Assert.assertEquals(Assert.java:118)
	at org.junit.Assert.assertEquals(Assert.java:144)
	at org.apache.tez.dag.app.dag.impl.TestVertexImpl.testExceptionFromII\_OnVertexStateUpdated(TestVertexImpl.java:5212)
{code}

*TestExceptionProgagation*
{code}
Error Message

test timed out after 180000 milliseconds
Stacktrace

java.lang.Exception: test timed out after 180000 milliseconds
	at java.lang.Thread.sleep(Native Method)
	at org.apache.tez.dag.api.client.DAGClientImpl.\_waitForCompletionWithStatusUpdates(DAGClientImpl.java:367)
	at org.apache.tez.dag.api.client.DAGClientImpl.waitForCompletion(DAGClientImpl.java:213)
	at org.apache.tez.test.TestExceptionPropagation.testExceptionPropagationSession(TestExceptionPropagation.java:223)
{code}


---

* [TEZ-1742](https://issues.apache.org/jira/browse/TEZ-1742) | *Major* | **Improve response time of internal preemption**

Tez YARN Task Scheduler currently preempts 1 running task at a time when a higher priority task is waiting and there are no available resources. When a large number of higher priority tasks are pending then it can take a long time to preempt the required number of lower priority tasks.


