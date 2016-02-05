
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
# Apache Flink Changelog

## Release 1.0.0 - Unreleased (as of 2016-02-05)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-3292](https://issues.apache.org/jira/browse/FLINK-3292) | Bug in flink-jdbc. Not all JDBC drivers supported |  Minor | other | Subhobrata Dey |  |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-3102](https://issues.apache.org/jira/browse/FLINK-3102) | Allow reading from multiple topics with one FlinkKafkaConsumer |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-3093](https://issues.apache.org/jira/browse/FLINK-3093) | Introduce annotations for interface stability |  Blocker | Build System | Robert Metzger | Robert Metzger |
| [FLINK-3058](https://issues.apache.org/jira/browse/FLINK-3058) | Add Kafka consumer for new 0.9.0.0 Kafka API |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-2996](https://issues.apache.org/jira/browse/FLINK-2996) | Add config entry to define BlobServer port |  Major | JobManager | Stephan Ewen | Robert Metzger |
| [FLINK-2978](https://issues.apache.org/jira/browse/FLINK-2978) | Integrate web submission interface into the new dashboard |  Major | Web Client, Webfrontend | Sachin Goel | Sachin Goel |
| [FLINK-2955](https://issues.apache.org/jira/browse/FLINK-2955) | Add operations introduction in Table API page. |  Minor | Documentation | Chengxiang Li | Chengxiang Li |
| [FLINK-2951](https://issues.apache.org/jira/browse/FLINK-2951) | Add Union operator to Table API. |  Minor | Documentation, Table API | Chengxiang Li | Chengxiang Li |
| [FLINK-2871](https://issues.apache.org/jira/browse/FLINK-2871) | Add OuterJoin strategy with HashTable on outer side |  Minor | Local Runtime, Optimizer | Fabian Hueske | Chengxiang Li |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-3306](https://issues.apache.org/jira/browse/FLINK-3306) | Auto type registration at Kryo is buggy |  Major | Java API | Stephan Ewen | Stephan Ewen |
| [FLINK-3305](https://issues.apache.org/jira/browse/FLINK-3305) | Remove JavaKaffee serializer util |  Blocker | Java API | Stephan Ewen | Stephan Ewen |
| [FLINK-3265](https://issues.apache.org/jira/browse/FLINK-3265) | RabbitMQ Source not threadsafe: ConcurrentModificationException |  Blocker | Streaming Connectors | Robert Metzger | Maximilian Michels |
| [FLINK-3262](https://issues.apache.org/jira/browse/FLINK-3262) | Remove fuzzy versioning from Bower dependencies |  Trivial | Webfrontend | Greg Hogan | Greg Hogan |
| [FLINK-3246](https://issues.apache.org/jira/browse/FLINK-3246) | Consolidate maven project names with \*-parent suffix |  Major | . | Stephan Ewen | Stephan Ewen |
| [FLINK-3244](https://issues.apache.org/jira/browse/FLINK-3244) | Add log messages to savepoint coordinator restore |  Minor | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3235](https://issues.apache.org/jira/browse/FLINK-3235) | Drop Flink-on-Tez code |  Major | Flink on Tez | Ufuk Celebi | Stephan Ewen |
| [FLINK-3233](https://issues.apache.org/jira/browse/FLINK-3233) | PartitionOperator does not support expression keys on atomic types |  Major | DataSet API | Fabian Hueske | Fabian Hueske |
| [FLINK-3232](https://issues.apache.org/jira/browse/FLINK-3232) | Add option to eagerly deploy channels |  Minor | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3219](https://issues.apache.org/jira/browse/FLINK-3219) | Implement DataSet.count using a single operator |  Minor | . | Greg Hogan | Greg Hogan |
| [FLINK-3209](https://issues.apache.org/jira/browse/FLINK-3209) | Remove Unused ProcessingTime, EventTime and AbstractTime |  Blocker | . | Aljoscha Krettek | Aljoscha Krettek |
| [FLINK-3198](https://issues.apache.org/jira/browse/FLINK-3198) | Rename Grouping.getDataSet() method and add JavaDocs |  Major | DataSet API | Fabian Hueske | Kostas |
| [FLINK-3194](https://issues.apache.org/jira/browse/FLINK-3194) | Remove web client |  Major | Webfrontend | Stephan Ewen | Stephan Ewen |
| [FLINK-3181](https://issues.apache.org/jira/browse/FLINK-3181) | The vertex-centric SSSP example and library method send unnecessary messages during the first superstep |  Major | Gelly | Vasia Kalavri | Vasia Kalavri |
| [FLINK-3178](https://issues.apache.org/jira/browse/FLINK-3178) | Make Closing Behavior of Window Operators Configurable |  Blocker | Streaming | Aljoscha Krettek | Aljoscha Krettek |
| [FLINK-3176](https://issues.apache.org/jira/browse/FLINK-3176) | Window Apply Website Example |  Trivial | website | radu |  |
| [FLINK-3161](https://issues.apache.org/jira/browse/FLINK-3161) | Externalize cluster start-up and tear-down when available |  Minor | Start-Stop Scripts | Greg Hogan | Greg Hogan |
| [FLINK-3147](https://issues.apache.org/jira/browse/FLINK-3147) | HadoopOutputFormatBase should expose fields as protected |  Minor | . | Nick Dimiduk |  |
| [FLINK-3135](https://issues.apache.org/jira/browse/FLINK-3135) | Add chainable driver for UNARY\_NO\_OP strategy |  Minor | Local Runtime | Fabian Hueske | ramkrishna.s.vasudevan |
| [FLINK-3131](https://issues.apache.org/jira/browse/FLINK-3131) | Expose checkpoint metrics |  Major | Webfrontend | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3124](https://issues.apache.org/jira/browse/FLINK-3124) | Introduce a TaskInfo object to better represent task name, index, attempt number etc. |  Major | . | Sachin Goel | Sachin Goel |
| [FLINK-3122](https://issues.apache.org/jira/browse/FLINK-3122) | Generalize value type in LabelPropagation |  Major | Gelly | Martin Junghanns | Martin Junghanns |
| [FLINK-3116](https://issues.apache.org/jira/browse/FLINK-3116) | Remove RecordOperator |  Trivial | Core | Chesnay Schepler | jun aoki |
| [FLINK-3084](https://issues.apache.org/jira/browse/FLINK-3084) | File State Backend should not write very small state into files |  Major | Streaming | Stephan Ewen | Stephan Ewen |
| [FLINK-3077](https://issues.apache.org/jira/browse/FLINK-3077) | Add "version" command to CliFrontend for showing the version of the installation |  Major | Command-line client | Robert Metzger | Sachin Goel |
| [FLINK-3074](https://issues.apache.org/jira/browse/FLINK-3074) | Make ApplicationMaster/JobManager akka port configurable |  Major | YARN Client | Robert Metzger | Robert Metzger |
| [FLINK-3073](https://issues.apache.org/jira/browse/FLINK-3073) | Activate streaming mode by default |  Major | TaskManager | Robert Metzger | Aljoscha Krettek |
| [FLINK-3069](https://issues.apache.org/jira/browse/FLINK-3069) | Make state materialization asynchronous |  Major | Streaming | Stephan Ewen | Aljoscha Krettek |
| [FLINK-3063](https://issues.apache.org/jira/browse/FLINK-3063) | [py] Remove combiner |  Major | Python API | Chesnay Schepler | Chesnay Schepler |
| [FLINK-3056](https://issues.apache.org/jira/browse/FLINK-3056) | Show bytes sent/received as MBs/GB and so on in web interface |  Major | Webfrontend | Robert Metzger | Sachin Goel |
| [FLINK-3055](https://issues.apache.org/jira/browse/FLINK-3055) | ExecutionVertex has duplicate method getParallelSubtaskIndex and getSubTaskIndex |  Trivial | Distributed Runtime | Ufuk Celebi | jun aoki |
| [FLINK-3051](https://issues.apache.org/jira/browse/FLINK-3051) | Define a maximum number of concurrent inflight checkpoints |  Major | Streaming | Stephan Ewen | Stephan Ewen |
| [FLINK-3049](https://issues.apache.org/jira/browse/FLINK-3049) | Move "Either" type to package "org.apache.flink.types" |  Major | Core, Java API | Stephan Ewen | Vasia Kalavri |
| [FLINK-3046](https://issues.apache.org/jira/browse/FLINK-3046) | Integrate the Either Java type with the TypeExtractor |  Major | Type Serialization System | Vasia Kalavri | Timo Walther |
| [FLINK-3045](https://issues.apache.org/jira/browse/FLINK-3045) | Properly expose the key of a kafka message |  Critical | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-3040](https://issues.apache.org/jira/browse/FLINK-3040) | Add docs describing how to configure State Backends |  Major | Documentation | Stephan Ewen | Stephan Ewen |
| [FLINK-3028](https://issues.apache.org/jira/browse/FLINK-3028) | Cannot cancel restarting job via web frontend |  Major | Webfrontend | Ufuk Celebi |  |
| [FLINK-3023](https://issues.apache.org/jira/browse/FLINK-3023) | Show Flink version + commit id for -SNAPSHOT versions in web frontend |  Major | Webfrontend | Robert Metzger | Sachin Goel |
| [FLINK-3017](https://issues.apache.org/jira/browse/FLINK-3017) | Broken 'Slots' link on Streaming Programming Guide |  Minor | Documentation | Suneel Marthi | Suneel Marthi |
| [FLINK-2994](https://issues.apache.org/jira/browse/FLINK-2994) | Client sysout logging does not report exceptions |  Major | Command-line client | Stephan Ewen | Stephan Ewen |
| [FLINK-2981](https://issues.apache.org/jira/browse/FLINK-2981) | Update README for building docs |  Minor | Documentation | Martin Junghanns | Martin Junghanns |
| [FLINK-2974](https://issues.apache.org/jira/browse/FLINK-2974) | Add periodic offset commit to Kafka Consumer if checkpointing is disabled |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-2966](https://issues.apache.org/jira/browse/FLINK-2966) | Improve the way job duration is reported on web frontend. |  Minor | Webfrontend | Sachin Goel | Sachin Goel |
| [FLINK-2962](https://issues.apache.org/jira/browse/FLINK-2962) | Cluster startup script refers to unused variable |  Major | Start-Stop Scripts | Ufuk Celebi | Ufuk Celebi |
| [FLINK-2961](https://issues.apache.org/jira/browse/FLINK-2961) | Add support for basic type Date in Table API |  Minor | Table API | Timo Walther | Timo Walther |
| [FLINK-2940](https://issues.apache.org/jira/browse/FLINK-2940) | Deploy multiple Scala versions for Maven artifacts |  Major | Build System | Maximilian Michels | Maximilian Michels |
| [FLINK-2936](https://issues.apache.org/jira/browse/FLINK-2936) | ClassCastException when using EventTimeSourceFunction in non-EventTime program |  Major | Streaming | Fabian Hueske | Aljoscha Krettek |
| [FLINK-2932](https://issues.apache.org/jira/browse/FLINK-2932) | Flink quickstart docs should ask users to download from https, not http |  Minor | Documentation | Frederick F. Kautz IV |  |
| [FLINK-2904](https://issues.apache.org/jira/browse/FLINK-2904) | Web interface truncated task counts |  Minor | Webfrontend | Greg Hogan | Sachin Goel |
| [FLINK-2902](https://issues.apache.org/jira/browse/FLINK-2902) | Web interface sort tasks newest first |  Minor | Webfrontend | Greg Hogan | Sachin Goel |
| [FLINK-2898](https://issues.apache.org/jira/browse/FLINK-2898) | Invert Travis CI build order |  Trivial | Build System | Greg Hogan | Robert Metzger |
| [FLINK-2897](https://issues.apache.org/jira/browse/FLINK-2897) | Use distinct initial indices for OutputEmitter round-robin |  Major | Distributed Runtime | Greg Hogan | Greg Hogan |
| [FLINK-2895](https://issues.apache.org/jira/browse/FLINK-2895) | Duplicate immutable object creation |  Minor | Distributed Runtime | Greg Hogan | Greg Hogan |
| [FLINK-2893](https://issues.apache.org/jira/browse/FLINK-2893) | Rename recovery configuration keys |  Major | . | Ufuk Celebi | Ufuk Celebi |
| [FLINK-2882](https://issues.apache.org/jira/browse/FLINK-2882) | Improve performance of string conversions |  Major | Core | Greg Hogan | Greg Hogan |
| [FLINK-2524](https://issues.apache.org/jira/browse/FLINK-2524) | Add "getTaskNameWithSubtasks()" to RuntimeContext |  Major | Local Runtime | Stephan Ewen | Sachin Goel |
| [FLINK-2488](https://issues.apache.org/jira/browse/FLINK-2488) | Expose attemptNumber in RuntimeContext |  Minor | JobManager, TaskManager | Robert Metzger | Sachin Goel |
| [FLINK-2017](https://issues.apache.org/jira/browse/FLINK-2017) | Add predefined required parameters to ParameterTool |  Major | . | Robert Metzger | Martin Liesenberg |
| [FLINK-1947](https://issues.apache.org/jira/browse/FLINK-1947) | Make Avro and Tachyon test logging less verbose |  Minor | . | Till Rohrmann |  |
| [FLINK-1903](https://issues.apache.org/jira/browse/FLINK-1903) | Joins where one side uses a field more than once don't work |  Minor | . | Aljoscha Krettek | Fabian Hueske |
| [FLINK-1228](https://issues.apache.org/jira/browse/FLINK-1228) | Add REST Interface to JobManager |  Major | . | Arvid Heise |  |
| [FLINK-734](https://issues.apache.org/jira/browse/FLINK-734) | Integrate web job client into JobManager web interface |  Major | . | GitHub Import |  |
| [FLINK-8](https://issues.apache.org/jira/browse/FLINK-8) | [GitHub] Implement automatic sample histogram building for Range Partitioning |  Major | . | GitHub Import | Chengxiang Li |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-3342](https://issues.apache.org/jira/browse/FLINK-3342) | Operator checkpoint statistics state size overflow |  Major | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3338](https://issues.apache.org/jira/browse/FLINK-3338) | Kafka deserialization issue - ClassNotFoundException |  Major | . | Shikhar Bhushan | Stephan Ewen |
| [FLINK-3328](https://issues.apache.org/jira/browse/FLINK-3328) | Incorrectly shaded dependencies in flink-runtime |  Blocker | Build System | Stephan Ewen | Robert Metzger |
| [FLINK-3314](https://issues.apache.org/jira/browse/FLINK-3314) | Early cancel calls can cause Tasks to not cancel properly |  Blocker | Local Runtime | Stephan Ewen | Stephan Ewen |
| [FLINK-3300](https://issues.apache.org/jira/browse/FLINK-3300) | Concurrency Bug in Yarn JobManager |  Blocker | JobManager | Stephan Ewen | Maximilian Michels |
| [FLINK-3293](https://issues.apache.org/jira/browse/FLINK-3293) | Custom Application Name on YARN is ignored in deploy jobmanager mode |  Minor | YARN Client | Johannes | Johannes |
| [FLINK-3289](https://issues.apache.org/jira/browse/FLINK-3289) | Double reference to flink-contrib |  Trivial | Documentation | Stefano Baghino | Stefano Baghino |
| [FLINK-3287](https://issues.apache.org/jira/browse/FLINK-3287) | Flink Kafka Consumer fails due to Curator version conflict |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-3281](https://issues.apache.org/jira/browse/FLINK-3281) | IndexOutOfBoundsException when range-partitioning empty DataSet |  Major | Distributed Runtime, Local Runtime | Fridtjof Sander | Chengxiang Li |
| [FLINK-3280](https://issues.apache.org/jira/browse/FLINK-3280) | Wrong usage of Boolean.getBoolean() |  Major | . | Ted Yu | Robert Metzger |
| [FLINK-3274](https://issues.apache.org/jira/browse/FLINK-3274) | Prefix Kafka connector accumulators with unique id |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-3268](https://issues.apache.org/jira/browse/FLINK-3268) | Unstable test JobManagerSubmittedJobGraphsRecoveryITCase |  Critical | Tests | Stephan Ewen | Stephan Ewen |
| [FLINK-3267](https://issues.apache.org/jira/browse/FLINK-3267) | Disable reference tracking in Kryo fallback serializer |  Blocker | Local Runtime | Stephan Ewen | Stephan Ewen |
| [FLINK-3261](https://issues.apache.org/jira/browse/FLINK-3261) | Tasks should eagerly report back when they cannot start a checkpoint |  Blocker | Distributed Runtime | Stephan Ewen | Aljoscha Krettek |
| [FLINK-3255](https://issues.apache.org/jira/browse/FLINK-3255) | Chaining behavior should not depend on parallelism |  Major | Streaming | Stephan Ewen | Stephan Ewen |
| [FLINK-3254](https://issues.apache.org/jira/browse/FLINK-3254) | CombineFunction interface not respected |  Blocker | DataSet API | Fabian Hueske | Kostas |
| [FLINK-3252](https://issues.apache.org/jira/browse/FLINK-3252) | Checkpoint stats only displayed after click on graph |  Major | Webfrontend | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3251](https://issues.apache.org/jira/browse/FLINK-3251) | Checkpoint stats show ghost numbers |  Major | Webfrontend | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3250](https://issues.apache.org/jira/browse/FLINK-3250) | Savepoint coordinator requires too strict parallelism match |  Major | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3247](https://issues.apache.org/jira/browse/FLINK-3247) | Kafka Connector unusable with quickstarts - shading issue |  Blocker | Kafka Connector | Stephan Ewen | Robert Metzger |
| [FLINK-3242](https://issues.apache.org/jira/browse/FLINK-3242) | User-specified StateBackend is not Respected if Checkpointing is Disabled |  Blocker | Streaming | Aljoscha Krettek | Aljoscha Krettek |
| [FLINK-3236](https://issues.apache.org/jira/browse/FLINK-3236) | Flink user code classloader should have Flink classloader as parent classloader |  Major | Local Runtime | Stephan Ewen | Stephan Ewen |
| [FLINK-3220](https://issues.apache.org/jira/browse/FLINK-3220) | Flink does not start on Hortonworks Sandbox 2.3.2 due to missing class |  Blocker | Build System | Robert Metzger | Robert Metzger |
| [FLINK-3218](https://issues.apache.org/jira/browse/FLINK-3218) | Merging Hadoop configurations overrides user parameters |  Major | Java API | Greg Hogan | Greg Hogan |
| [FLINK-3206](https://issues.apache.org/jira/browse/FLINK-3206) | Heap size for non-pre-allocated off-heap memory |  Major | Start-Stop Scripts | Greg Hogan | Maximilian Michels |
| [FLINK-3197](https://issues.apache.org/jira/browse/FLINK-3197) | InputStream not closed in BinaryInputFormat#createStatistics |  Minor | . | Ted Yu |  |
| [FLINK-3196](https://issues.apache.org/jira/browse/FLINK-3196) | InputStream should be closed in EnvironmentInformation#getRevisionInformation() |  Minor | . | Ted Yu | Suneel Marthi |
| [FLINK-3189](https://issues.apache.org/jira/browse/FLINK-3189) | Error while parsing job arguments passed by CLI |  Minor | Command-line client | Filip Leczycki | Matthias J. Sax |
| [FLINK-3188](https://issues.apache.org/jira/browse/FLINK-3188) | Deletes in Kafka source should be passed on to KeyedDeserializationSchema |  Major | Kafka Connector | Sebastian Klemke | Robert Metzger |
| [FLINK-3185](https://issues.apache.org/jira/browse/FLINK-3185) | Silent failure during job graph recovery |  Major | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-3175](https://issues.apache.org/jira/browse/FLINK-3175) | KafkaITCase.testOffsetAutocommitTest |  Critical | Kafka Connector, Tests | Matthias J. Sax | Robert Metzger |
| [FLINK-3173](https://issues.apache.org/jira/browse/FLINK-3173) | Bump org.apache.httpcomponents.httpclient version to 4.2.6 |  Minor | . | Till Rohrmann | Till Rohrmann |
| [FLINK-3171](https://issues.apache.org/jira/browse/FLINK-3171) | Consolidate zoo of wrapper classes for input/output-stream to data-input/output-view |  Major | . | Stephan Ewen | Stephan Ewen |
| [FLINK-3166](https://issues.apache.org/jira/browse/FLINK-3166) | The first program in ObjectReuseITCase has the wrong expected result, and it succeeds |  Critical | Distributed Runtime, Documentation, Tests | Gabor Gevay | Greg Hogan |
| [FLINK-3157](https://issues.apache.org/jira/browse/FLINK-3157) | Web frontend json files contain author attribution |  Trivial | Webfrontend | Ufuk Celebi | Stephan Ewen |
| [FLINK-3156](https://issues.apache.org/jira/browse/FLINK-3156) | FlinkKafkaConsumer fails with NPE on notifyCheckpointComplete |  Major | Kafka Connector | Till Rohrmann | Robert Metzger |
| [FLINK-3151](https://issues.apache.org/jira/browse/FLINK-3151) | YARN kills Flink TM containers due to memory overuse (outside heap/offheap) |  Blocker | TaskManager | Robert Metzger | Ufuk Celebi |
| [FLINK-3145](https://issues.apache.org/jira/browse/FLINK-3145) | Storm examples can't be run without flink-java as dependency |  Major | Build System, Java API, Storm Compatibility | Maximilian Michels | Maximilian Michels |
| [FLINK-3143](https://issues.apache.org/jira/browse/FLINK-3143) | Update Clojure Cleaner's ASM references to ASM5 |  Major | Local Runtime | Maximilian Michels | Maximilian Michels |
| [FLINK-3136](https://issues.apache.org/jira/browse/FLINK-3136) | Scala Closure Cleaner uses wrong ASM import |  Critical | Scala API | Stephan Ewen | Aljoscha Krettek |
| [FLINK-3125](https://issues.apache.org/jira/browse/FLINK-3125) | Web dashboard does not start when log files are not found |  Major | Webfrontend | Stephan Ewen | Stephan Ewen |
| [FLINK-3121](https://issues.apache.org/jira/browse/FLINK-3121) | Watermark forwarding does not work for sources not producing any data |  Blocker | . | Robert Metzger | Aljoscha Krettek |
| [FLINK-3118](https://issues.apache.org/jira/browse/FLINK-3118) | Check if MessageFunction implements ResultTypeQueryable |  Major | Gelly | Martin Junghanns | Martin Junghanns |
| [FLINK-3108](https://issues.apache.org/jira/browse/FLINK-3108) | JoinOperator's with() calls the wrong TypeExtractor method |  Major | . | Vasia Kalavri | Timo Walther |
| [FLINK-3103](https://issues.apache.org/jira/browse/FLINK-3103) | Remove synchronization in FsStateBackend#FsCheckpointStateOutputStream#close() |  Major | . | Ted Yu | Ted Yu |
| [FLINK-3101](https://issues.apache.org/jira/browse/FLINK-3101) | Flink Kafka consumer crashes with NPE when it sees deleted record |  Major | Kafka Connector | Sanjar Akhmedov | Robert Metzger |
| [FLINK-3100](https://issues.apache.org/jira/browse/FLINK-3100) | Signal handler prints error on normal shutdown of cluster |  Major | JobManager, TaskManager | Maximilian Michels | Maximilian Michels |
| [FLINK-3098](https://issues.apache.org/jira/browse/FLINK-3098) | Cast from Date to Long throw compile error. |  Major | Table API | Chengxiang Li | Chengxiang Li |
| [FLINK-3087](https://issues.apache.org/jira/browse/FLINK-3087) | Table API do not support multi count in aggregation. |  Major | Table API | Chengxiang Li | Chengxiang Li |
| [FLINK-3082](https://issues.apache.org/jira/browse/FLINK-3082) | Confusing error about ManualTimestampSourceFunction |  Major | . | Niels Basjes | Niels Basjes |
| [FLINK-3081](https://issues.apache.org/jira/browse/FLINK-3081) | Kafka Periodic Offset Committer does not properly terminate on canceling |  Blocker | Kafka Connector | Stephan Ewen | Robert Metzger |
| [FLINK-3080](https://issues.apache.org/jira/browse/FLINK-3080) | Cannot union a data stream with a product of itself |  Major | Streaming | Vasia Kalavri | Aljoscha Krettek |
| [FLINK-3067](https://issues.apache.org/jira/browse/FLINK-3067) | Kafka source fails during checkpoint notifications with NPE |  Major | Kafka Connector | Gyula Fora | Robert Metzger |
| [FLINK-3061](https://issues.apache.org/jira/browse/FLINK-3061) | Kafka Consumer is not failing if broker is not available |  Major | Kafka Connector | Robert Metzger | Robert Metzger |
| [FLINK-3059](https://issues.apache.org/jira/browse/FLINK-3059) | Javadoc fix for DataSet.writeAsText() |  Trivial | . | jun aoki | jun aoki |
| [FLINK-3054](https://issues.apache.org/jira/browse/FLINK-3054) | Remove R (return) type variable from SerializationSchema |  Major | Streaming | Robert Metzger | Robert Metzger |
| [FLINK-3052](https://issues.apache.org/jira/browse/FLINK-3052) | Optimizer does not push properties out of bulk iterations |  Major | Optimizer | Till Rohrmann | Till Rohrmann |
| [FLINK-3048](https://issues.apache.org/jira/browse/FLINK-3048) | DataSinkTaskTest.testCancelDataSinkTask |  Critical | Tests | Matthias J. Sax | Stephan Ewen |
| [FLINK-3043](https://issues.apache.org/jira/browse/FLINK-3043) | Kafka Connector description in Streaming API guide is wrong/outdated |  Major | Documentation | Stephan Ewen | Stephan Ewen |
| [FLINK-3032](https://issues.apache.org/jira/browse/FLINK-3032) | Flink does not start on Hadoop 2.7.1 (HDP), due to class conflict |  Critical | Build System | Robert Metzger | Robert Metzger |
| [FLINK-3024](https://issues.apache.org/jira/browse/FLINK-3024) | TimestampExtractor Does not Work When returning Long.MIN\_VALUE |  Major | Streaming | Aljoscha Krettek | Aljoscha Krettek |
| [FLINK-3022](https://issues.apache.org/jira/browse/FLINK-3022) | Broken link 'Working With State' in Fault Tolerance Section of Stream Programming Guide |  Major | Documentation | Suneel Marthi | Suneel Marthi |
| [FLINK-3020](https://issues.apache.org/jira/browse/FLINK-3020) | Local streaming execution: set number of task manager slots to the maximum parallelism |  Minor | Local Runtime | Maximilian Michels | Maximilian Michels |
| [FLINK-3019](https://issues.apache.org/jira/browse/FLINK-3019) | CLI does not list running/restarting jobs |  Minor | Command-line client | Ufuk Celebi |  |
| [FLINK-3013](https://issues.apache.org/jira/browse/FLINK-3013) | Incorrect package declaration in GellyScalaAPICompletenessTest.scala |  Major | Gelly, Scala API | Suneel Marthi | Suneel Marthi |
| [FLINK-3011](https://issues.apache.org/jira/browse/FLINK-3011) | Cannot cancel failing/restarting streaming job from the command line |  Critical | Command-line client | Gyula Fora | Ufuk Celebi |
| [FLINK-3009](https://issues.apache.org/jira/browse/FLINK-3009) | Cannot build docs with Jekyll 3.0.0 |  Minor | Build System | Ufuk Celebi | jun aoki |
| [FLINK-3005](https://issues.apache.org/jira/browse/FLINK-3005) | Commons-collections object deserialization remote command execution vulnerability |  Major | . | Ted Yu | Ted Yu |
| [FLINK-3000](https://issues.apache.org/jira/browse/FLINK-3000) | Add ShutdownHook to YARN CLI to prevent lingering sessions |  Major | YARN Client | Ufuk Celebi | Sachin Goel |
| [FLINK-2992](https://issues.apache.org/jira/browse/FLINK-2992) | New Windowing code is using SerializationUtils with wrong classloader |  Critical | Streaming | Robert Metzger | Robert Metzger |
| [FLINK-2990](https://issues.apache.org/jira/browse/FLINK-2990) | Scala 2.11 build fails to start on YARN |  Major | Build System, YARN Client | Robert Metzger | Robert Metzger |
| [FLINK-2989](https://issues.apache.org/jira/browse/FLINK-2989) | Job Cancel button doesn't work on Yarn |  Major | Webfrontend | Sachin Goel | Maximilian Michels |
| [FLINK-2987](https://issues.apache.org/jira/browse/FLINK-2987) | Flink 0.10 fails to start on YARN 2.6.0 |  Major | Build System, YARN Client | Robert Metzger | Robert Metzger |
| [FLINK-2979](https://issues.apache.org/jira/browse/FLINK-2979) | RollingSink does not work with Hadoop 2.7.1 |  Major | Streaming Connectors | Till Rohrmann | Aljoscha Krettek |
| [FLINK-2977](https://issues.apache.org/jira/browse/FLINK-2977) | Cannot access HBase in a Kerberos secured Yarn cluster |  Major | YARN Client | Niels Basjes | Niels Basjes |
| [FLINK-2967](https://issues.apache.org/jira/browse/FLINK-2967) | TM address detection might not always detect the right interface on slow networks / overloaded JMs |  Major | . | Robert Metzger | Robert Metzger |
| [FLINK-2963](https://issues.apache.org/jira/browse/FLINK-2963) | Dependence on SerializationUtils#deserialize() should be avoided |  Minor | . | Ted Yu | Robert Metzger |
| [FLINK-2958](https://issues.apache.org/jira/browse/FLINK-2958) | StreamingJobGraphGenerator sets hard coded number execution retry |  Major | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-2954](https://issues.apache.org/jira/browse/FLINK-2954) | Not able to pass custom environment variables in cluster to processes that spawning TaskManager |  Critical | Command-line client, Distributed Runtime | Jian Jiang | Robert Metzger |
| [FLINK-2950](https://issues.apache.org/jira/browse/FLINK-2950) | Markdown presentation problem in SVM documentation |  Minor | Documentation, Machine Learning Library | Chiwan Park | Chiwan Park |
| [FLINK-2942](https://issues.apache.org/jira/browse/FLINK-2942) | Dangling operators in web UI's program visualization (non-deterministic) |  Critical | Webfrontend | Fabian Hueske | Piotr Godek |
| [FLINK-2938](https://issues.apache.org/jira/browse/FLINK-2938) | Streaming docs not in sync with latest state changes |  Minor | Documentation | Maximilian Michels | Stephan Ewen |
| [FLINK-2937](https://issues.apache.org/jira/browse/FLINK-2937) | Typo in Quickstart-\>Scala API-\>Alternative Build Tools: SBT |  Trivial | Documentation | Theodore Vasiloudis | Chesnay Schepler |
| [FLINK-2934](https://issues.apache.org/jira/browse/FLINK-2934) | Remove placehoder pages in Web dashboard |  Major | . | Sachin Goel | Sachin Goel |
| [FLINK-2930](https://issues.apache.org/jira/browse/FLINK-2930) | ExecutionConfig execution retry delay not respected |  Major | Distributed Runtime | Ufuk Celebi | Ufuk Celebi |
| [FLINK-2914](https://issues.apache.org/jira/browse/FLINK-2914) | Missing break in ZooKeeperSubmittedJobGraphStore#SubmittedJobGraphsPathCacheListener#childEvent() |  Minor | . | Ted Yu | Chesnay Schepler |
| [FLINK-2913](https://issues.apache.org/jira/browse/FLINK-2913) | Close of ObjectOutputStream should be enclosed in finally block in FsStateBackend |  Minor | . | Ted Yu | Ted Yu |
| [FLINK-2879](https://issues.apache.org/jira/browse/FLINK-2879) | Links in documentation are broken |  Minor | website | Nikolaas Steenbergen | Andra Lungu |
| [FLINK-2845](https://issues.apache.org/jira/browse/FLINK-2845) | TimestampITCase.testWatermarkPropagation |  Critical | Streaming | Matthias J. Sax | Aljoscha Krettek |
| [FLINK-2827](https://issues.apache.org/jira/browse/FLINK-2827) | Potential resource leak in TwitterSource#loadAuthenticationProperties() |  Minor | . | Ted Yu | Saumitra Shahapure |
| [FLINK-2826](https://issues.apache.org/jira/browse/FLINK-2826) | transformed is modified in BroadcastVariableMaterialization#decrementReferenceInternal without proper locking |  Major | . | Ted Yu | Ted Yu |
| [FLINK-2800](https://issues.apache.org/jira/browse/FLINK-2800) | kryo serialization problem |  Major | Type Serialization System | Stefano Bortoli | Till Rohrmann |
| [FLINK-2797](https://issues.apache.org/jira/browse/FLINK-2797) | CLI: Missing option to submit jobs in detached mode |  Major | Command-line client | Maximilian Michels | Sachin Goel |
| [FLINK-2671](https://issues.apache.org/jira/browse/FLINK-2671) | Instable Test StreamCheckpointNotifierITCase |  Critical | Tests | Matthias J. Sax | Stephan Ewen |
| [FLINK-2622](https://issues.apache.org/jira/browse/FLINK-2622) | Scala DataStream API does not have writeAsText method which supports WriteMode |  Major | Scala API, Streaming | Till Rohrmann | Till Rohrmann |
| [FLINK-2586](https://issues.apache.org/jira/browse/FLINK-2586) | Unstable Storm Compatibility Tests |  Critical | Storm Compatibility | Stephan Ewen | Matthias J. Sax |
| [FLINK-2348](https://issues.apache.org/jira/browse/FLINK-2348) | IterateExampleITCase failing |  Critical | Streaming | Matthias J. Sax | Stephan Ewen |
| [FLINK-2115](https://issues.apache.org/jira/browse/FLINK-2115) | TableAPI throws ExpressionException for "Dangling GroupBy operation" |  Major | Table API | Fabian Hueske | Chengxiang Li |
| [FLINK-1644](https://issues.apache.org/jira/browse/FLINK-1644) | WebClient dies when no ExecutionEnvironment in main method |  Minor | Webfrontend | Jonathan Hasenburg |  |
| [FLINK-1278](https://issues.apache.org/jira/browse/FLINK-1278) | Remove the Record special code paths |  Minor | Local Runtime | Stephan Ewen | Stephan Ewen |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-3285](https://issues.apache.org/jira/browse/FLINK-3285) | Skip Maven deployment of flink-java8 |  Major | Java API | Maximilian Michels | Maximilian Michels |
| [FLINK-3224](https://issues.apache.org/jira/browse/FLINK-3224) | The Streaming API does not call setInputType if a format implements InputTypeConfigurable |  Major | DataStream API | Nick Dimiduk |  |
| [FLINK-3208](https://issues.apache.org/jira/browse/FLINK-3208) | Rename Gelly vertex-centric model to scatter-gather |  Major | Gelly | Vasia Kalavri | Vasia Kalavri |
| [FLINK-3195](https://issues.apache.org/jira/browse/FLINK-3195) | Restructure examples projects and package streaming examples |  Major | Examples | Stephan Ewen | Stephan Ewen |
| [FLINK-3071](https://issues.apache.org/jira/browse/FLINK-3071) | Add asynchronous materialization thread |  Major | Streaming | Stephan Ewen | Aljoscha Krettek |
| [FLINK-3070](https://issues.apache.org/jira/browse/FLINK-3070) | Create an asynchronous state handle interface |  Major | Streaming | Stephan Ewen | Aljoscha Krettek |
| [FLINK-3057](https://issues.apache.org/jira/browse/FLINK-3057) | [py] Provide a way to pass information back to the plan process |  Minor | Python API | Chesnay Schepler | Chesnay Schepler |
| [FLINK-2972](https://issues.apache.org/jira/browse/FLINK-2972) | Remove Twitter Chill dependency from flink-java module |  Major | Java API | Fabian Hueske |  |
| [FLINK-2933](https://issues.apache.org/jira/browse/FLINK-2933) | Flink scala libraries exposed with maven should carry scala version |  Minor | Build System | Frederick F. Kautz IV | Maximilian Michels |
| [FLINK-2919](https://issues.apache.org/jira/browse/FLINK-2919) | Apply JMH on FieldAccessMinibenchmark class. |  Minor | Tests | GaoLun | GaoLun |
| [FLINK-2890](https://issues.apache.org/jira/browse/FLINK-2890) | Apply JMH on StringSerializationSpeedBenchmark class. |  Minor | Tests | GaoLun | GaoLun |
| [FLINK-2889](https://issues.apache.org/jira/browse/FLINK-2889) | Apply JMH on LongSerializationSpeedBenchmark class |  Minor | Tests | GaoLun | GaoLun |
| [FLINK-2853](https://issues.apache.org/jira/browse/FLINK-2853) | Apply JMH on MutableHashTablePerformanceBenchmark class. |  Minor | Tests | GaoLun | GaoLun |
| [FLINK-2850](https://issues.apache.org/jira/browse/FLINK-2850) | Limit the types of jobs which can run in detached mode |  Major | . | Sachin Goel | Sachin Goel |
| [FLINK-1982](https://issues.apache.org/jira/browse/FLINK-1982) | Remove dependencies on Record for Flink runtime and core |  Major | Core | Henry Saputra | Fabian Hueske |
| [FLINK-146](https://issues.apache.org/jira/browse/FLINK-146) | Sorted output not working |  Major | Distributed Runtime, Java API, Scala API | Fabian Hueske |  |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [FLINK-2429](https://issues.apache.org/jira/browse/FLINK-2429) | Remove the "enableCheckpointing()" without interval variant |  Minor | Streaming | Stephan Ewen | Stephan Ewen |
| [FLINK-3186](https://issues.apache.org/jira/browse/FLINK-3186) | Deprecate DataSink.sortLocalOutput() methods |  Major | DataSet API | Fabian Hueske | Suneel Marthi |
| [FLINK-3113](https://issues.apache.org/jira/browse/FLINK-3113) | Remove unused global order methods from GenericDataSinkBase |  Minor | Core | Fabian Hueske | Fabian Hueske |
| [FLINK-3112](https://issues.apache.org/jira/browse/FLINK-3112) | Remove unused RecordModelPostPass class |  Trivial | Optimizer | Fabian Hueske | Fabian Hueske |


