
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
# Apache Tez Changelog

## Release 0.8.3 - Unreleased (as of 2016-02-24)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [TEZ-3093](https://issues.apache.org/jira/browse/TEZ-3093) | CriticalPathAnalyzer should be accessible via zeppelin |  Major | . | Rajesh Balamohan | Rajesh Balamohan |
| [TEZ-3090](https://issues.apache.org/jira/browse/TEZ-3090) | MRInput should make dagIdentifier, vertexIdentifier, etc available to the InputFormat jobConf |  Major | . | Siddharth Seth | Siddharth Seth |
| [TEZ-3079](https://issues.apache.org/jira/browse/TEZ-3079) | Fix tez-tfile parser documentation |  Major | . | Rajesh Balamohan | Rajesh Balamohan |
| [TEZ-2974](https://issues.apache.org/jira/browse/TEZ-2974) | Tez tools: TFileRecordReader in tez-tools should support reading \>2 GB tfiles |  Major | . | Rajesh Balamohan | Rajesh Balamohan |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [TEZ-3135](https://issues.apache.org/jira/browse/TEZ-3135) | tez-ext-service-tests, tez-plugins/tez-yarn-timeline-history and tez-tools/tez-javadoc-tools missing dependencies |  Major | . | Vijay Kumar | Vijay Kumar |
| [TEZ-3134](https://issues.apache.org/jira/browse/TEZ-3134) | tez-dag should depend on commons-collections4 |  Trivial | . | Hitesh Shah | Hitesh Shah |
| [TEZ-3131](https://issues.apache.org/jira/browse/TEZ-3131) | Support a way to override test\_root\_dir for FaultToleranceTestRunner |  Minor | . | Hitesh Shah | Hitesh Shah |
| [TEZ-3126](https://issues.apache.org/jira/browse/TEZ-3126) | Log reason for not reducing parallelism |  Minor | . | Jonathan Eagles | Jonathan Eagles |
| [TEZ-3124](https://issues.apache.org/jira/browse/TEZ-3124) | Running task hangs due to missing event to initialize input in recovery |  Major | . | Jeff Zhang | Jeff Zhang |
| [TEZ-3123](https://issues.apache.org/jira/browse/TEZ-3123) | Containers can get re-used even with conflicting local resources |  Major | . | Hitesh Shah | Hitesh Shah |
| [TEZ-3117](https://issues.apache.org/jira/browse/TEZ-3117) | Deadlock in Edge and Vertex code |  Major | . | Yesha Vora | Bikas Saha |
| [TEZ-3104](https://issues.apache.org/jira/browse/TEZ-3104) | Tez fails on Bzip2 intermediate output format on hadoop 2.7.1 and earlier |  Critical | . | Jonathan Eagles | Jonathan Eagles |
| [TEZ-3101](https://issues.apache.org/jira/browse/TEZ-3101) | Tez UI: Task attempt log link doesn't have the correct protocol |  Major | . | Sreenath Somarajapuram | Sreenath Somarajapuram |
| [TEZ-3089](https://issues.apache.org/jira/browse/TEZ-3089) | TaskConcurrencyAnalyzer can return negative task count with very large jobs |  Major | . | Rajesh Balamohan | Rajesh Balamohan |
| [TEZ-3081](https://issues.apache.org/jira/browse/TEZ-3081) | Update tez website for trademarks feedback |  Major | . | Hitesh Shah | Hitesh Shah |
| [TEZ-3076](https://issues.apache.org/jira/browse/TEZ-3076) | Reduce merge memory overhead to support large number of in-memory mapoutputs |  Major | . | Jonathan Eagles | Jonathan Eagles |
| [TEZ-3067](https://issues.apache.org/jira/browse/TEZ-3067) | Links to tez configs documentation should be bubbled up to top-level release page |  Major | . | Hitesh Shah | Tsuyoshi Ozawa |
| [TEZ-3066](https://issues.apache.org/jira/browse/TEZ-3066) | TaskAttemptFinishedEvent ConcurrentModificationException in recovery or history logging services |  Major | . | Jason Lowe | Jeff Zhang |
| [TEZ-3053](https://issues.apache.org/jira/browse/TEZ-3053) | Containers timeout if they do not receive a task within the container timeout interval |  Major | . | Siddharth Seth | Siddharth Seth |
| [TEZ-3052](https://issues.apache.org/jira/browse/TEZ-3052) | Task internal error due to Invalid event: T\_ATTEMPT\_FAILED at FAILED |  Major | . | Jason Lowe | Jason Lowe |
| [TEZ-3037](https://issues.apache.org/jira/browse/TEZ-3037) | History URL should be set regardless of which history logging service is enabled |  Major | . | Hitesh Shah | Hitesh Shah |
| [TEZ-3036](https://issues.apache.org/jira/browse/TEZ-3036) | Tez AM can hang on startup with no indication of error |  Critical | . | Jason Lowe | Jason Lowe |
| [TEZ-3032](https://issues.apache.org/jira/browse/TEZ-3032) | DAG start time getting logged using system time instead of recorded time in startTime field |  Minor | . | Hitesh Shah | Hitesh Shah |
| [TEZ-2937](https://issues.apache.org/jira/browse/TEZ-2937) | Can Processor.close() be called after closing inputs and outputs? |  Major | . | Rohini Palaniswamy | Jonathan Eagles |
| [TEZ-2898](https://issues.apache.org/jira/browse/TEZ-2898) | tez tools : swimlanes.py is broken in master |  Major | . | Rajesh Balamohan | Rajesh Balamohan |
| [TEZ-2307](https://issues.apache.org/jira/browse/TEZ-2307) | Possible wrong error message when submitting new dag |  Major | . | Jeff Zhang | Jeff Zhang |
| [TEZ-1491](https://issues.apache.org/jira/browse/TEZ-1491) | Tez reducer-side merge's counter update is slow |  Major | . | Gopal V | Gopal V |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [TEZ-3029](https://issues.apache.org/jira/browse/TEZ-3029) | Add an onError method to service plugin contexts |  Major | . | Siddharth Seth | Siddharth Seth |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [TEZ-3033](https://issues.apache.org/jira/browse/TEZ-3033) | changes for 0.8.2 release |  Major | . | Siddharth Seth | Siddharth Seth |
| [TEZ-2594](https://issues.apache.org/jira/browse/TEZ-2594) | Fix LICENSE for missing entries for full and minimal tarballs |  Major | . | Hitesh Shah | Hitesh Shah |


