
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
# Apache BigTop Changelog

## Release 1.2.0 - Unreleased (as of 2016-03-01)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [BIGTOP-2339](https://issues.apache.org/jira/browse/BIGTOP-2339) | add centos-7 to the provisioiner matrix |  Major | provisioner | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2296](https://issues.apache.org/jira/browse/BIGTOP-2296) | Provide a way to build Docker container with functional stack |  Major | docker, general | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-1641](https://issues.apache.org/jira/browse/BIGTOP-1641) | Add packaging for Apache Tajo |  Major | debian, rpm, tests | YoungWoo Kim | Yeongeon KIM |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [BIGTOP-2337](https://issues.apache.org/jira/browse/BIGTOP-2337) | Fix script to make deb in Tajo |  Major | . | Yeongeon KIM | Yeongeon KIM |
| [BIGTOP-2332](https://issues.apache.org/jira/browse/BIGTOP-2332) | Upgrade Tajo version to 0.11.1 |  Major | . | Yeongeon KIM | Yeongeon KIM |
| [BIGTOP-2118](https://issues.apache.org/jira/browse/BIGTOP-2118) | Update HBase to 0.98.17 |  Minor | . | Andrew Purtell | YoungWoo Kim |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [BIGTOP-2347](https://issues.apache.org/jira/browse/BIGTOP-2347) | Clean up build directory after sucessfull build of package (2nd try) |  Major | build | Olaf Flebbe | Olaf Flebbe |
| [BIGTOP-2346](https://issues.apache.org/jira/browse/BIGTOP-2346) | Do not use gradle delete() for sources and build directories |  Major | build | Olaf Flebbe | Olaf Flebbe |
| [BIGTOP-2340](https://issues.apache.org/jira/browse/BIGTOP-2340) | BIGTOP-2319 is incomplete: the code for smoke-tests is missing |  Major | tests | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2318](https://issues.apache.org/jira/browse/BIGTOP-2318) | Release assembly needs to be updated |  Major | build | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2308](https://issues.apache.org/jira/browse/BIGTOP-2308) | Clean up build directory after sucessfull build of package |  Major | debian | Olaf Flebbe | Olaf Flebbe |
| [BIGTOP-2303](https://issues.apache.org/jira/browse/BIGTOP-2303) | Fix the indentation in docker-hadoop.sh |  Minor | . | Faraaz Sareshwala | Faraaz Sareshwala |
| [BIGTOP-2302](https://issues.apache.org/jira/browse/BIGTOP-2302) | Use apt instead of yum in setup-env-debian.sh |  Minor | . | Faraaz Sareshwala | Faraaz Sareshwala |
| [BIGTOP-2301](https://issues.apache.org/jira/browse/BIGTOP-2301) | Bigtop Homepage shows wrong url to CI |  Major | website | Olaf Flebbe | Olaf Flebbe |
| [BIGTOP-2229](https://issues.apache.org/jira/browse/BIGTOP-2229) | bigtop deploy to support centos-7 |  Major | docker | Olaf Flebbe | Konstantin Boudnik |
| [BIGTOP-2220](https://issues.apache.org/jira/browse/BIGTOP-2220) | flume-agent.init incorrectly handles flume.conf |  Major | . | Teruyoshi Zenmyo | Teruyoshi Zenmyo |
| [BIGTOP-2136](https://issues.apache.org/jira/browse/BIGTOP-2136) | A comment about parameter substitution in BPS\_analytics.pig is slightly wrong |  Trivial | blueprints | Kengo Seki | Kengo Seki |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [BIGTOP-2319](https://issues.apache.org/jira/browse/BIGTOP-2319) | Build initial smoke-tests distribution |  Major | build, tests | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2314](https://issues.apache.org/jira/browse/BIGTOP-2314) | Added deb and rpm package of Apache Apex to bigtop. |  Major | debian, rpm | Chinmay Kolhatkar | Chinmay Kolhatkar |
| [BIGTOP-2180](https://issues.apache.org/jira/browse/BIGTOP-2180) | Apache Tajo to bigtop: make tests |  Major | tests | Yeongeon KIM | Yeongeon KIM |
| [BIGTOP-2179](https://issues.apache.org/jira/browse/BIGTOP-2179) | Apache Tajo to bigtop: packaging as deb/rpm |  Major | debian, rpm, tests | Yeongeon KIM | Yeongeon KIM |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [BIGTOP-2335](https://issues.apache.org/jira/browse/BIGTOP-2335) | ci link should use https:// authority |  Major | website | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2334](https://issues.apache.org/jira/browse/BIGTOP-2334) | Update latest release link on the website |  Major | website | Konstantin Boudnik | Konstantin Boudnik |
| [BIGTOP-2289](https://issues.apache.org/jira/browse/BIGTOP-2289) | Set master version to 1.2.0-SNAPSHOT |  Major | general | Konstantin Boudnik | Konstantin Boudnik |


