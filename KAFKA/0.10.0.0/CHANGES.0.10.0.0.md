
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
# Apache Kafka Changelog

## Release 0.10.0.0 - Unreleased (as of 2016-03-01)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3044](https://issues.apache.org/jira/browse/KAFKA-3044) | Consumer.poll doesnot return messages when poll interval is less |  Major | clients | Praveen Devarao | Praveen Devarao |
| [KAFKA-3029](https://issues.apache.org/jira/browse/KAFKA-3029) | Make class org.apache.kafka.common.TopicPartition Serializable |  Major | clients | Praveen Devarao | Praveen Devarao |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3046](https://issues.apache.org/jira/browse/KAFKA-3046) | add ByteBuffer Serializer&Deserializer |  Major | clients | Xin Wang |  |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3291](https://issues.apache.org/jira/browse/KAFKA-3291) | DumpLogSegment tool should also provide an option to only verify index sanity. |  Major | tools | Parth Brahmbhatt | Parth Brahmbhatt |
| [KAFKA-3273](https://issues.apache.org/jira/browse/KAFKA-3273) | MessageFormatter and MessageReader interfaces should be resilient to changes |  Major | tools | Ismael Juma | Ismael Juma |
| [KAFKA-3272](https://issues.apache.org/jira/browse/KAFKA-3272) | Add debugging options to kafka-run-class.sh so we can easily run remote debugging |  Minor | tools | Christian Posta |  |
| [KAFKA-3259](https://issues.apache.org/jira/browse/KAFKA-3259) | KIP-31/KIP-32 clean-ups |  Major | . | Ismael Juma | Ismael Juma |
| [KAFKA-3253](https://issues.apache.org/jira/browse/KAFKA-3253) | Skip duplicate message size check if there is no re-compression during log appending. |  Major | . | Jiangjie Qin | Ismael Juma |
| [KAFKA-3227](https://issues.apache.org/jira/browse/KAFKA-3227) | Conservative update of Kafka dependencies |  Major | build | Ismael Juma | Ismael Juma |
| [KAFKA-3191](https://issues.apache.org/jira/browse/KAFKA-3191) | Improve offset committing JavaDoc in KafkaConsumer |  Minor | consumer | Adam Kunicki | Adam Kunicki |
| [KAFKA-3164](https://issues.apache.org/jira/browse/KAFKA-3164) | Document client and mirrormaker upgrade procedure/requirements |  Minor | . | Grant Henke | Grant Henke |
| [KAFKA-3162](https://issues.apache.org/jira/browse/KAFKA-3162) | KIP-42: Add Producer and Consumer Interceptors |  Major | . | Anna Povzner | Anna Povzner |
| [KAFKA-3119](https://issues.apache.org/jira/browse/KAFKA-3119) | Adding -daemon option to zookeeper-server-start.sh USAGE |  Minor | config | Atul Soman | Atul Soman |
| [KAFKA-3116](https://issues.apache.org/jira/browse/KAFKA-3116) | Failure to build |  Major | build | edwardt | Vahid Hashemian |
| [KAFKA-3105](https://issues.apache.org/jira/browse/KAFKA-3105) | Use `Utils.atomicMoveWithFallback` instead of `File.rename` |  Major | . | Ismael Juma | Ismael Juma |
| [KAFKA-3093](https://issues.apache.org/jira/browse/KAFKA-3093) | Keep track of connector and task status info, expose it via the REST API |  Major | copycat | jin xing | Jason Gustafson |
| [KAFKA-3092](https://issues.apache.org/jira/browse/KAFKA-3092) | Rename SinkTask.onPartitionsAssigned/onPartitionsRevoked and Clarify Contract |  Major | copycat | Jason Gustafson | Jason Gustafson |
| [KAFKA-3086](https://issues.apache.org/jira/browse/KAFKA-3086) | unused handle method in MirrorMakerMessageHandler |  Major | . | Jun Rao | Jakub Nowak |
| [KAFKA-3084](https://issues.apache.org/jira/browse/KAFKA-3084) | Topic existence checks in topic commands (create, alter, delete) |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-3077](https://issues.apache.org/jira/browse/KAFKA-3077) | Enable KafkaLog4jAppender to work with SASL enabled brokers. |  Major | clients | Ashish K Singh | Ashish K Singh |
| [KAFKA-3076](https://issues.apache.org/jira/browse/KAFKA-3076) | BrokerChangeListener should log the brokers in order |  Major | core | Jun Rao | Konrad Kalita |
| [KAFKA-3058](https://issues.apache.org/jira/browse/KAFKA-3058) | remove the usage of deprecated config properties |  Major | core | Jun Rao | Konrad Kalita |
| [KAFKA-3043](https://issues.apache.org/jira/browse/KAFKA-3043) | Replace request.required.acks with acks in docs |  Major | website | Sasaki Toru |  |
| [KAFKA-3024](https://issues.apache.org/jira/browse/KAFKA-3024) | Remove old patch review tools |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-3019](https://issues.apache.org/jira/browse/KAFKA-3019) | Add an exceptionName method to Errors |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-3012](https://issues.apache.org/jira/browse/KAFKA-3012) | Avoid reserved.broker.max.id collisions on upgrade |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-3007](https://issues.apache.org/jira/browse/KAFKA-3007) | Implement max.poll.records for new consumer (KIP-41) |  Major | consumer | aarti gupta | Jason Gustafson |
| [KAFKA-3002](https://issues.apache.org/jira/browse/KAFKA-3002) | Make available to specify hostname with Uppercase at broker list |  Minor | clients | Sasaki Toru |  |
| [KAFKA-2992](https://issues.apache.org/jira/browse/KAFKA-2992) | Trace log statements in the replica fetcher inner loop create large amounts of garbage |  Minor | core | Cory Kolbeck |  |
| [KAFKA-2964](https://issues.apache.org/jira/browse/KAFKA-2964) | Split Security Rolling Upgrade Test By Client and Broker Protocols |  Minor | . | Ben Stopford | Ben Stopford |
| [KAFKA-2958](https://issues.apache.org/jira/browse/KAFKA-2958) | Remove duplicate API key mapping functionality |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-2957](https://issues.apache.org/jira/browse/KAFKA-2957) | Fix typos in Kafka documentation |  Trivial | . | Vahid Hashemian | Vahid Hashemian |
| [KAFKA-2929](https://issues.apache.org/jira/browse/KAFKA-2929) | Migrate server side error mapping functionality |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-2881](https://issues.apache.org/jira/browse/KAFKA-2881) | Documentation improvement |  Major | . | Gwen Shapira | Guozhang Wang |
| [KAFKA-2879](https://issues.apache.org/jira/browse/KAFKA-2879) | Make MiniKDC test service slightly more generic |  Major | . | Gwen Shapira | Gwen Shapira |
| [KAFKA-2668](https://issues.apache.org/jira/browse/KAFKA-2668) | Add a metric that records the total number of metrics |  Major | . | Joel Koshy | Dong Lin |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3292](https://issues.apache.org/jira/browse/KAFKA-3292) | ClientQuotaManager.getOrCreateQuotaSensors() may return a null ClientSensors.throttleTimeSensor |  Major | . | Jun Rao | Ismael Juma |
| [KAFKA-3280](https://issues.apache.org/jira/browse/KAFKA-3280) | KafkaConsumer Javadoc contains misleading description of heartbeat behavior and correct use |  Major | consumer | Richard Whaling | Neha Narkhede |
| [KAFKA-3278](https://issues.apache.org/jira/browse/KAFKA-3278) | clientId is not unique in producer/consumer registration leads to mbean warning |  Minor | kafka streams | Tom Dearman | Tom Dearman |
| [KAFKA-3256](https://issues.apache.org/jira/browse/KAFKA-3256) | Large number of system test failures |  Major | . | Geoff Anderson | Jiangjie Qin |
| [KAFKA-3243](https://issues.apache.org/jira/browse/KAFKA-3243) | Fix Kafka basic ops documentation for Mirror maker, blacklist is not supported for new consumers |  Major | . | Ashish K Singh | Ashish K Singh |
| [KAFKA-3242](https://issues.apache.org/jira/browse/KAFKA-3242) | "Add Partition" log message doesn't actually indicate adding a partition |  Major | . | Gwen Shapira |  |
| [KAFKA-3235](https://issues.apache.org/jira/browse/KAFKA-3235) | Unclosed stream in AppInfoParser static block |  Minor | . | Ted Yu |  |
| [KAFKA-3229](https://issues.apache.org/jira/browse/KAFKA-3229) | Root statestore is not registered with ProcessorStateManager, inner state store is registered instead |  Major | kafka streams | Tom Dearman | Tom Dearman |
| [KAFKA-3225](https://issues.apache.org/jira/browse/KAFKA-3225) | Method commit() of class SourceTask never invoked |  Major | copycat | Krzysztof Dębski | Ewen Cheslack-Postava |
| [KAFKA-3217](https://issues.apache.org/jira/browse/KAFKA-3217) | Unit tests which dont close producers auto-create topics in Kafka brokers of other tests when port is reused |  Major | unit tests | Rajini Sivaram | Rajini Sivaram |
| [KAFKA-3216](https://issues.apache.org/jira/browse/KAFKA-3216) | "Modifying topics" section incorrectly says you can't change replication factor. |  Major | . | James Cheng | James Cheng |
| [KAFKA-3211](https://issues.apache.org/jira/browse/KAFKA-3211) | Handle Connect WorkerTask shutdown before startup correctly |  Major | copycat | Jason Gustafson | Jason Gustafson |
| [KAFKA-3207](https://issues.apache.org/jira/browse/KAFKA-3207) | StateStore seems to be writing state to one topic but restoring from another |  Blocker | kafka streams | Tom Dearman | Guozhang Wang |
| [KAFKA-3198](https://issues.apache.org/jira/browse/KAFKA-3198) | Ticket Renewal Thread exits prematurely due to inverted comparison |  Critical | security | Adam Kunicki | Adam Kunicki |
| [KAFKA-3195](https://issues.apache.org/jira/browse/KAFKA-3195) | Transient test failure in OffsetCheckpointTest.testReadWrite |  Major | kafka streams | Ewen Cheslack-Postava | Ismael Juma |
| [KAFKA-3194](https://issues.apache.org/jira/browse/KAFKA-3194) | Validate security.inter.broker.protocol against the advertised.listeners protocols |  Major | core | Grant Henke | Grant Henke |
| [KAFKA-3189](https://issues.apache.org/jira/browse/KAFKA-3189) | Kafka server returns UnknownServerException for inherited exceptions |  Major | core | Jiangjie Qin | Grant Henke |
| [KAFKA-3179](https://issues.apache.org/jira/browse/KAFKA-3179) | Kafka consumer delivers message whose offset is earlier than sought offset. |  Major | clients | Jiangjie Qin | Jiangjie Qin |
| [KAFKA-3147](https://issues.apache.org/jira/browse/KAFKA-3147) | Memory records is not writable in MirrorMaker |  Major | . | Meghana Narasimhan | Mayuresh Gharat |
| [KAFKA-3141](https://issues.apache.org/jira/browse/KAFKA-3141) | kafka-acls.sh throws ArrayIndexOutOfBoundsException for an invalid authorizer-property |  Major | . | Ashish K Singh | Ashish K Singh |
| [KAFKA-3140](https://issues.apache.org/jira/browse/KAFKA-3140) | PatternSyntaxException thrown in MM, causes MM to hang |  Major | tools | Ashish K Singh | Ashish K Singh |
| [KAFKA-3138](https://issues.apache.org/jira/browse/KAFKA-3138) | 0.9.0 docs still say that log compaction doesn't work on compressed topics. |  Major | . | James Cheng |  |
| [KAFKA-3134](https://issues.apache.org/jira/browse/KAFKA-3134) | Missing required configuration "value.deserializer" when initializing a KafkaConsumer with a valid "valueDeserializer" |  Major | . | Yifan Ying |  |
| [KAFKA-3132](https://issues.apache.org/jira/browse/KAFKA-3132) | URI scheme in "listeners" property should not be case-sensitive |  Minor | config | Jake Robb | Grant Henke |
| [KAFKA-3098](https://issues.apache.org/jira/browse/KAFKA-3098) | "partition.assignment.strategy" appears twice in documentation |  Major | . | Gwen Shapira | David Jacot |
| [KAFKA-3095](https://issues.apache.org/jira/browse/KAFKA-3095) | No documentation on format of sasl.kerberos.principal.to.local.rules |  Major | core | Thomas Graves | Thomas Graves |
| [KAFKA-3091](https://issues.apache.org/jira/browse/KAFKA-3091) | Broker with an invalid id would not start when its id is updated to a new valid one |  Minor | . | Vahid Hashemian | Grant Henke |
| [KAFKA-3088](https://issues.apache.org/jira/browse/KAFKA-3088) | 0.9.0.0 broker crash on receipt of produce request with empty client ID |  Major | producer | Dave Peterson | Grant Henke |
| [KAFKA-3085](https://issues.apache.org/jira/browse/KAFKA-3085) | BrokerChangeListener computes inconsistent live/dead broker list |  Major | core | Jun Rao | David Jacot |
| [KAFKA-3080](https://issues.apache.org/jira/browse/KAFKA-3080) | ConsoleConsumerTest.test\_version system test fails consistently |  Major | system tests | Ewen Cheslack-Postava |  |
| [KAFKA-3069](https://issues.apache.org/jira/browse/KAFKA-3069) | Fix recursion in ZkSecurityMigrator |  Major | security | Flavio Junqueira | Flavio Junqueira |
| [KAFKA-3068](https://issues.apache.org/jira/browse/KAFKA-3068) | NetworkClient may connect to a different Kafka cluster than originally configured |  Major | clients | Jun Rao | Eno Thereska |
| [KAFKA-3055](https://issues.apache.org/jira/browse/KAFKA-3055) | JsonConverter mangles schema during serialization (fromConnectData) |  Major | copycat | Kishore Senji | Ewen Cheslack-Postava |
| [KAFKA-3037](https://issues.apache.org/jira/browse/KAFKA-3037) | Number of alive brokers not known after single node cluster startup |  Minor | . | Stevo Slavic | Grant Henke |
| [KAFKA-3009](https://issues.apache.org/jira/browse/KAFKA-3009) | Disallow star imports |  Major | . | Gwen Shapira | Manasvi Gupta |
| [KAFKA-2999](https://issues.apache.org/jira/browse/KAFKA-2999) | Errors enum should be a 1 to 1 mapping of error codes and exceptions |  Major | . | Grant Henke | Grant Henke |
| [KAFKA-2990](https://issues.apache.org/jira/browse/KAFKA-2990) | NoSuchMethodError when Kafka is compiled with 1.8 and run on 1.7 |  Major | . | Jason Gustafson | Jason Gustafson |
| [KAFKA-2973](https://issues.apache.org/jira/browse/KAFKA-2973) | Fix leak of child sensors on remove |  Major | clients | Ismael Juma | Ismael Juma |
| [KAFKA-2965](https://issues.apache.org/jira/browse/KAFKA-2965) | Two variables should be exchanged. |  Minor | controller | Bo Wang |  |
| [KAFKA-2928](https://issues.apache.org/jira/browse/KAFKA-2928) | system tests: failures in version-related sanity checks |  Major | . | Geoff Anderson | Geoff Anderson |
| [KAFKA-2927](https://issues.apache.org/jira/browse/KAFKA-2927) | System tests: reduce storage footprint of collected logs |  Major | . | Geoff Anderson | Geoff Anderson |
| [KAFKA-2926](https://issues.apache.org/jira/browse/KAFKA-2926) | [MirrorMaker] InternalRebalancer calls wrong method of external rebalancer |  Major | tools | Gwen Shapira | Gwen Shapira |
| [KAFKA-2915](https://issues.apache.org/jira/browse/KAFKA-2915) | System Tests that use bootstrap.servers embedded in jinja files are not working |  Major | . | Ben Stopford |  |
| [KAFKA-2911](https://issues.apache.org/jira/browse/KAFKA-2911) | Replace Utils.sleep() with Time.sleep() whenever possible |  Major | . | Guozhang Wang | Jason Gustafson |
| [KAFKA-2906](https://issues.apache.org/jira/browse/KAFKA-2906) | Kafka Connect javadocs not built properly |  Major | copycat | Ewen Cheslack-Postava | Ewen Cheslack-Postava |
| [KAFKA-2902](https://issues.apache.org/jira/browse/KAFKA-2902) | StreamingConfig getConsumerConfiigs uses getRestoreConsumerConfigs instead of  getBaseConsumerConfigs |  Major | kafka streams | Bill Bejeck | Bill Bejeck |
| [KAFKA-2892](https://issues.apache.org/jira/browse/KAFKA-2892) | Consumer Docs Use Wrong Method |  Major | clients | Jesse Anderson |  |
| [KAFKA-2886](https://issues.apache.org/jira/browse/KAFKA-2886) | WorkerSinkTask doesn't catch exceptions from rebalance callbacks |  Major | copycat | Ewen Cheslack-Postava | Jason Gustafson |
| [KAFKA-2878](https://issues.apache.org/jira/browse/KAFKA-2878) | Kafka broker throws OutOfMemory exception with invalid join group request |  Critical | clients | Rajini Sivaram | Rajini Sivaram |
| [KAFKA-2874](https://issues.apache.org/jira/browse/KAFKA-2874) | zookeeper-server-stop.sh may fail to shutdown ZK and/or may stop unrelated processes |  Major | . | Michael Noll |  |
| [KAFKA-2872](https://issues.apache.org/jira/browse/KAFKA-2872) | Error starting KafkaStream caused by sink not being connected to parent source/processor nodes |  Major | kafka streams | Bill Bejeck | Bill Bejeck |
| [KAFKA-2862](https://issues.apache.org/jira/browse/KAFKA-2862) | Incorrect help description for MirrorMaker's message.handler.args |  Major | . | Ashish K Singh | Ashish K Singh |
| [KAFKA-2859](https://issues.apache.org/jira/browse/KAFKA-2859) | Deadlock in WorkerSourceTask |  Blocker | copycat | Ewen Cheslack-Postava | Ewen Cheslack-Postava |
| [KAFKA-2850](https://issues.apache.org/jira/browse/KAFKA-2850) | SslTransportLayerTest.testInvalidEndpointIdentification fails consistently |  Major | clients, security | Flavio Junqueira | Rajini Sivaram |
| [KAFKA-2826](https://issues.apache.org/jira/browse/KAFKA-2826) | Make Kafka Connect ducktape services easier to extend |  Minor | copycat | Ewen Cheslack-Postava | Ewen Cheslack-Postava |
| [KAFKA-2824](https://issues.apache.org/jira/browse/KAFKA-2824) | MiniKDC based tests don't run in VirtualBox |  Major | . | Ben Stopford | Ben Stopford |
| [KAFKA-2820](https://issues.apache.org/jira/browse/KAFKA-2820) | System tests: log level is no longer propagating from service classes |  Major | . | Geoff Anderson | Geoff Anderson |
| [KAFKA-2815](https://issues.apache.org/jira/browse/KAFKA-2815) | unit test failure in org.apache.kafka.streams.processor.internals.KafkaStreamingPartitionAssignorTest |  Major | . | Jun Rao | Grant Henke |
| [KAFKA-2814](https://issues.apache.org/jira/browse/KAFKA-2814) | Kafka Connect system tests using REST interface fail on AWS |  Major | copycat, system tests | Ewen Cheslack-Postava | Ewen Cheslack-Postava |
| [KAFKA-2803](https://issues.apache.org/jira/browse/KAFKA-2803) | Add hard bounce system test for distributed Kafka Connect |  Major | copycat | Ewen Cheslack-Postava | Ewen Cheslack-Postava |
| [KAFKA-2757](https://issues.apache.org/jira/browse/KAFKA-2757) | Consolidate BrokerEndPoint and EndPoint |  Major | . | Guozhang Wang | chen zhu |
| [KAFKA-2589](https://issues.apache.org/jira/browse/KAFKA-2589) | Documentation bug: the default value for the "rebalance.backoff.ms" property is not specified correctly |  Major | config | Bogdan Dimitriu | Grant Henke |
| [KAFKA-2578](https://issues.apache.org/jira/browse/KAFKA-2578) | Client Metadata internal state should be synchronized |  Trivial | . | Jason Gustafson | Edward Ribeiro |
| [KAFKA-2421](https://issues.apache.org/jira/browse/KAFKA-2421) | Upgrade LZ4 to version 1.3 to avoid crashing with IBM Java 7 |  Major | . | Rajini Sivaram | Grant Henke |
| [KAFKA-2399](https://issues.apache.org/jira/browse/KAFKA-2399) | Replace Stream.continually with Iterator.continually |  Minor | . | Ismael Juma | Ismael Juma |
| [KAFKA-2146](https://issues.apache.org/jira/browse/KAFKA-2146) | adding partition did not find the correct startIndex |  Minor | admin | chenshangan | chenshangan |
| [KAFKA-1860](https://issues.apache.org/jira/browse/KAFKA-1860) | File system errors are not detected unless Kafka tries to write |  Major | . | Guozhang Wang | Mayuresh Gharat |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3255](https://issues.apache.org/jira/browse/KAFKA-3255) | Extra unit tests for NetworkClient.connectionDelay(Node node, long now) |  Trivial | core | Frank Scholten |  |
| [KAFKA-3214](https://issues.apache.org/jira/browse/KAFKA-3214) | Add consumer system tests for compressed topics |  Major | consumer | Jason Gustafson | Anna Povzner |
| [KAFKA-2989](https://issues.apache.org/jira/browse/KAFKA-2989) | Verify all partitions consumed after rebalancing in system tests |  Major | . | Jason Gustafson | Jason Gustafson |
| [KAFKA-2979](https://issues.apache.org/jira/browse/KAFKA-2979) | Enable authorizer and ACLs in ducktape tests |  Major | system tests | Flavio Junqueira | Flavio Junqueira |
| [KAFKA-2949](https://issues.apache.org/jira/browse/KAFKA-2949) | Make EndToEndAuthorizationTest replicated |  Major | . | Flavio Junqueira | Flavio Junqueira |
| [KAFKA-2905](https://issues.apache.org/jira/browse/KAFKA-2905) | System test for rolling upgrade to enable ZooKeeper ACLs with SASL |  Major | . | Flavio Junqueira | Flavio Junqueira |
| [KAFKA-2846](https://issues.apache.org/jira/browse/KAFKA-2846) | Add Ducktape test for kafka-consumer-groups |  Major | . | Ashish K Singh | Ashish K Singh |
| [KAFKA-2825](https://issues.apache.org/jira/browse/KAFKA-2825) | Add controller failover to existing replication tests |  Major | . | Anna Povzner | Anna Povzner |
| [KAFKA-2732](https://issues.apache.org/jira/browse/KAFKA-2732) | Add test cases with ZK Auth, SASL and SSL |  Major | security | Flavio Junqueira | Flavio Junqueira |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-3289](https://issues.apache.org/jira/browse/KAFKA-3289) | Update Kafka protocol guide wiki for KIP-31 / KIP-32 |  Major | . | Jiangjie Qin | Jiangjie Qin |
| [KAFKA-3277](https://issues.apache.org/jira/browse/KAFKA-3277) | Update trunk version to be 0.10.0.0-SNAPSHOT |  Major | build | Ismael Juma | Ismael Juma |
| [KAFKA-3276](https://issues.apache.org/jira/browse/KAFKA-3276) | Rename 0.10.0.0 to 0.10.1.0 and 0.9.1.0 to 0.10.0.0 in JIRA |  Major | . | Ismael Juma | Ewen Cheslack-Postava |
| [KAFKA-3245](https://issues.apache.org/jira/browse/KAFKA-3245) | need a way to specify the number of replicas for change log topics |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-3192](https://issues.apache.org/jira/browse/KAFKA-3192) | Add implicit unlimited windowed aggregation for KStream |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3165](https://issues.apache.org/jira/browse/KAFKA-3165) | Fix ignored parameters in the gradle "All" tasks |  Major | build | Grant Henke | Grant Henke |
| [KAFKA-3142](https://issues.apache.org/jira/browse/KAFKA-3142) | Improve error message in kstreams |  Major | . | Jay Kreps | Guozhang Wang |
| [KAFKA-3136](https://issues.apache.org/jira/browse/KAFKA-3136) | Rename KafkaStreaming to KafkaStreams |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3133](https://issues.apache.org/jira/browse/KAFKA-3133) | Add putIfAbsent function to KeyValueStore |  Major | . | Guozhang Wang | Kim Christensen |
| [KAFKA-3125](https://issues.apache.org/jira/browse/KAFKA-3125) | Exception Hierarchy for Streams |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3121](https://issues.apache.org/jira/browse/KAFKA-3121) | KStream DSL API Improvement |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3108](https://issues.apache.org/jira/browse/KAFKA-3108) | KStream custom StreamPartitioner for windowed key |  Minor | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-3104](https://issues.apache.org/jira/browse/KAFKA-3104) | Windowed Stream Aggregation Implementation |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3081](https://issues.apache.org/jira/browse/KAFKA-3081) | KTable Aggregation Implementation |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3078](https://issues.apache.org/jira/browse/KAFKA-3078) | Add ducktape tests for KafkaLog4jAppender producing to SASL enabled Kafka cluster |  Major | clients | Ashish K Singh | Ashish K Singh |
| [KAFKA-3066](https://issues.apache.org/jira/browse/KAFKA-3066) | Add Demo Examples for Kafka Streams |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-3063](https://issues.apache.org/jira/browse/KAFKA-3063) | LogRecoveryTest exits with -1 occasionally |  Major | . | Guozhang Wang | Ismael Juma |
| [KAFKA-3060](https://issues.apache.org/jira/browse/KAFKA-3060) | Refactor MeteredXXStore |  Minor | kafka streams | Yasuhiro Matsuda | Guozhang Wang |
| [KAFKA-3036](https://issues.apache.org/jira/browse/KAFKA-3036) | Add up-conversion and down-conversion of ProducerRequest and FetchRequest to broker. |  Major | . | Jiangjie Qin | Jiangjie Qin |
| [KAFKA-3030](https://issues.apache.org/jira/browse/KAFKA-3030) | Remove unused scala dependencies |  Major | build | Grant Henke | Grant Henke |
| [KAFKA-3026](https://issues.apache.org/jira/browse/KAFKA-3026) | KIP-32 (part 2): Changes in broker to over-write timestamp or reject message |  Major | . | Anna Povzner | Jiangjie Qin |
| [KAFKA-3025](https://issues.apache.org/jira/browse/KAFKA-3025) | KIP-31&KIP-32 (part 1): Add timestamp field to message, configs, and Producer/ConsumerRecord |  Major | . | Anna Povzner | Jiangjie Qin |
| [KAFKA-3022](https://issues.apache.org/jira/browse/KAFKA-3022) | Deduplicate common project configurations |  Major | build | Grant Henke | Grant Henke |
| [KAFKA-3021](https://issues.apache.org/jira/browse/KAFKA-3021) | Centralize dependency version managment |  Major | build | Grant Henke | Grant Henke |
| [KAFKA-3020](https://issues.apache.org/jira/browse/KAFKA-3020) | Ensure Checkstyle runs on all Java code |  Major | build | Grant Henke | Grant Henke |
| [KAFKA-3016](https://issues.apache.org/jira/browse/KAFKA-3016) | Add KStream-KStream window joins |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2984](https://issues.apache.org/jira/browse/KAFKA-2984) | KTable should send old values along with new values to downstreams |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2962](https://issues.apache.org/jira/browse/KAFKA-2962) | Add Simple Join API |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2856](https://issues.apache.org/jira/browse/KAFKA-2856) | add KTable |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2837](https://issues.apache.org/jira/browse/KAFKA-2837) | FAILING TEST: kafka.api.ProducerBounceTest \> testBrokerFailure |  Major | . | Gwen Shapira | jin xing |
| [KAFKA-2811](https://issues.apache.org/jira/browse/KAFKA-2811) | Add standby tasks |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2804](https://issues.apache.org/jira/browse/KAFKA-2804) | Create / Update changelog topics upon state store initialization |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-2802](https://issues.apache.org/jira/browse/KAFKA-2802) | Add integration tests for Kafka Streams |  Major | . | Guozhang Wang | Yasuhiro Matsuda |
| [KAFKA-2763](https://issues.apache.org/jira/browse/KAFKA-2763) | Reduce stream task migrations and initialization costs |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2733](https://issues.apache.org/jira/browse/KAFKA-2733) | Distinguish metric names inside the sensor registry |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-2727](https://issues.apache.org/jira/browse/KAFKA-2727) | initialize only the part of the topology relevant to the task |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2718](https://issues.apache.org/jira/browse/KAFKA-2718) | Reuse of temporary directories leading to transient unit test failures |  Major | core | Rajini Sivaram | Rajini Sivaram |
| [KAFKA-2707](https://issues.apache.org/jira/browse/KAFKA-2707) | Make KStream processor names deterministic |  Major | . | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2706](https://issues.apache.org/jira/browse/KAFKA-2706) | Make state stores first class citizens in the processor DAG |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2698](https://issues.apache.org/jira/browse/KAFKA-2698) | add paused API |  Critical | consumer | Onur Karaman | Jason Gustafson |
| [KAFKA-2694](https://issues.apache.org/jira/browse/KAFKA-2694) | Make a task id be a composite id of a topic group id and a partition id |  Major | kafka streams | Yasuhiro Matsuda | Yasuhiro Matsuda |
| [KAFKA-2667](https://issues.apache.org/jira/browse/KAFKA-2667) | Copycat KafkaBasedLogTest.testSendAndReadToEnd transient failure |  Major | copycat | Jason Gustafson | Ewen Cheslack-Postava |
| [KAFKA-2654](https://issues.apache.org/jira/browse/KAFKA-2654) | Avoid calling Consumer.poll(0) in each iteration |  Major | . | Guozhang Wang | Yasuhiro Matsuda |
| [KAFKA-2653](https://issues.apache.org/jira/browse/KAFKA-2653) | Stateful operations in the KStream DSL layer |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-2652](https://issues.apache.org/jira/browse/KAFKA-2652) | Incorporate the new consumer protocol with partition-group interface |  Major | . | Guozhang Wang | Yasuhiro Matsuda |
| [KAFKA-2649](https://issues.apache.org/jira/browse/KAFKA-2649) | Add support for custom partitioner in sink nodes |  Major | kafka streams | Randall Hauch | Randall Hauch |
| [KAFKA-2643](https://issues.apache.org/jira/browse/KAFKA-2643) | Run mirror maker tests in ducktape with SSL and SASL |  Major | . | Rajini Sivaram | Rajini Sivaram |
| [KAFKA-2642](https://issues.apache.org/jira/browse/KAFKA-2642) | Run replication tests in ducktape with SSL for clients |  Major | . | Rajini Sivaram | Rajini Sivaram |
| [KAFKA-2600](https://issues.apache.org/jira/browse/KAFKA-2600) | Make KStream interfaces compatible with Java 8 java.util.function |  Major | . | Guozhang Wang | Randall Hauch |
| [KAFKA-2594](https://issues.apache.org/jira/browse/KAFKA-2594) | Add a key-value store that is a fixed-capacity in-memory LRU cache |  Major | kafka streams | Randall Hauch | Randall Hauch |
| [KAFKA-2593](https://issues.apache.org/jira/browse/KAFKA-2593) | KeyValueStores should not require use of the context's default serializers and deserializers |  Major | kafka streams | Randall Hauch | Randall Hauch |
| [KAFKA-2591](https://issues.apache.org/jira/browse/KAFKA-2591) | Remove Persistent Data before Restoringafter a Fault |  Major | . | Guozhang Wang | Guozhang Wang |
| [KAFKA-2509](https://issues.apache.org/jira/browse/KAFKA-2509) | Replace LeaderAndIsr{Request,Response} with org.apache.kafka.common.network.requests equivalent |  Major | . | Ismael Juma | Grant Henke |
| [KAFKA-2508](https://issues.apache.org/jira/browse/KAFKA-2508) | Replace UpdateMetadata{Request,Response} with org.apache.kafka.common.requests equivalent |  Major | . | Ismael Juma | Grant Henke |
| [KAFKA-2422](https://issues.apache.org/jira/browse/KAFKA-2422) | Allow copycat connector plugins to be aliased to simpler names |  Minor | copycat | Ewen Cheslack-Postava | Gwen Shapira |
| [KAFKA-2072](https://issues.apache.org/jira/browse/KAFKA-2072) | Add StopReplica request/response to o.a.k.common.requests and replace the usage in core module |  Major | . | Gwen Shapira | David Jacot |
| [KAFKA-2071](https://issues.apache.org/jira/browse/KAFKA-2071) | Replace Produce Request/Response with their org.apache.kafka.common.requests equivalents |  Major | . | Gwen Shapira | David Jacot |
| [KAFKA-2070](https://issues.apache.org/jira/browse/KAFKA-2070) | Replace OffsetRequest/response with ListOffsetRequest/response from org.apache.kafka.common.requests |  Major | . | Gwen Shapira | Grant Henke |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [KAFKA-2896](https://issues.apache.org/jira/browse/KAFKA-2896) | System test for partition re-assignment |  Major | . | Gwen Shapira | Anna Povzner |
| [KAFKA-2845](https://issues.apache.org/jira/browse/KAFKA-2845) | Add 0.9 clients vs 0.8 brokers compatibility test |  Major | . | Geoff Anderson | Geoff Anderson |
| [KAFKA-2830](https://issues.apache.org/jira/browse/KAFKA-2830) | Change default fix version to 0.9.1.0 in kafka-merge-pr.py |  Major | build | Ismael Juma | Ismael Juma |


