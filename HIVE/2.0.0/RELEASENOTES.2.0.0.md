
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
# Apache Hive  2.0.0 Release Notes

These release notes cover new developer and user-facing incompatibilities, features, and major improvements.


---

* [HIVE-11228](https://issues.apache.org/jira/browse/HIVE-11228) | *Major* | **Mutation API should use semi-shared locks.**

Streaming mutation API uses semi-shared locks.


---

* [HIVE-11215](https://issues.apache.org/jira/browse/HIVE-11215) | *Minor* | **Vectorized grace hash-join throws FileUtil warnings**

 HIVE-11215: Delete spills only if they exist (Gopal V, reviewed by Matt Mccline)


---

* [HIVE-11145](https://issues.apache.org/jira/browse/HIVE-11145) | *Major* | **Remove OFFLINE and NO\_DROP from tables and partitions**

OFFLINE and NO\_DROP mode for partitions removed, use SQLStandardAuth or other authorization scheme to prevent partitions from being dropped or read.


---

* [HIVE-11073](https://issues.apache.org/jira/browse/HIVE-11073) | *Minor* | **ORC FileDump utility ignores errors when writing output**

orcfiledump exits if errors are detected when writing to stdout.


---

* [HIVE-11055](https://issues.apache.org/jira/browse/HIVE-11055) | *Major* | **HPL/SQL - Implementing Procedural SQL in Hive (PL/HQL Contribution)**

Adds procedural SQL to Hive


---

* [HIVE-11054](https://issues.apache.org/jira/browse/HIVE-11054) | *Major* | **Read error : Partition Varchar column cannot be cast to string**

HIVE-11054: Handle varchar/char partition columns in vectorization


---

* [HIVE-11051](https://issues.apache.org/jira/browse/HIVE-11051) | *Critical* | **Hive 1.2.0  MapJoin w/Tez - LazyBinaryArray cannot be cast to [Ljava.lang.Object;**

HIVE-11051: Hive 1.2.0 MapJoin w/Tez - LazyBinaryArray cannot be cast to [Ljava.lang.Object; (Matt McCline via Gopal V)


---

* [HIVE-11043](https://issues.apache.org/jira/browse/HIVE-11043) | *Major* | **ORC split strategies should adapt based on number of files**

Use ETLStrategy for a small number of ORC files.


---

* [HIVE-10974](https://issues.apache.org/jira/browse/HIVE-10974) | *Major* | **Use Configuration::getRaw() for the Base64 data**

Use Configuration::getRaw() to read Base64 data out of Configuration objects


---

* [HIVE-10746](https://issues.apache.org/jira/browse/HIVE-10746) | *Critical* | ** Hive 1.2.0+Tez produces 1-byte FileSplits from mapred.TextInputFormat**

Use sane split min-sizes when using legacy mapred.InputFormat::getSplits(job, num)


---

* [HIVE-10707](https://issues.apache.org/jira/browse/HIVE-10707) | *Trivial* | **CBO: debug logging OOMs**

CBO: dump AST only when in DEBUG mode.


---

* [HIVE-10509](https://issues.apache.org/jira/browse/HIVE-10509) | *Major* | **Bump trunk version to 1.3 as branch-1.2 has been created.**

Hive master/trunk version bumped up to 1.3


---

* [HIVE-10191](https://issues.apache.org/jira/browse/HIVE-10191) | *Major* | **ORC: Cleanup writer per-row synchronization**

Remove per-row synchronization from ORC WriterImpl


---

* [HIVE-10165](https://issues.apache.org/jira/browse/HIVE-10165) | *Major* | **Improve hive-hcatalog-streaming extensibility and support updates and deletes.**

Expanded streaming API to include update and delete operations and support merge type processes.


---

* [HIVE-9365](https://issues.apache.org/jira/browse/HIVE-9365) | *Minor* | **The Metastore should take port configuration from hive-site.xml**

**WARNING: No release note provided for this incompatible change.**


---

* [HIVE-6026](https://issues.apache.org/jira/browse/HIVE-6026) | *Minor* | **Ldap Authenticator should be more generic with BindDN**

Hive LDAP Authenticator now has filter support for LDAP users and groups.


