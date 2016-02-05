
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
# Apache Flink  1.0.0 Release Notes

These release notes cover new developer and user-facing incompatibilities, important issues, features, and major improvements.


---

* [FLINK-3292](https://issues.apache.org/jira/browse/FLINK-3292) | *Minor* | **Bug in flink-jdbc. Not all JDBC drivers supported**

Hello,

In method open in JDBCInputFormat.java, while using dbConn.createStatement, the resultSetType & resultSetConcurrency are hardcoded. 
These two fields may vary with different JDBC drivers & hence it fails in a few cases like SAP HANA Jdbc driver. 
There are two variants of the method dbCon.createStatement, one with parameters & the other without  parameters. Both should be supported. 

Thanks & regards,
Subhobrata



