
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
# Apache Hadoop Yetus Changelog

## Release HADOOP-12111 - Unreleased

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-12156](https://issues.apache.org/jira/browse/HADOOP-12156) | modernize smart-apply-patch |  Major | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-12135](https://issues.apache.org/jira/browse/HADOOP-12135) | cleanup releasedocmaker |  Major | yetus | Allen Wittenauer | Allen Wittenauer |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11807](https://issues.apache.org/jira/browse/HADOOP-11807) | add a lint mode to releasedocmaker |  Minor | build, documentation, yetus | Allen Wittenauer | ramtin |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-12237](https://issues.apache.org/jira/browse/HADOOP-12237) | releasedocmaker.py doesn't work behind a proxy |  Major | yetus | Tsuyoshi Ozawa | Tsuyoshi Ozawa |
| [HADOOP-12226](https://issues.apache.org/jira/browse/HADOOP-12226) | CHANGED\_MODULES is wrong for ant |  Major | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-12225](https://issues.apache.org/jira/browse/HADOOP-12225) | Add docs-overview page |  Major | yetus | Sean Busbey | Sean Busbey |
| [HADOOP-12206](https://issues.apache.org/jira/browse/HADOOP-12206) | The preceding invocations of findlargest in test-patch effect the following invocation results |  Major | yetus | Kengo Seki | Kengo Seki |
| [HADOOP-12202](https://issues.apache.org/jira/browse/HADOOP-12202) | releasedocmaker drops missing component and assignee entries |  Blocker | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-12199](https://issues.apache.org/jira/browse/HADOOP-12199) | Optimize find\_changed\_modules |  Trivial | yetus | Allen Wittenauer | Kengo Seki |
| [HADOOP-12197](https://issues.apache.org/jira/browse/HADOOP-12197) | smart-apply-patch shouldn't print successful dryrun in apply mode |  Major | yetus | Allen Wittenauer | Kengo Seki |
| [HADOOP-12196](https://issues.apache.org/jira/browse/HADOOP-12196) | shellcheck plugin is picking up target executables |  Major | yetus | Allen Wittenauer | Kengo Seki |
| [HADOOP-12188](https://issues.apache.org/jira/browse/HADOOP-12188) | javac warning file is always empty on ant-based projects |  Major | yetus | Kengo Seki | Kengo Seki |
| [HADOOP-12187](https://issues.apache.org/jira/browse/HADOOP-12187) | Whitespace plugin shows unexpected error messages if gitdiffcontent is empty |  Minor | yetus | Kengo Seki | Kengo Seki |
| [HADOOP-12165](https://issues.apache.org/jira/browse/HADOOP-12165) | author tests show entire run time not test time when skipped |  Trivial | yetus | Allen Wittenauer | Kengo Seki |
| [HADOOP-12157](https://issues.apache.org/jira/browse/HADOOP-12157) | test-patch should report max memory consumed |  Minor | yetus | Allen Wittenauer | Kengo Seki |
| [HADOOP-12147](https://issues.apache.org/jira/browse/HADOOP-12147) | bundled dockerfile should use the JDK version of openjdk, not JRE |  Trivial | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-12142](https://issues.apache.org/jira/browse/HADOOP-12142) | Test code modification is not detected if test directory is at the top level of the project |  Major | yetus | Kengo Seki | Kengo Seki |
| [HADOOP-12134](https://issues.apache.org/jira/browse/HADOOP-12134) | Pig personality always fails at precheck\_javac and check\_patch\_javac |  Major | yetus | Kengo Seki | Kengo Seki |
| [HADOOP-12127](https://issues.apache.org/jira/browse/HADOOP-12127) | some personalities are still using releaseaudit instead of asflicense |  Trivial | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-12113](https://issues.apache.org/jira/browse/HADOOP-12113) | update test-patch branch to latest code |  Major | yetus | Allen Wittenauer | Allen Wittenauer |
| [HADOOP-11914](https://issues.apache.org/jira/browse/HADOOP-11914) | test-patch.sh confused by certain patch formats |  Critical | yetus | Allen Wittenauer | Kengo Seki |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |

