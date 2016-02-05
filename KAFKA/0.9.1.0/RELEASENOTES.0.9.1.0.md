
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
# Apache Kafka  0.9.1.0 Release Notes

These release notes cover new developer and user-facing incompatibilities, important issues, features, and major improvements.


---

* [KAFKA-3044](https://issues.apache.org/jira/browse/KAFKA-3044) | *Major* | **Consumer.poll doesnot return messages when poll interval is less**

When seeking to particular position in consumer and starting poll with timeout param 0 the consumer does not come back with data though there is data published via a producer already. If the timeout is increased slowly in chunks of 100ms then at 700ms value the consumer returns back the record on first call to poll.

Docs [http://kafka.apache.org/090/javadoc/org/apache/kafka/clients/consumer/KafkaConsumer.html#poll(long)] for poll reads if timeout is 0 then data will be returned immediately but the behaviour seen is that data is not returned.

The test code I am using can be found here https://gist.github.com/praveend/013dcab01ebb8c7e2f2d

I have created a topic with data published as below and then running the test program [ConsumerPollTest.java]

$ bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic mytopic
$ bin/kafka-console-producer.sh --broker-list localhost:9092 --topic mytopic
Hello
Hai
bye
$ java ConsumerPollTest

I have published this 3 lines of data to kafka only once....later on I just use the above program with different poll interval

Let me know if I am missing anything and interpreting it wrongly.


---

* [KAFKA-3029](https://issues.apache.org/jira/browse/KAFKA-3029) | *Major* | **Make class org.apache.kafka.common.TopicPartition Serializable**

The client class TopicPartition is exposed and used by consumer applications directly. In case where the application needs to checkpoint the state it is difficult to serialize different app classes that use TopicPartition as TopicParitition is not serializable.

For instance consider the Spark use case where RDDs have to be checkpointed....the KafakaInputDstream (which we are currently modifying to use the new Kafka API rather than the Highlevel apis in previous version) cannot be serialized due to above limitation.

I have created a patch to serialize TopicPartition class by making it implement serializable interface and have issued a pull request.

Can this be merged for the next release (0.9.0.1)

Thanks

Praveen



