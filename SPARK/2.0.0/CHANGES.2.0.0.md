
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
# Apache Spark Changelog

## Release 2.0.0 - Unreleased (as of 2016-02-24)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13195](https://issues.apache.org/jira/browse/SPARK-13195) | PairDStreamFunctions.mapWithState fails in case timeout is set without updating State[S] |  Major | Streaming | Yuval Itzchakov | Shixiong Zhu |
| [SPARK-12016](https://issues.apache.org/jira/browse/SPARK-12016) | word2vec load model can't use findSynonyms to get words |  Major | PySpark | yuangang.liu | Liang-Chi Hsieh |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13373](https://issues.apache.org/jira/browse/SPARK-13373) | Generate code for sort merge join |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13075](https://issues.apache.org/jira/browse/SPARK-13075) | Native database/table system catalog |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13074](https://issues.apache.org/jira/browse/SPARK-13074) | Add getPersistentRDDs() API to JavaSparkContext |  Minor | Spark Core | Junyang Shen | Junyang Shen |
| [SPARK-13011](https://issues.apache.org/jira/browse/SPARK-13011) | K-means wrapper in SparkR |  Major | ML, SparkR | Xiangrui Meng | Xusen Yin |
| [SPARK-12828](https://issues.apache.org/jira/browse/SPARK-12828) | support natural join |  Major | SQL | Adrian Wang | Adrian Wang |
| [SPARK-12818](https://issues.apache.org/jira/browse/SPARK-12818) | Implement Bloom filter and count-min sketch in DataFrames |  Major | SQL | Reynold Xin | Cheng Lian |
| [SPARK-12798](https://issues.apache.org/jira/browse/SPARK-12798) | Broadcast hash join |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12797](https://issues.apache.org/jira/browse/SPARK-12797) | Aggregation without grouping keys |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12796](https://issues.apache.org/jira/browse/SPARK-12796) | initial prototype: projection/filter/range |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12785](https://issues.apache.org/jira/browse/SPARK-12785) | Implement columnar in memory representation |  Major | SQL | Nong Li | Nong Li |
| [SPARK-12544](https://issues.apache.org/jira/browse/SPARK-12544) | Support window functions in SQLContext |  Major | SQL | Davies Liu | Herman van Hovell |
| [SPARK-12542](https://issues.apache.org/jira/browse/SPARK-12542) | Support intersect/except in Hive SQL |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12541](https://issues.apache.org/jira/browse/SPARK-12541) | Support rollup/cube in SQL query |  Major | SQL | Davies Liu | Apache Spark |
| [SPARK-12538](https://issues.apache.org/jira/browse/SPARK-12538) | bucketed table support |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12401](https://issues.apache.org/jira/browse/SPARK-12401) | Add support for enums in postgres |  Minor | SQL | Jaka Jancar | Takeshi Yamamuro |
| [SPARK-12394](https://issues.apache.org/jira/browse/SPARK-12394) | Support writing out pre-hash-partitioned data and exploit that in join optimizations to avoid shuffle (i.e. bucketing in Hive) |  Major | SQL | Reynold Xin | Nong Li |
| [SPARK-12337](https://issues.apache.org/jira/browse/SPARK-12337) | Implement dropDuplicates() method of DataFrame in SparkR |  Major | SparkR | Sun Rui | Sun Rui |
| [SPARK-12321](https://issues.apache.org/jira/browse/SPARK-12321) | JSON format for logical/physical execution plans |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12204](https://issues.apache.org/jira/browse/SPARK-12204) | Implement drop method for DataFrame in SparkR |  Major | SparkR | Sun Rui | Sun Rui |
| [SPARK-11774](https://issues.apache.org/jira/browse/SPARK-11774) | Implement "struct", "encode","decode" in SparkR |  Major | SparkR | Sun Rui | Sun Rui |
| [SPARK-11713](https://issues.apache.org/jira/browse/SPARK-11713) | Initial RDD for updateStateByKey for pyspark |  Major | PySpark | David Watson | Bryan Cutler |
| [SPARK-11515](https://issues.apache.org/jira/browse/SPARK-11515) | QuantileDiscretizer should take random seed |  Minor | ML | Joseph K. Bradley | Yu Ishikawa |
| [SPARK-11206](https://issues.apache.org/jira/browse/SPARK-11206) | Support SQL UI on the history server |  Major | SQL, Web UI | Carson Wang | Carson Wang |
| [SPARK-10809](https://issues.apache.org/jira/browse/SPARK-10809) | Single-document topicDistributions method for LocalLDAModel |  Minor | MLlib | Joseph K. Bradley | yuhao yang |
| [SPARK-10359](https://issues.apache.org/jira/browse/SPARK-10359) | Enumerate Spark's dependencies in a file and diff against it for new pull requests |  Major | Build, Project Infra | Patrick Wendell | Josh Rosen |
| [SPARK-9843](https://issues.apache.org/jira/browse/SPARK-9843) | Catalyst: Allow adding custom optimizers |  Major | SQL | Robert Kruszewski | Robert Kruszewski |
| [SPARK-9835](https://issues.apache.org/jira/browse/SPARK-9835) | Iteratively reweighted least squares solver for GLMs |  Critical | ML, MLlib | Xiangrui Meng | Yanbo Liang |
| [SPARK-9516](https://issues.apache.org/jira/browse/SPARK-9516) | Improve Thread Dump page |  Minor | Web UI | Nan Zhu | Nan Zhu |
| [SPARK-6990](https://issues.apache.org/jira/browse/SPARK-6990) | Add Java linting script |  Minor | Project Infra | Josh Rosen | Dmitry Erastov |
| [SPARK-6519](https://issues.apache.org/jira/browse/SPARK-6519) | Add spark.ml API for bisecting k-means |  Major | ML | Yu Ishikawa | Yu Ishikawa |
| [SPARK-3611](https://issues.apache.org/jira/browse/SPARK-3611) | Show number of cores for each executor in application web UI |  Minor | Web UI | Matei Zaharia | Alex Bozarth |
| [SPARK-2750](https://issues.apache.org/jira/browse/SPARK-2750) | Add Https support for Web UI |  Major | Web UI | Tao Wang | Fei Wang |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13429](https://issues.apache.org/jira/browse/SPARK-13429) | Unify Logistic Regression convergence tolerance of ML & MLlib |  Minor | ML, MLlib | Yanbo Liang | Yanbo Liang |
| [SPARK-13422](https://issues.apache.org/jira/browse/SPARK-13422) | Use HashedRelation instead of HashSet in Left Semi Joins |  Minor | SQL | Herman van Hovell | Xiu (Joe) Guo |
| [SPARK-13416](https://issues.apache.org/jira/browse/SPARK-13416) | Add positive check for option 'numIter' in StronglyConnectedComponents |  Trivial | GraphX | zhengruifeng | zhengruifeng |
| [SPARK-13414](https://issues.apache.org/jira/browse/SPARK-13414) | Add support for launching multiple Mesos dispatchers |  Major | Mesos | Timothy Chen | Timothy Chen |
| [SPARK-13399](https://issues.apache.org/jira/browse/SPARK-13399) | Investigate type erasure warnings in CheckpointSuite |  Trivial | Tests | holdenk | holdenk |
| [SPARK-13386](https://issues.apache.org/jira/browse/SPARK-13386) | ConnectedComponents should support maxIteration option |  Minor | GraphX | zhengruifeng | zhengruifeng |
| [SPARK-13376](https://issues.apache.org/jira/browse/SPARK-13376) | Improve column pruning |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13364](https://issues.apache.org/jira/browse/SPARK-13364) | history server application column Id not sorting as number |  Minor | Web UI | Thomas Graves | Zhuo Liu |
| [SPARK-13357](https://issues.apache.org/jira/browse/SPARK-13357) | Use generated projection and ordering for TakeOrderedAndProjectNode |  Major | SQL | Takuya Ueshin | Takuya Ueshin |
| [SPARK-13339](https://issues.apache.org/jira/browse/SPARK-13339) | Clarify commutative / associative operator requirements for reduce, fold |  Minor | Documentation | Sean Owen | Sean Owen |
| [SPARK-13329](https://issues.apache.org/jira/browse/SPARK-13329) | Considering output for statistics of logical plan |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13324](https://issues.apache.org/jira/browse/SPARK-13324) | Update plugin, test, example dependencies for 2.x |  Minor | Build, Examples, Spark Core | Sean Owen | Sean Owen |
| [SPARK-13295](https://issues.apache.org/jira/browse/SPARK-13295) | ML/MLLIB: AFTSurvivalRegression: Improve AFTAggregator - Avoid creating new instances of arrays/vectors for each record |  Major | ML, MLlib | Narine Kokhlikyan | Narine Kokhlikyan |
| [SPARK-13293](https://issues.apache.org/jira/browse/SPARK-13293) | Generate code for Expand |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13280](https://issues.apache.org/jira/browse/SPARK-13280) | FileBasedWriteAheadLog logger name should be under o.a.s namespace |  Minor | Streaming | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-13279](https://issues.apache.org/jira/browse/SPARK-13279) | Scheduler does O(N^2) operation when adding a new task set (making it prohibitively slow for scheduling 200K tasks) |  Major | Scheduler, Spark Core | Sital Kedia | Sital Kedia |
| [SPARK-13271](https://issues.apache.org/jira/browse/SPARK-13271) | Better error message if 'path' is not specified |  Major | SQL | Shixiong Zhu | Shixiong Zhu |
| [SPARK-13264](https://issues.apache.org/jira/browse/SPARK-13264) | Remove multi-byte character in spark-env.sh.template |  Trivial | Spark Core | Sasaki Toru | Sasaki Toru |
| [SPARK-13257](https://issues.apache.org/jira/browse/SPARK-13257) | Refine naive Bayes example code |  Minor | Examples | Lenjoy Lin | Lenjoy Lin |
| [SPARK-13248](https://issues.apache.org/jira/browse/SPARK-13248) | Remove depecrated Streaming APIs |  Minor | Streaming | Luciano Resende | Luciano Resende |
| [SPARK-13237](https://issues.apache.org/jira/browse/SPARK-13237) | Generate broadcast outer join |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13235](https://issues.apache.org/jira/browse/SPARK-13235) | Remove an Extra Distinct in Union |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-13234](https://issues.apache.org/jira/browse/SPARK-13234) | Remove duplicated SQL metrics |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13215](https://issues.apache.org/jira/browse/SPARK-13215) | Remove fallback in codegen |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13203](https://issues.apache.org/jira/browse/SPARK-13203) | Add scalastyle rule banning use of mutable.SynchronizedBuffer |  Trivial | Build | Ted Yu | Ted Yu |
| [SPARK-13189](https://issues.apache.org/jira/browse/SPARK-13189) | Cleanup build references to Scala 2.10 |  Minor | Build | Luciano Resende | Luciano Resende |
| [SPARK-13185](https://issues.apache.org/jira/browse/SPARK-13185) | Improve the performance of DateTimeUtils.StringToDate by reusing Calendar objects |  Minor | SQL | Carson Wang | Carson Wang |
| [SPARK-13168](https://issues.apache.org/jira/browse/SPARK-13168) | Collapse adjacent Repartition operations |  Major | SQL | Josh Rosen | Josh Rosen |
| [SPARK-13154](https://issues.apache.org/jira/browse/SPARK-13154) | Add pydoc lint for docs |  Trivial | PySpark | holdenk | holdenk |
| [SPARK-13152](https://issues.apache.org/jira/browse/SPARK-13152) | Fix task metrics deprecation warning |  Minor | Spark Core | holdenk | holdenk |
| [SPARK-13147](https://issues.apache.org/jira/browse/SPARK-13147) | improve readability of generated code |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13138](https://issues.apache.org/jira/browse/SPARK-13138) | Add "logical" package prefix for ddl.scala |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13136](https://issues.apache.org/jira/browse/SPARK-13136) | Data exchange (shuffle, broadcast) should only be handled by the exchange operator |  Major | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-13132](https://issues.apache.org/jira/browse/SPARK-13132) | LogisticRegression spends 35% of its time fetching the standardization parameter |  Minor | ML | Gary King | Gary King |
| [SPARK-13131](https://issues.apache.org/jira/browse/SPARK-13131) | Use best  time and average time in micro benchmark |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13130](https://issues.apache.org/jira/browse/SPARK-13130) | Make whole stage codegen variable names slightly easier to read |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13113](https://issues.apache.org/jira/browse/SPARK-13113) | Remove unnecessary bit operation when decoding page number |  Minor | Spark Core | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-13100](https://issues.apache.org/jira/browse/SPARK-13100) | improving the performance of stringToDate method in DateTimeUtils.scala |  Minor | SQL | Yang Wang | Yang Wang |
| [SPARK-13098](https://issues.apache.org/jira/browse/SPARK-13098) | remove GenericInternalRowWithSchema |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-13097](https://issues.apache.org/jira/browse/SPARK-13097) | Extend Binarizer to allow Double AND Vector inputs |  Minor | ML | Mike Seddon | Mike Seddon |
| [SPARK-13094](https://issues.apache.org/jira/browse/SPARK-13094) | No encoder implicits for Seq[Primitive] |  Major | SQL | Deenar Toraskar | Michael Armbrust |
| [SPARK-13093](https://issues.apache.org/jira/browse/SPARK-13093) | improve null check in nullSafeCodeGen for unary, binary and ternary expression |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-13086](https://issues.apache.org/jira/browse/SPARK-13086) | Spark Shell for 2.11 does not allow loading files via '-i' |  Minor | Spark Shell | Iulian Dragos | Iulian Dragos |
| [SPARK-13072](https://issues.apache.org/jira/browse/SPARK-13072) | simplify and improve murmur3 hash expression codegen |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-13070](https://issues.apache.org/jira/browse/SPARK-13070) | Points out which physical file is the trouble maker when Parquet schema merging fails |  Minor | SQL | Cheng Lian | Cheng Lian |
| [SPARK-13057](https://issues.apache.org/jira/browse/SPARK-13057) | Add benchmark codes and the performance results for implemented compression schemes for InMemoryRelation |  Major | SQL | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-13031](https://issues.apache.org/jira/browse/SPARK-13031) | Improve test coverage for whole stage codegen |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13020](https://issues.apache.org/jira/browse/SPARK-13020) | fix random generator for map type |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12992](https://issues.apache.org/jira/browse/SPARK-12992) | Vectorize parquet decoding using ColumnarBatch |  Major | SQL | Nong Li | Apache Spark |
| [SPARK-12976](https://issues.apache.org/jira/browse/SPARK-12976) | Add LazilyGenerateOrdering and use it for RangePartitioner of Exchange. |  Major | SQL | Takuya Ueshin | Takuya Ueshin |
| [SPARK-12975](https://issues.apache.org/jira/browse/SPARK-12975) | Throwing Exception when Bucketing Columns are part of Partitioning Columns |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-12974](https://issues.apache.org/jira/browse/SPARK-12974) | Add Python API for spark.ml bisecting k-means |  Minor | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-12967](https://issues.apache.org/jira/browse/SPARK-12967) | NettyRPC races with SparkContext.stop() and throws exception |  Minor | Spark Core | Nishkam Ravi | Nishkam Ravi |
| [SPARK-12962](https://issues.apache.org/jira/browse/SPARK-12962) | PySpark support covar\_samp and covar\_pop |  Minor | PySpark, SQL | Yanbo Liang | Yanbo Liang |
| [SPARK-12953](https://issues.apache.org/jira/browse/SPARK-12953) | RDDRelation write set mode will be better to avoid error "pair.parquet already exists" |  Minor | Examples | shijinkui | shijinkui |
| [SPARK-12951](https://issues.apache.org/jira/browse/SPARK-12951) | Support spilling in generate aggregate |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12950](https://issues.apache.org/jira/browse/SPARK-12950) | Improve performance of BytesToBytesMap |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12932](https://issues.apache.org/jira/browse/SPARK-12932) | Bad error message with trying to create Dataset from RDD of Java objects that are not bean-compliant |  Trivial | Java API | Andy Grove | Andy Grove |
| [SPARK-12926](https://issues.apache.org/jira/browse/SPARK-12926) | SQLContext to display warning message when non-sql configs are being set |  Trivial | SQL | Tejas Patil | Tejas Patil |
| [SPARK-12925](https://issues.apache.org/jira/browse/SPARK-12925) | Improve HiveInspectors.unwrap for StringObjectInspector.getPrimitiveWritableObject |  Major | SQL | Rajesh Balamohan | Rajesh Balamohan |
| [SPARK-12915](https://issues.apache.org/jira/browse/SPARK-12915) | SQL metrics for generated operators |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12914](https://issues.apache.org/jira/browse/SPARK-12914) | Generate TungstenAggregate with grouping keys |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12913](https://issues.apache.org/jira/browse/SPARK-12913) | Reimplement stat functions as declarative function |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12912](https://issues.apache.org/jira/browse/SPARK-12912) | Add test suite for EliminateSubQueries |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12910](https://issues.apache.org/jira/browse/SPARK-12910) | Support for specifying version of R to use while creating sparkR libraries |  Minor | SparkR | Shubhanshu Mishra | Shubhanshu Mishra |
| [SPARK-12908](https://issues.apache.org/jira/browse/SPARK-12908) | Add tests to make sure that ml.classification.LogisticRegression returns meaningful result when labels are the same without intercept |  Major | ML | DB Tsai | DB Tsai |
| [SPARK-12905](https://issues.apache.org/jira/browse/SPARK-12905) | PCAModel return eigenvalues for PySpark |  Minor | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-12903](https://issues.apache.org/jira/browse/SPARK-12903) | Add covar\_samp and covar\_pop for SparkR |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12902](https://issues.apache.org/jira/browse/SPARK-12902) | Visualization and metrics for generated operators |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12898](https://issues.apache.org/jira/browse/SPARK-12898) | Consider having dummyCallSite for HiveTableScan |  Major | SQL | Rajesh Balamohan | Rajesh Balamohan |
| [SPARK-12888](https://issues.apache.org/jira/browse/SPARK-12888) | benchmark the new hash expression |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12882](https://issues.apache.org/jira/browse/SPARK-12882) | simplify bucket tests and add more comments |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12879](https://issues.apache.org/jira/browse/SPARK-12879) | improve unsafe row writing framework |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12873](https://issues.apache.org/jira/browse/SPARK-12873) | Add more comment in HiveTypeCoercion for type widening |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12872](https://issues.apache.org/jira/browse/SPARK-12872) | Support to specify the option for compression codec for JSON datasource. |  Minor | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12860](https://issues.apache.org/jira/browse/SPARK-12860) | speed up safe projection for primitive types |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12856](https://issues.apache.org/jira/browse/SPARK-12856) | speed up hashCode of unsafe array |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12840](https://issues.apache.org/jira/browse/SPARK-12840) | Support passing arbitrary objects (not just expressions) into code generated classes |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12834](https://issues.apache.org/jira/browse/SPARK-12834) | Use type conversion instead of Ser/De of Pickle to transform JavaArray and JavaList |  Major | PySpark | Xusen Yin | Xusen Yin |
| [SPARK-12788](https://issues.apache.org/jira/browse/SPARK-12788) | Simplify BooleanEquality by using casts |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12761](https://issues.apache.org/jira/browse/SPARK-12761) | Clean up duplicated code in scala 2.11 repl.Main |  Trivial | Spark Shell | Jakob Odersky | Jakob Odersky |
| [SPARK-12759](https://issues.apache.org/jira/browse/SPARK-12759) | Spark should fail fast if --executor-memory is too small for spark to start |  Trivial | Spark Shell | Imran Rashid | Daniel Jalova |
| [SPARK-12749](https://issues.apache.org/jira/browse/SPARK-12749) | Spark SQL JSON schema infernce should allow floating-point numbers as BigDecimal |  Minor | SQL | Brandon Bradley | Brandon Bradley |
| [SPARK-12735](https://issues.apache.org/jira/browse/SPARK-12735) | Move spark-ec2 scripts to AMPLab |  Major | EC2 | Reynold Xin | Reynold Xin |
| [SPARK-12730](https://issues.apache.org/jira/browse/SPARK-12730) | De-duplicate some test code in BlockManagerSuite |  Major | Tests | Josh Rosen | Josh Rosen |
| [SPARK-12701](https://issues.apache.org/jira/browse/SPARK-12701) | Logging FileAppender should use join to ensure thread is finished |  Minor | Spark Core | Bryan Cutler | Bryan Cutler |
| [SPARK-12700](https://issues.apache.org/jira/browse/SPARK-12700) | SortMergeJoin and BroadcastHashJoin should support condition |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12663](https://issues.apache.org/jira/browse/SPARK-12663) | More informative error message in MLUtils.loadLibSVMFile |  Minor | MLlib | Robert Dodier | Robert Dodier |
| [SPARK-12656](https://issues.apache.org/jira/browse/SPARK-12656) | Rewrite Intersect phyiscal plan using semi-join |  Major | SQL | Reynold Xin | Xiao Li |
| [SPARK-12645](https://issues.apache.org/jira/browse/SPARK-12645) | SparkR support hash function |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12643](https://issues.apache.org/jira/browse/SPARK-12643) | Set lib directory for antlr |  Minor | Build | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-12642](https://issues.apache.org/jira/browse/SPARK-12642) | improve the hash expression to be decoupled from unsafe row |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12637](https://issues.apache.org/jira/browse/SPARK-12637) | Print stage info of finished stages properly |  Trivial | Spark Core | Navis | Navis |
| [SPARK-12636](https://issues.apache.org/jira/browse/SPARK-12636) | Expose API on UnsafeRowRecordReader to just run on files |  Major | SQL | Nong Li | Nong Li |
| [SPARK-12616](https://issues.apache.org/jira/browse/SPARK-12616) | Union logical plan should support arbitrary number of children (rather than binary) |  Major | SQL | Reynold Xin | Xiao Li |
| [SPARK-12608](https://issues.apache.org/jira/browse/SPARK-12608) | Remove submitJobThreadPool since submitJob doesn't create a separate thread to wait for the job result |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12603](https://issues.apache.org/jira/browse/SPARK-12603) | PySpark MLlib GaussianMixtureModel should support single instance predict/predictSoft |  Minor | MLlib, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-12599](https://issues.apache.org/jira/browse/SPARK-12599) | Remove the use of the deprecated callUDF in MLlib |  Major | MLlib, SQL | Reynold Xin | Reynold Xin |
| [SPARK-12594](https://issues.apache.org/jira/browse/SPARK-12594) | Outer Join Elimination by Filter Condition |  Critical | Optimizer, SQL | Xiao Li | Xiao Li |
| [SPARK-12585](https://issues.apache.org/jira/browse/SPARK-12585) | The numFields of UnsafeRow should not changed by pointTo() |  Major | SQL | Davies Liu | Apache Spark |
| [SPARK-12580](https://issues.apache.org/jira/browse/SPARK-12580) | Remove string concatenations from usage and extended in @ExpressionDescription |  Minor | SQL | Kazuaki Ishizaki | Kazuaki Ishizaki |
| [SPARK-12564](https://issues.apache.org/jira/browse/SPARK-12564) | Improve missing column AnalysisException |  Minor | SQL | Michael Armbrust | Xiao Li |
| [SPARK-12549](https://issues.apache.org/jira/browse/SPARK-12549) | UDFs' input type specification should take Option[Seq[DataType]] rather than Seq[DataType] |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12547](https://issues.apache.org/jira/browse/SPARK-12547) | Tighten scala style checker enforcement for UDF registration |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12537](https://issues.apache.org/jira/browse/SPARK-12537) | Add option to accept quoting of all character backslash quoting mechanism |  Major | SQL | Cazen Lee | Cazen Lee |
| [SPARK-12534](https://issues.apache.org/jira/browse/SPARK-12534) | Document missing command line options to Spark properties mapping |  Minor | Deploy, Documentation, YARN | Felix Cheung | Felix Cheung |
| [SPARK-12515](https://issues.apache.org/jira/browse/SPARK-12515) | Minor clarification on DataFrameReader.jdbc doc |  Trivial | Documentation, SQL | Felix Cheung | Felix Cheung |
| [SPARK-12510](https://issues.apache.org/jira/browse/SPARK-12510) | Refactor ActorReceiver to support Java |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12503](https://issues.apache.org/jira/browse/SPARK-12503) | Pushdown a Limit on top of a Union |  Major | Optimizer, SQL | Xiao Li | Josh Rosen |
| [SPARK-12500](https://issues.apache.org/jira/browse/SPARK-12500) | Fix Tachyon deprecations; pull Tachyon dependency into one class |  Minor | Spark Core | Sean Owen | Sean Owen |
| [SPARK-12498](https://issues.apache.org/jira/browse/SPARK-12498) | BooleanSimplification cleanup |  Minor | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12490](https://issues.apache.org/jira/browse/SPARK-12490) | Don't use Javascript for web UI's paginated table navigation controls |  Major | Web UI | Josh Rosen | Josh Rosen |
| [SPARK-12476](https://issues.apache.org/jira/browse/SPARK-12476) | Implement JdbcRelation#unhandledFilters for removing unnecessary Spark Filter |  Major | SQL | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-12475](https://issues.apache.org/jira/browse/SPARK-12475) | Upgrade Zinc from 0.3.5.3 to 0.3.9 |  Major | Build, Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-12471](https://issues.apache.org/jira/browse/SPARK-12471) | Spark daemons should log their pid in the log file |  Major | Spark Core | Nong Li | Nong Li |
| [SPARK-12450](https://issues.apache.org/jira/browse/SPARK-12450) | Un-persist broadcasted variables in KMeans |  Minor | MLlib | RJ Nowling | RJ Nowling |
| [SPARK-12440](https://issues.apache.org/jira/browse/SPARK-12440) | Avoid setCheckpointDir warning when filesystem is not local |  Trivial | Spark Core | Pierre Borckmans | Pierre Borckmans |
| [SPARK-12438](https://issues.apache.org/jira/browse/SPARK-12438) | Add SQLUserDefinedType support for encoder |  Major | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-12411](https://issues.apache.org/jira/browse/SPARK-12411) | Reconsider executor heartbeats rpc timeout |  Major | Spark Core | Nong Li | Nong Li |
| [SPARK-12409](https://issues.apache.org/jira/browse/SPARK-12409) | JDBC AND operator push down |  Minor | SQL | Huaxin Gao | Takeshi Yamamuro |
| [SPARK-12400](https://issues.apache.org/jira/browse/SPARK-12400) | Avoid writing a shuffle file if a partition has no output (empty) |  Major | Shuffle | Reynold Xin | Saisai Shao |
| [SPARK-12398](https://issues.apache.org/jira/browse/SPARK-12398) | Smart truncation of DataFrame / Dataset toString |  Major | SQL | Reynold Xin | Dilip Biswal |
| [SPARK-12397](https://issues.apache.org/jira/browse/SPARK-12397) | Improve error messages for data sources when they are not found |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12392](https://issues.apache.org/jira/browse/SPARK-12392) | Optimize a location order of broadcast blocks by considering preferred local hosts |  Major | Spark Core | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-12391](https://issues.apache.org/jira/browse/SPARK-12391) | JDBC OR operator push down |  Minor | SQL | Huaxin Gao | Takeshi Yamamuro |
| [SPARK-12388](https://issues.apache.org/jira/browse/SPARK-12388) | Change default compressor to LZ4 |  Minor | SQL | Davies Liu | Davies Liu |
| [SPARK-12387](https://issues.apache.org/jira/browse/SPARK-12387) | JDBC  IN operator push down |  Minor | SQL | Huaxin Gao | Takeshi Yamamuro |
| [SPARK-12374](https://issues.apache.org/jira/browse/SPARK-12374) | Improve performance of Range APIs via adding logical/physical operators |  Critical | SQL | Xiao Li | Apache Spark |
| [SPARK-12368](https://issues.apache.org/jira/browse/SPARK-12368) | Better doc for the binary classification evaluator' metricName |  Minor | Documentation, ML | Benjamin Fradet | Benjamin Fradet |
| [SPARK-12364](https://issues.apache.org/jira/browse/SPARK-12364) | Add ML example for SparkR |  Major | ML, SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12362](https://issues.apache.org/jira/browse/SPARK-12362) | Create a full-fledged built-in SQL parser |  Critical | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-12361](https://issues.apache.org/jira/browse/SPARK-12361) | Should set PYSPARK\_DRIVER\_PYTHON before python test |  Minor | PySpark, Tests | Jeff Zhang | Jeff Zhang |
| [SPARK-12349](https://issues.apache.org/jira/browse/SPARK-12349) | Make spark.ml PCAModel load backwards compatible |  Minor | ML | Joseph K. Bradley | Sean Owen |
| [SPARK-12332](https://issues.apache.org/jira/browse/SPARK-12332) | Typo in ResetSystemProperties.scala's comments |  Trivial | Tests | holdenk | holdenk |
| [SPARK-12331](https://issues.apache.org/jira/browse/SPARK-12331) | R^2 for regression through the origin |  Minor | ML | Imran Younus | Imran Younus |
| [SPARK-12317](https://issues.apache.org/jira/browse/SPARK-12317) | Support configurate value for AUTO\_BROADCASTJOIN\_THRESHOLD and SHUFFLE\_TARGET\_POSTSHUFFLE\_INPUT\_SIZE with unit(e.g. kb/mb/gb) in SQLConf |  Minor | SQL | Yadong Qi | kevin yu |
| [SPARK-12315](https://issues.apache.org/jira/browse/SPARK-12315) | isnotnull operator not pushed down for JDBC datasource. |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12314](https://issues.apache.org/jira/browse/SPARK-12314) | isnull operator not pushed down for JDBC datasource. |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12309](https://issues.apache.org/jira/browse/SPARK-12309) | Use sqlContext from MLlibTestSparkContext for spark.ml test suites |  Major | ML | Yanbo Liang | Yanbo Liang |
| [SPARK-12304](https://issues.apache.org/jira/browse/SPARK-12304) | Make Spark Streaming web UI display more friendly Receiver graphs |  Minor | Streaming | Liwei Lin | Liwei Lin |
| [SPARK-12295](https://issues.apache.org/jira/browse/SPARK-12295) | Manage the memory used by window function |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12294](https://issues.apache.org/jira/browse/SPARK-12294) | Support UnsafeRow in HiveTableScan |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12293](https://issues.apache.org/jira/browse/SPARK-12293) | Support UnsafeRow in LocalTableScan |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12292](https://issues.apache.org/jira/browse/SPARK-12292) | Support UnsafeRow in Generate |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12290](https://issues.apache.org/jira/browse/SPARK-12290) | Change the default value in SparkPlan |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12289](https://issues.apache.org/jira/browse/SPARK-12289) | Support UnsafeRow in TakeOrderedAndProject/Limit |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12288](https://issues.apache.org/jira/browse/SPARK-12288) | Support UnsafeRow in Coalesce/Except/Intersect |  Major | SQL | Davies Liu | Xiao Li |
| [SPARK-12287](https://issues.apache.org/jira/browse/SPARK-12287) | Support UnsafeRow in MapPartitions/MapGroups/CoGroup |  Major | SQL | Davies Liu | Xiao Li |
| [SPARK-12284](https://issues.apache.org/jira/browse/SPARK-12284) | Output UnsafeRow from window function |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12273](https://issues.apache.org/jira/browse/SPARK-12273) | Spark Streaming Web UI does not list Receivers in order |  Minor | Streaming, Web UI | Liwei Lin | Liwei Lin |
| [SPARK-12269](https://issues.apache.org/jira/browse/SPARK-12269) | Update aws-java-sdk version |  Minor | Streaming | Brian London | Brian London |
| [SPARK-12263](https://issues.apache.org/jira/browse/SPARK-12263) | IllegalStateException: Memory can't be 0 for SPARK\_WORKER\_MEMORY without unit |  Trivial | Documentation | Jacek Laskowski | Neelesh Srinivas Salian |
| [SPARK-12249](https://issues.apache.org/jira/browse/SPARK-12249) | JDBC non-equality comparison operator not pushed down. |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12241](https://issues.apache.org/jira/browse/SPARK-12241) | Improve failure reporting in Yarn client obtainTokenForHBase() |  Minor | YARN | Steve Loughran | Steve Loughran |
| [SPARK-12228](https://issues.apache.org/jira/browse/SPARK-12228) | Use in-memory for execution hive's derby metastore |  Major | SQL | Yin Huai | Yin Huai |
| [SPARK-12213](https://issues.apache.org/jira/browse/SPARK-12213) | Query with only one distinct should not having on expand |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12166](https://issues.apache.org/jira/browse/SPARK-12166) | Unset hadoop related environment in testing |  Minor | Tests | Jeff Zhang | Jeff Zhang |
| [SPARK-12164](https://issues.apache.org/jira/browse/SPARK-12164) | [SQL] Display the binary/encoded values |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-12150](https://issues.apache.org/jira/browse/SPARK-12150) | numPartitions argument to sqlContext.range()  should be optional |  Minor | SQL | Henri DF | Xiao Li |
| [SPARK-12130](https://issues.apache.org/jira/browse/SPARK-12130) | Replace shuffleManagerClass with shortShuffleMgrNames in ExternalShuffleBlockResolver |  Major | Shuffle, YARN | Lianhui Wang | Lianhui Wang |
| [SPARK-12120](https://issues.apache.org/jira/browse/SPARK-12120) | Improve exception message when failing to initialize HiveContext in PySpark |  Minor | PySpark | Jeff Zhang | Jeff Zhang |
| [SPARK-12115](https://issues.apache.org/jira/browse/SPARK-12115) | Change numPartitions() in RDD to be "getNumPartitions" to be consistent with pyspark/scala |  Major | SparkR | Sun Rui | Yanbo Liang |
| [SPARK-12103](https://issues.apache.org/jira/browse/SPARK-12103) | Clarify documentation of KafkaUtils createStream with multiple topics |  Minor | Documentation, Streaming | Dan Dutrow | Cody Koeninger |
| [SPARK-12096](https://issues.apache.org/jira/browse/SPARK-12096) | remove the old constraint in word2vec |  Trivial | MLlib | yuhao yang | yuhao yang |
| [SPARK-12080](https://issues.apache.org/jira/browse/SPARK-12080) | Kryo - Support multiple user registrators |  Minor | Spark Core | Rotem Shaul | Rotem Shaul |
| [SPARK-12074](https://issues.apache.org/jira/browse/SPARK-12074) | Avoid memory copy involving ByteBuffer.wrap(ByteArrayOutputStream.toByteArray) |  Major | Spark Core | Ted Yu | Ted Yu |
| [SPARK-12060](https://issues.apache.org/jira/browse/SPARK-12060) | Avoid memory copy in JavaSerializerInstance.serialize |  Critical | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12057](https://issues.apache.org/jira/browse/SPARK-12057) | Prevent failure on corrupt JSON records |  Minor | SQL | Ian Macalinao | Yin Huai |
| [SPARK-12054](https://issues.apache.org/jira/browse/SPARK-12054) | Consider nullable in codegen |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12044](https://issues.apache.org/jira/browse/SPARK-12044) | Fix usage of isnan, isNaN |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12032](https://issues.apache.org/jira/browse/SPARK-12032) | Filter can't be pushed down to correct Join because of bad order of Join |  Critical | SQL | Davies Liu | Davies Liu |
| [SPARK-11988](https://issues.apache.org/jira/browse/SPARK-11988) | Update JPMML to 1.2.7 |  Minor | ML, MLlib | Sean Owen | Sean Owen |
| [SPARK-11983](https://issues.apache.org/jira/browse/SPARK-11983) | remove all unused codegen fallback traits |  Minor | SQL | Adrian Wang | Adrian Wang |
| [SPARK-11982](https://issues.apache.org/jira/browse/SPARK-11982) | Improve performance of CartesianProduct |  Minor | SQL | Davies Liu | Davies Liu |
| [SPARK-11955](https://issues.apache.org/jira/browse/SPARK-11955) | Mark one side fields in merging schema for safely pushdowning filters in parquet |  Major | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-11929](https://issues.apache.org/jira/browse/SPARK-11929) | spark-shell log level customization is lost if user provides a log4j.properties file |  Minor | Spark Core, Spark Shell | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-11904](https://issues.apache.org/jira/browse/SPARK-11904) | pyspark reduceByKeyAndWindow with invFunc=None requires checkpointing |  Major | PySpark | David Tolpin | David Tolpin |
| [SPARK-11903](https://issues.apache.org/jira/browse/SPARK-11903) | Deprecate make-distribution.sh --skip-java-test |  Minor | Build | Nicholas Chammas | Nicholas Chammas |
| [SPARK-11898](https://issues.apache.org/jira/browse/SPARK-11898) | Use broadcast for the global tables in Word2Vec |  Major | MLlib | yuhao yang | yuhao yang |
| [SPARK-11884](https://issues.apache.org/jira/browse/SPARK-11884) | Drop multiple columns in the DataFrame API |  Minor | Spark Core | Ted Yu | Ted Yu |
| [SPARK-11878](https://issues.apache.org/jira/browse/SPARK-11878) | Eliminate distribute by in case group by is present with exactly the same grouping expressions |  Minor | SQL | Yash Datta | Yash Datta |
| [SPARK-11824](https://issues.apache.org/jira/browse/SPARK-11824) | WebUI throws console error for descriptions with 'bad' HTML |  Minor | SQL, Web UI | Andy Robb | Sean Owen |
| [SPARK-11717](https://issues.apache.org/jira/browse/SPARK-11717) | Ignore R session and history files from git |  Trivial | SparkR | Kai Sasaki | Kai Sasaki |
| [SPARK-11692](https://issues.apache.org/jira/browse/SPARK-11692) | Support for Parquet logical types, JSON and BSON (embedded types) |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-11622](https://issues.apache.org/jira/browse/SPARK-11622) | Make LibSVMRelation extends HadoopFsRelation and Add LibSVMOutputWriter |  Minor | MLlib | Jeff Zhang | Jeff Zhang |
| [SPARK-11592](https://issues.apache.org/jira/browse/SPARK-11592) | flush spark-sql command line history to history file |  Minor | SQL | Adrian Wang | Adrian Wang |
| [SPARK-11565](https://issues.apache.org/jira/browse/SPARK-11565) | replace deprecated DigestUtils.shaHex call |  Minor | SQL | Gabor Liptak | Gabor Liptak |
| [SPARK-11531](https://issues.apache.org/jira/browse/SPARK-11531) | PySpark SparseVector: improve error message for bad indices |  Trivial | MLlib, PySpark | Urvish Parikh | Rekha Joshi |
| [SPARK-11530](https://issues.apache.org/jira/browse/SPARK-11530) | Return eigenvalues with PCA model |  Minor | ML, MLlib | Christos Iraklis Tsatsoulis | Sean Owen |
| [SPARK-11439](https://issues.apache.org/jira/browse/SPARK-11439) | Optimization of creating sparse feature without dense one |  Minor | ML | Kai Sasaki | Nakul Jindal |
| [SPARK-11295](https://issues.apache.org/jira/browse/SPARK-11295) | Add packages to JUnit output for Python tests |  Minor | PySpark, Tests | Gabor Liptak | Gabor Liptak |
| [SPARK-11259](https://issues.apache.org/jira/browse/SPARK-11259) | Params.validateParams() should be called automatically |  Minor | ML | Yanbo Liang | Yanbo Liang |
| [SPARK-11164](https://issues.apache.org/jira/browse/SPARK-11164) | Add InSet pushdown filter back for Parquet |  Major | SQL | Liang-Chi Hsieh | Xiao Li |
| [SPARK-11155](https://issues.apache.org/jira/browse/SPARK-11155) | Stage summary json should include stage duration |  Minor | Web UI | Imran Rashid | Xin Ren |
| [SPARK-11044](https://issues.apache.org/jira/browse/SPARK-11044) | Parquet writer version fixed as version1 |  Minor | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-10991](https://issues.apache.org/jira/browse/SPARK-10991) | LogisticRegressionTrainingSummary should dynamically add prediction col if there is no prediction col set |  Minor | ML | holdenk | holdenk |
| [SPARK-10985](https://issues.apache.org/jira/browse/SPARK-10985) | Avoid passing evicted blocks throughout BlockManager / CacheManager |  Minor | Block Manager, Spark Core | Andrew Or | Josh Rosen |
| [SPARK-10963](https://issues.apache.org/jira/browse/SPARK-10963) | Make KafkaCluster api public |  Minor | Streaming | Cody Koeninger | Cody Koeninger |
| [SPARK-10911](https://issues.apache.org/jira/browse/SPARK-10911) | Executors should System.exit on clean shutdown |  Minor | Spark Core | Thomas Graves | Zhuo Liu |
| [SPARK-10749](https://issues.apache.org/jira/browse/SPARK-10749) | Support multiple roles with Spark Mesos dispatcher |  Major | Mesos | Timothy Chen | Timothy Chen |
| [SPARK-10509](https://issues.apache.org/jira/browse/SPARK-10509) | Excessive param boiler plate code |  Minor | ML, PySpark | holdenk | holdenk |
| [SPARK-10498](https://issues.apache.org/jira/browse/SPARK-10498) | Add requirements file for create dev python tools |  Minor | Build | holdenk | holdenk |
| [SPARK-10477](https://issues.apache.org/jira/browse/SPARK-10477) | using DSL in ColumnPruningSuite to improve readablity |  Trivial | SQL, Tests | Wenchen Fan | Wenchen Fan |
| [SPARK-10299](https://issues.apache.org/jira/browse/SPARK-10299) | word2vec should allow users to specify the window size |  Minor | MLlib | holdenk | holdenk |
| [SPARK-10180](https://issues.apache.org/jira/browse/SPARK-10180) | JDBCRDD does not process EqualNullSafe filter. |  Minor | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-10158](https://issues.apache.org/jira/browse/SPARK-10158) | ALS should print better errors when given Long IDs |  Minor | ML, MLlib, PySpark | Joseph K. Bradley | Bryan Cutler |
| [SPARK-10123](https://issues.apache.org/jira/browse/SPARK-10123) | Cannot set "--deploy-mode" in default configuration |  Minor | Spark Core | Marcelo Vanzin | Saisai Shao |
| [SPARK-9716](https://issues.apache.org/jira/browse/SPARK-9716) | BinaryClassificationEvaluator should accept Double prediction column |  Minor | ML | Joseph K. Bradley | Benjamin Fradet |
| [SPARK-9383](https://issues.apache.org/jira/browse/SPARK-9383) | Merge script should reset back to previous ref instead of detached commit |  Trivial | Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-8968](https://issues.apache.org/jira/browse/SPARK-8968) | dynamic partitioning in spark sql performance issue due to the high GC overhead |  Major | SQL | Fei Wang | Fei Wang |
| [SPARK-8964](https://issues.apache.org/jira/browse/SPARK-8964) | Use Exchange in limit operations (per partition limit -\> exchange to one partition -\> per partition limit) |  Major | SQL | Josh Rosen | Josh Rosen |
| [SPARK-8745](https://issues.apache.org/jira/browse/SPARK-8745) | Remove GenerateProjection |  Major | SQL | Reynold Xin | Davies Liu |
| [SPARK-8725](https://issues.apache.org/jira/browse/SPARK-8725) | Test modules in topological order in dev/run-tests and python/run-tests |  Minor | Build, Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-7889](https://issues.apache.org/jira/browse/SPARK-7889) | Jobs progress of apps on complete page of HistoryServer shows uncompleted |  Minor | Spark Core | meiyoula | Steve Loughran |
| [SPARK-7729](https://issues.apache.org/jira/browse/SPARK-7729) | Executor which has been killed should also be displayed on Executors Tab. |  Minor | Web UI | Archit Thakur | Lianhui Wang |
| [SPARK-7727](https://issues.apache.org/jira/browse/SPARK-7727) | Avoid inner classes in RuleExecutor |  Major | SQL | Santiago M. Mola | Stephan Kessler |
| [SPARK-7675](https://issues.apache.org/jira/browse/SPARK-7675) | PySpark spark.ml Params type conversions |  Minor | ML, PySpark | Joseph K. Bradley | holdenk |
| [SPARK-7617](https://issues.apache.org/jira/browse/SPARK-7617) | Word2VecModel fVector not normalized |  Trivial | MLlib | Eric Li | YongGang Cao |
| [SPARK-6363](https://issues.apache.org/jira/browse/SPARK-6363) | Switch to Scala 2.11 for default build |  Minor | Build | antonkulaga | Josh Rosen |
| [SPARK-6166](https://issues.apache.org/jira/browse/SPARK-6166) | Limit number of in flight outbound requests for shuffle fetch |  Minor | Spark Core | Mridul Muralidharan | Sanket Reddy |
| [SPARK-5865](https://issues.apache.org/jira/browse/SPARK-5865) | Add doc warnings for methods that return local data structures |  Minor | Spark Core, SQL | Nicholas Chammas | Tommy Yu |
| [SPARK-5273](https://issues.apache.org/jira/browse/SPARK-5273) | Improve documentation examples for LinearRegression |  Minor | Documentation | Dev Lakhani | Sean Owen |
| [SPARK-5095](https://issues.apache.org/jira/browse/SPARK-5095) | Support launching multiple mesos executors in coarse grained mesos mode |  Major | Mesos | Timothy Chen | Timothy Chen |
| [SPARK-4117](https://issues.apache.org/jira/browse/SPARK-4117) | Spark on Yarn handle AM being told command from RM |  Major | YARN | Thomas Graves | Devaraj K |
| [SPARK-2930](https://issues.apache.org/jira/browse/SPARK-2930) | clarify docs on using webhdfs with spark.yarn.access.namenodes |  Trivial | Documentation, YARN | Thomas Graves | Thomas Graves |
| [SPARK-1832](https://issues.apache.org/jira/browse/SPARK-1832) | Executor UI improvement suggestions |  Major | Web UI | Thomas Graves | Alex Bozarth |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13472](https://issues.apache.org/jira/browse/SPARK-13472) | Fix unstable Kmeans test in R |  Major | SparkR | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-13440](https://issues.apache.org/jira/browse/SPARK-13440) | Option fields in Datasets cause analysis exceptions when resolving columns |  Major | SQL | Josh Rosen | Michael Armbrust |
| [SPARK-13431](https://issues.apache.org/jira/browse/SPARK-13431) | Maven build fails due to: Method code too large! in Catalyst |  Blocker | Build | Stavros Kontopoulos | Davies Liu |
| [SPARK-13410](https://issues.apache.org/jira/browse/SPARK-13410) | unionAll AnalysisException with DataFrames containing UDT columns. |  Major | SQL | Franklyn Dsouza | Franklyn Dsouza |
| [SPARK-13408](https://issues.apache.org/jira/browse/SPARK-13408) | Exception in resultHandler will shutdown SparkContext |  Major | . | Davies Liu | Shixiong Zhu |
| [SPARK-13407](https://issues.apache.org/jira/browse/SPARK-13407) | TaskMetrics.fromAccumulatorUpdates can crash when trying to access garbage-collected accumulators |  Major | Spark Core | Josh Rosen | Josh Rosen |
| [SPARK-13405](https://issues.apache.org/jira/browse/SPARK-13405) | Flaky test: o.a.s.sql.util.ContinuousQueryListenerSuite.event ordering |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-13384](https://issues.apache.org/jira/browse/SPARK-13384) | Keep attribute qualifiers after dedup in Analyzer |  Major | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-13383](https://issues.apache.org/jira/browse/SPARK-13383) | Keep broadcast hint after column pruning |  Major | SQL | Liang-Chi Hsieh |  |
| [SPARK-13379](https://issues.apache.org/jira/browse/SPARK-13379) | MLlib LogisticRegressionWithLBFGS swaps L1 and L2 incorrectly |  Major | MLlib | Yanbo Liang | Yanbo Liang |
| [SPARK-13371](https://issues.apache.org/jira/browse/SPARK-13371) | TaskSetManager.dequeueSpeculativeTask compares Option[String] and String directly. |  Major | Scheduler | Guoqiang Li | Sean Owen |
| [SPARK-13358](https://issues.apache.org/jira/browse/SPARK-13358) | Retrieve grep path when doing Benchmark |  Minor | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-13355](https://issues.apache.org/jira/browse/SPARK-13355) | Replace GraphImpl.fromExistingRDDs by Graph |  Major | ML, MLlib | Xiangrui Meng | Xiangrui Meng |
| [SPARK-13351](https://issues.apache.org/jira/browse/SPARK-13351) | Column pruning fails on expand |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13344](https://issues.apache.org/jira/browse/SPARK-13344) | Tests have many "accumulator not found" exceptions |  Major | SQL, Tests | Andrew Or | Andrew Or |
| [SPARK-13338](https://issues.apache.org/jira/browse/SPARK-13338) | [ML] Allow setting 'degree' parameter to 1 for PolynomialExpansion |  Major | ML, MLlib | Grzegorz Chilkiewicz | Grzegorz Chilkiewicz |
| [SPARK-13334](https://issues.apache.org/jira/browse/SPARK-13334) | ML KMeansModel/BisectingKMeansModel should be set parent |  Minor | ML | Yanbo Liang | Yanbo Liang |
| [SPARK-13321](https://issues.apache.org/jira/browse/SPARK-13321) | Support nested UNION in parser |  Major | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-13312](https://issues.apache.org/jira/browse/SPARK-13312) | ML Model Selection via Train Validation Split example uses incorrect data |  Minor | Documentation | Jeremy | Jeremy |
| [SPARK-13310](https://issues.apache.org/jira/browse/SPARK-13310) | Missing Sorting Columns in Generate |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-13308](https://issues.apache.org/jira/browse/SPARK-13308) | ManagedBuffers passed to OneToOneStreamManager need to be freed in non-error cases |  Major | Spark Core | Josh Rosen | Josh Rosen |
| [SPARK-13304](https://issues.apache.org/jira/browse/SPARK-13304) | Broadcast join with two ints could be very slow |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13300](https://issues.apache.org/jira/browse/SPARK-13300) | Spark examples page gives errors : Liquid error: pygments |  Minor | Documentation | stefan | Amit Ranjit |
| [SPARK-13298](https://issues.apache.org/jira/browse/SPARK-13298) | DAG visualization does not render correctly for jobs |  Major | Web UI | Lucas Woltmann | Shixiong Zhu |
| [SPARK-13278](https://issues.apache.org/jira/browse/SPARK-13278) | Launcher fails to start with JDK 9 EA |  Minor | Spark Core | Claes Redestad | Claes Redestad |
| [SPARK-13277](https://issues.apache.org/jira/browse/SPARK-13277) | ANTLR ignores other rule using the USING keyword |  Minor | SQL | Herman van Hovell | Liang-Chi Hsieh |
| [SPARK-13276](https://issues.apache.org/jira/browse/SPARK-13276) | Parse Table Identifiers/Expression skips bad characters at the end of the passed string |  Minor | SQL | Herman van Hovell | Herman van Hovell |
| [SPARK-13270](https://issues.apache.org/jira/browse/SPARK-13270) | Improve readability of whole stage codegen by skipping empty lines and outputting the pipeline plan |  Major | . | Nong Li | Nong Li |
| [SPARK-13265](https://issues.apache.org/jira/browse/SPARK-13265) | Refactoring of basic ML import/export for other file system besides HDFS |  Major | ML | Yu Ishikawa | Yu Ishikawa |
| [SPARK-13260](https://issues.apache.org/jira/browse/SPARK-13260) | count(\*) does not work with CSV data source |  Major | SQL | Hossein Falaki | Hyukjin Kwon |
| [SPARK-13254](https://issues.apache.org/jira/browse/SPARK-13254) | Fix planning of TakeOrderedAndProject operator |  Major | SQL | Josh Rosen | Josh Rosen |
| [SPARK-13245](https://issues.apache.org/jira/browse/SPARK-13245) | ShuffleBlockFetcherIterator should not use shuffleMetrics in multiple threads |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-13221](https://issues.apache.org/jira/browse/SPARK-13221) | GroupingSets Returns an Incorrect Results |  Critical | SQL | Xiao Li | Xiao Li |
| [SPARK-13210](https://issues.apache.org/jira/browse/SPARK-13210) | NPE in Sort |  Critical | SQL | Davies Liu | Davies Liu |
| [SPARK-13187](https://issues.apache.org/jira/browse/SPARK-13187) | Add boolean/long/double type option functions in DataFrameReader/Writer |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13163](https://issues.apache.org/jira/browse/SPARK-13163) | Column width on new History Server DataTables not getting set correctly |  Minor | Web UI | Alex Bozarth | Alex Bozarth |
| [SPARK-13162](https://issues.apache.org/jira/browse/SPARK-13162) | Standalone mode does not respect `spark.dynamicAllocation.initialExecutors` |  Major | Deploy, Spark Core | Andrew Or | Andrew Or |
| [SPARK-13157](https://issues.apache.org/jira/browse/SPARK-13157) | ADD JAR command cannot handle path with @ character |  Blocker | SQL | Cheng Lian | Herman van Hovell |
| [SPARK-13153](https://issues.apache.org/jira/browse/SPARK-13153) | PySpark ML persistence failed when handle no default value parameter |  Minor | ML, PySpark | Tommy Yu | Tommy Yu |
| [SPARK-13142](https://issues.apache.org/jira/browse/SPARK-13142) | Problem accessing Web UI /logPage/ on Microsoft Windows |  Minor | Web UI | Neil Andrassy | Mark Pavey |
| [SPARK-13126](https://issues.apache.org/jira/browse/SPARK-13126) | History Server page always has horizontal scrollbar |  Minor | Web UI | Alex Bozarth | Zhuo Liu |
| [SPARK-13124](https://issues.apache.org/jira/browse/SPARK-13124) | Adding JQuery DataTables messed up the Web UI css and js |  Major | Web UI | Alex Bozarth | Alex Bozarth |
| [SPARK-13122](https://issues.apache.org/jira/browse/SPARK-13122) | Race condition in MemoryStore.unrollSafely() causes memory leak |  Major | Spark Core, Streaming | Adam Budde | Adam Budde |
| [SPARK-13121](https://issues.apache.org/jira/browse/SPARK-13121) | java mapWithState mishandles scala Option |  Critical | Java API, Streaming | Gabriele Nizzoli | Gabriele Nizzoli |
| [SPARK-13109](https://issues.apache.org/jira/browse/SPARK-13109) | SBT publishLocal failed to publish to local ivy repo |  Major | Build | Saisai Shao | Saisai Shao |
| [SPARK-13101](https://issues.apache.org/jira/browse/SPARK-13101) | Dataset complex types mapping to DataFrame  (element nullability) mismatch |  Blocker | SQL | Deenar Toraskar | Wenchen Fan |
| [SPARK-13096](https://issues.apache.org/jira/browse/SPARK-13096) | Make AccumulatorSuite#verifyPeakExecutionMemorySet less flaky |  Major | Tests | Andrew Or | Andrew Or |
| [SPARK-13095](https://issues.apache.org/jira/browse/SPARK-13095) | improve performance of hash join with dimension table |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13088](https://issues.apache.org/jira/browse/SPARK-13088) | DAG viz does not work with latest version of chrome |  Blocker | Web UI | Andrew Or | Andrew Or |
| [SPARK-13087](https://issues.apache.org/jira/browse/SPARK-13087) | Grouping by a complex expression may lead to incorrect AttributeReferences in aggregations |  Critical | SQL | Mark Hamstra | Michael Armbrust |
| [SPARK-13082](https://issues.apache.org/jira/browse/SPARK-13082) | sqlCtx.real.json() doesn't work with PythonRDD |  Major | PySpark | Gaëtan Lehmann | Shixiong Zhu |
| [SPARK-13067](https://issues.apache.org/jira/browse/SPARK-13067) | DataFrameSuite.simple explode fail locally |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-13056](https://issues.apache.org/jira/browse/SPARK-13056) | Map column would throw NPE if value is null |  Major | SQL | Adrian Wang | Adrian Wang |
| [SPARK-13055](https://issues.apache.org/jira/browse/SPARK-13055) | SQLHistoryListener throws ClassCastException |  Major | Spark Core, SQL | Andrew Or | Andrew Or |
| [SPARK-13053](https://issues.apache.org/jira/browse/SPARK-13053) | Rectify ignored tests in InternalAccumulatorSuite |  Major | Spark Core, Tests | Andrew Or | Andrew Or |
| [SPARK-13052](https://issues.apache.org/jira/browse/SPARK-13052) | waitingApps metric doesn't show the number of apps currently in the WAITING state |  Minor | Web UI | Raafat Akkad | Raafat Akkad |
| [SPARK-13050](https://issues.apache.org/jira/browse/SPARK-13050) | Scalatest tags fail builds with the addition of the sketch module |  Major | Build | Alex Bozarth | Alex Bozarth |
| [SPARK-13049](https://issues.apache.org/jira/browse/SPARK-13049) | Cannot use FIRST/LAST ignoreNulls option in 1.6 and below |  Minor | SQL | Herman van Hovell | Herman van Hovell |
| [SPARK-13047](https://issues.apache.org/jira/browse/SPARK-13047) | Pyspark Params.hasParam should not throw an error |  Minor | ML, PySpark | Seth Hendrickson | Seth Hendrickson |
| [SPARK-13023](https://issues.apache.org/jira/browse/SPARK-13023) | Check for presence of 'root' module after computing test\_modules, not changed\_modules |  Major | Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-13021](https://issues.apache.org/jira/browse/SPARK-13021) | Fail fast when custom RDD's violate RDD.partition's API contract |  Major | Spark Core | Josh Rosen | Josh Rosen |
| [SPARK-13002](https://issues.apache.org/jira/browse/SPARK-13002) | Mesos scheduler backend does not follow the property spark.dynamicAllocation.initialExecutors |  Major | Mesos | Luc Bourlier | Luc Bourlier |
| [SPARK-12989](https://issues.apache.org/jira/browse/SPARK-12989) | Bad interaction between StarExpansion and ExtractWindowExpressions |  Major | SQL | Michael Armbrust | Xiao Li |
| [SPARK-12986](https://issues.apache.org/jira/browse/SPARK-12986) | Fix pydoc warnings in mllib/regression.py |  Minor | MLlib, PySpark | Xiangrui Meng | Nam Pham |
| [SPARK-12979](https://issues.apache.org/jira/browse/SPARK-12979) | Paths are resolved relative to the local file system |  Major | Mesos | Iulian Dragos | Iulian Dragos |
| [SPARK-12971](https://issues.apache.org/jira/browse/SPARK-12971) | Address test isolation problems which broke Hive tests on Hadoop 2.3 SBT build |  Major | SQL, Tests | Josh Rosen | Josh Rosen |
| [SPARK-12966](https://issues.apache.org/jira/browse/SPARK-12966) | Postgres JDBC ArrayType(DecimalType) 'Unable to find server array type' |  Major | SQL | Brandon Bradley | Brandon Bradley |
| [SPARK-12961](https://issues.apache.org/jira/browse/SPARK-12961) | Work around memory leak in Snappy library |  Major | Spark Core | Josh Rosen | Liang-Chi Hsieh |
| [SPARK-12960](https://issues.apache.org/jira/browse/SPARK-12960) | Some examples are missing support for python2 |  Minor | PySpark | Mark Grover | Mark Grover |
| [SPARK-12959](https://issues.apache.org/jira/browse/SPARK-12959) | Writing Bucketed Data with Disabled Bucketing in SQLConf |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-12952](https://issues.apache.org/jira/browse/SPARK-12952) | EMLDAOptimizer initialize should return EMLDAOptimizer other than its parent class |  Trivial | MLlib | Xusen Yin | Xusen Yin |
| [SPARK-12939](https://issues.apache.org/jira/browse/SPARK-12939) | migrate encoder resolution to Analyzer |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12904](https://issues.apache.org/jira/browse/SPARK-12904) | Strength reduction for integer/decimal comparisons |  Major | Optimizer, SQL | Reynold Xin | Reynold Xin |
| [SPARK-12881](https://issues.apache.org/jira/browse/SPARK-12881) | Enable sub-expression Elimination in generated mutable projection |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12870](https://issues.apache.org/jira/browse/SPARK-12870) | better format bucket id in file name |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12867](https://issues.apache.org/jira/browse/SPARK-12867) | Nullability of Intersect can be stricter |  Minor | SQL | Cheng Lian | Xiao Li |
| [SPARK-12862](https://issues.apache.org/jira/browse/SPARK-12862) | Jenkins does not run R tests |  Major | SparkR | Felix Cheung | Felix Cheung |
| [SPARK-12859](https://issues.apache.org/jira/browse/SPARK-12859) | Names of input streams with receivers don't fit in Streaming page |  Trivial | Streaming, Web UI | Jacek Laskowski | Alex Bozarth |
| [SPARK-12842](https://issues.apache.org/jira/browse/SPARK-12842) | Add Hadoop 2.7 build profile |  Major | Build | Josh Rosen | Josh Rosen |
| [SPARK-12841](https://issues.apache.org/jira/browse/SPARK-12841) | UnresolvedException with cast |  Blocker | SQL | Michael Armbrust | Wenchen Fan |
| [SPARK-12821](https://issues.apache.org/jira/browse/SPARK-12821) | Style checker should run when some configuration files for style are modified but any source files are not. |  Minor | Project Infra | Kousuke Saruta | Kousuke Saruta |
| [SPARK-12816](https://issues.apache.org/jira/browse/SPARK-12816) | Schema generation for type aliases does not work |  Major | Spark Core | Jakob Odersky | Jakob Odersky |
| [SPARK-12807](https://issues.apache.org/jira/browse/SPARK-12807) | Spark External Shuffle not working in Hadoop clusters with Jackson 2.2.3 |  Critical | Shuffle, YARN | Steve Loughran | Steve Loughran |
| [SPARK-12805](https://issues.apache.org/jira/browse/SPARK-12805) | Outdated details in doc related to Mesos run modes |  Minor | Documentation | Luc Bourlier | Luc Bourlier |
| [SPARK-12804](https://issues.apache.org/jira/browse/SPARK-12804) | ml.classification.LogisticRegression fails when FitIntercept with same-label dataset |  Major | ML | Feynman Liang | Feynman Liang |
| [SPARK-12784](https://issues.apache.org/jira/browse/SPARK-12784) | Spark UI IndexOutOfBoundsException with dynamic allocation |  Major | Web UI, YARN | Thomas Graves | Shixiong Zhu |
| [SPARK-12780](https://issues.apache.org/jira/browse/SPARK-12780) | Inconsistency returning value of ML python models' properties |  Minor | ML, PySpark | Xusen Yin | Xusen Yin |
| [SPARK-12765](https://issues.apache.org/jira/browse/SPARK-12765) | CountVectorizerModel.transform lost the transformSchema |  Major | ML | sloth | sloth |
| [SPARK-12760](https://issues.apache.org/jira/browse/SPARK-12760) | inaccurate description for difference between local vs cluster mode in closure handling |  Minor | Documentation | Mortada Mehyar | Mortada Mehyar |
| [SPARK-12755](https://issues.apache.org/jira/browse/SPARK-12755) | Spark may attempt to rebuild application UI before finishing writing the event logs in possible race condition |  Minor | Spark Core | Michael Allman | Michael Allman |
| [SPARK-12747](https://issues.apache.org/jira/browse/SPARK-12747) | Postgres JDBC ArrayType(DoubleType) 'Unable to find server array type' |  Major | SQL | Brandon Bradley | Liang-Chi Hsieh |
| [SPARK-12746](https://issues.apache.org/jira/browse/SPARK-12746) | ArrayType(\_, true) should also accept ArrayType(\_, false) |  Major | ML, SQL | Earthson Lu | Earthson Lu |
| [SPARK-12744](https://issues.apache.org/jira/browse/SPARK-12744) | Inconsistent behavior parsing JSON with unix timestamp values |  Minor | SQL | Anatoliy Plastinin | Anatoliy Plastinin |
| [SPARK-12742](https://issues.apache.org/jira/browse/SPARK-12742) | org.apache.spark.sql.hive.LogicalPlanToSQLSuite failure due to Table already exists |  Major | SQL | Fei Wang | Fei Wang |
| [SPARK-12739](https://issues.apache.org/jira/browse/SPARK-12739) | Details of batch in Streaming tab uses two Duration columns |  Minor | Streaming, Web UI | Jacek Laskowski | Mario Briggs |
| [SPARK-12736](https://issues.apache.org/jira/browse/SPARK-12736) | Standalone Master cannot be started due to NoClassDefFoundError: org/spark-project/guava/collect/Maps |  Major | Deploy, Spark Core | Jacek Laskowski | Jacek Laskowski |
| [SPARK-12734](https://issues.apache.org/jira/browse/SPARK-12734) | Fix Netty exclusions and use Maven Enforcer to prevent bug from being reintroduced |  Major | Build, Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-12732](https://issues.apache.org/jira/browse/SPARK-12732) | Fix LinearRegression.train for the case when label is constant and fitIntercept=false |  Minor | MLlib | Imran Younus | Imran Younus |
| [SPARK-12711](https://issues.apache.org/jira/browse/SPARK-12711) | ML StopWordsRemover does not protect itself from column name duplication |  Trivial | ML, MLlib | Grzegorz Chilkiewicz | Grzegorz Chilkiewicz |
| [SPARK-12708](https://issues.apache.org/jira/browse/SPARK-12708) | Sorting task error in Stages Page when yarn mode |  Minor | Web UI | Koyo Yoshida | Koyo Yoshida |
| [SPARK-12690](https://issues.apache.org/jira/browse/SPARK-12690) | NullPointerException in UnsafeInMemorySorter.free() |  Minor | Spark Core | Carson Wang | Carson Wang |
| [SPARK-12685](https://issues.apache.org/jira/browse/SPARK-12685) | word2vec trainWordsCount gets overflow |  Minor | MLlib | yuhao yang | yuhao yang |
| [SPARK-12682](https://issues.apache.org/jira/browse/SPARK-12682) | Hive will fail if the schema of a parquet table has a very wide schema |  Major | SQL | Yin Huai | Sameer Agarwal |
| [SPARK-12678](https://issues.apache.org/jira/browse/SPARK-12678) | MapPartitionsRDD should clear reference to prev RDD |  Minor | Spark Core | Guillaume Poulin | Guillaume Poulin |
| [SPARK-12673](https://issues.apache.org/jira/browse/SPARK-12673) | Prepending base URI of job description is missing |  Major | Web UI | Saisai Shao | Saisai Shao |
| [SPARK-12662](https://issues.apache.org/jira/browse/SPARK-12662) | Add a local sort operator to DataFrame used by randomSplit |  Major | Documentation, SQL | Yin Huai | Sameer Agarwal |
| [SPARK-12659](https://issues.apache.org/jira/browse/SPARK-12659) | NPE when spill in CartisianProduct |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12655](https://issues.apache.org/jira/browse/SPARK-12655) | GraphX does not unpersist RDDs |  Minor | GraphX | Alexander Pivovarov | Jason C Lee |
| [SPARK-12654](https://issues.apache.org/jira/browse/SPARK-12654) | sc.wholeTextFiles with spark.hadoop.cloneConf=true fails on secure Hadoop |  Major | Spark Core | Thomas Graves | Thomas Graves |
| [SPARK-12652](https://issues.apache.org/jira/browse/SPARK-12652) | Upgrade py4j to the incoming version 0.9.1 |  Major | PySpark | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12638](https://issues.apache.org/jira/browse/SPARK-12638) | Parameter explaination not very accurate for rdd function "aggregate" |  Trivial | Documentation, Spark Core | Tommy Yu | Tommy Yu |
| [SPARK-12629](https://issues.apache.org/jira/browse/SPARK-12629) | SparkR: DataFrame's saveAsTable method has issues with the signature and HiveContext |  Major | SparkR | Narine Kokhlikyan | Narine Kokhlikyan |
| [SPARK-12625](https://issues.apache.org/jira/browse/SPARK-12625) | SparkR is using deprecated APIs |  Blocker | SparkR, SQL | Reynold Xin | Felix Cheung |
| [SPARK-12624](https://issues.apache.org/jira/browse/SPARK-12624) | When schema is specified, we should give better error message if actual row length doesn't match |  Blocker | PySpark, SQL | Reynold Xin | Cheng Lian |
| [SPARK-12617](https://issues.apache.org/jira/browse/SPARK-12617) | socket descriptor leak killing streaming app |  Critical | PySpark, Streaming | Antony Mayi | Shixiong Zhu |
| [SPARK-12614](https://issues.apache.org/jira/browse/SPARK-12614) | Don't throw non fatal exception from RpcEndpointRef.send/ask |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12612](https://issues.apache.org/jira/browse/SPARK-12612) | Add missing Hadoop profiles to dev/run-tests-\*.py scripts |  Major | Build, Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-12611](https://issues.apache.org/jira/browse/SPARK-12611) | test\_infer\_schema\_to\_local depended on old handling of missing value in row |  Trivial | SQL, Tests | holdenk | holdenk |
| [SPARK-12598](https://issues.apache.org/jira/browse/SPARK-12598) | Bug in setMinPartitions function of StreamFileInputFormat |  Minor | Spark Core | Darek Blasiak | Darek Blasiak |
| [SPARK-12591](https://issues.apache.org/jira/browse/SPARK-12591) | NullPointerException using checkpointed mapWithState with KryoSerializer |  Major | Streaming | Jan Uyttenhove | Shixiong Zhu |
| [SPARK-12589](https://issues.apache.org/jira/browse/SPARK-12589) | result row size is wrong in UnsafeRowParquetRecordReader |  Major | SQL | Wenchen Fan | Nong Li |
| [SPARK-12582](https://issues.apache.org/jira/browse/SPARK-12582) | IndexShuffleBlockResolverSuite fails in windows |  Major | Tests, Windows | yucai | yucai |
| [SPARK-12579](https://issues.apache.org/jira/browse/SPARK-12579) | User-specified JDBC driver should always take precedence |  Major | SQL | Josh Rosen | Josh Rosen |
| [SPARK-12562](https://issues.apache.org/jira/browse/SPARK-12562) | DataFrame.write.format("text") requires the column name to be called value |  Major | SQL | Michael Armbrust | Xiu (Joe) Guo |
| [SPARK-12558](https://issues.apache.org/jira/browse/SPARK-12558) | AnalysisException when multiple functions applied in GROUP BY clause |  Major | SQL | Maciej Bryński | Dilip Biswal |
| [SPARK-12546](https://issues.apache.org/jira/browse/SPARK-12546) | Writing to partitioned parquet table can fail with OOM |  Blocker | SQL | Nong Li | Michael Armbrust |
| [SPARK-12533](https://issues.apache.org/jira/browse/SPARK-12533) | hiveContext.table() throws the wrong exception |  Major | SQL | Michael Armbrust | Thomas Sebastian |
| [SPARK-12530](https://issues.apache.org/jira/browse/SPARK-12530) | Build break at Spark-Master-Maven-Snapshots from #1293 |  Major | Build | Kazuaki Ishizaki | Kazuaki Ishizaki |
| [SPARK-12526](https://issues.apache.org/jira/browse/SPARK-12526) | `ifelse`, `when`, `otherwise` unable to take Column as value |  Major | SparkR | Sen Fang | Sen Fang |
| [SPARK-12525](https://issues.apache.org/jira/browse/SPARK-12525) | Fix compiler warnings in Kinesis ASL module due to @transient annotations |  Major | Streaming | Josh Rosen | Josh Rosen |
| [SPARK-12522](https://issues.apache.org/jira/browse/SPARK-12522) | Add the missing the document string for the SQL configuration |  Minor | SQL | Xiao Li | Xiao Li |
| [SPARK-12520](https://issues.apache.org/jira/browse/SPARK-12520) | Python API dataframe join returns wrong results on outer join |  Major | PySpark, SQL | Aravind  B | Xiao Li |
| [SPARK-12517](https://issues.apache.org/jira/browse/SPARK-12517) | No default RDD name for ones created by sc.textFile |  Minor | Spark Core | yaron weinsberg | yaron weinsberg |
| [SPARK-12513](https://issues.apache.org/jira/browse/SPARK-12513) | SocketReceiver hang in Netcat example |  Minor | Streaming | Shawn Guo | Shawn Guo |
| [SPARK-12512](https://issues.apache.org/jira/browse/SPARK-12512) | WithColumn does not work on multiple column with special character |  Major | SQL | JO EE | Xiu (Joe) Guo |
| [SPARK-12511](https://issues.apache.org/jira/browse/SPARK-12511) | streaming driver with checkpointing unable to finalize leading to OOM |  Critical | PySpark, Streaming | Antony Mayi | Shixiong Zhu |
| [SPARK-12509](https://issues.apache.org/jira/browse/SPARK-12509) | Fix error messages for DataFrame correlation and covariance |  Minor | Documentation, SQL | Narine Kokhlikyan | Narine Kokhlikyan |
| [SPARK-12508](https://issues.apache.org/jira/browse/SPARK-12508) | Fix multiple bugs in pr\_public\_classes.sh script |  Trivial | Project Infra | Josh Rosen | Apache Spark |
| [SPARK-12504](https://issues.apache.org/jira/browse/SPARK-12504) | JDBC data source credentials are not masked in the data frame explain output. |  Major | SQL | Suresh Thalamati | Apache Spark |
| [SPARK-12502](https://issues.apache.org/jira/browse/SPARK-12502) | Script /dev/run-tests fails when IBM Java is used |  Minor | Tests | Kazuaki Ishizaki | Kazuaki Ishizaki |
| [SPARK-12499](https://issues.apache.org/jira/browse/SPARK-12499) | make\_distribution should not override MAVEN\_OPTS |  Minor | Build | Adrian Bridgett | Adrian Bridgett |
| [SPARK-12489](https://issues.apache.org/jira/browse/SPARK-12489) | Fix minor issues found by Findbugs |  Minor | MLlib, Spark Core, SQL | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12478](https://issues.apache.org/jira/browse/SPARK-12478) | Dataset fields of product types can't be null |  Major | SQL | Cheng Lian | Apache Spark |
| [SPARK-12477](https://issues.apache.org/jira/browse/SPARK-12477) | [SQL] Tungsten projection fails for null values in array fields |  Major | SQL | Pierre Borckmans | Pierre Borckmans |
| [SPARK-12470](https://issues.apache.org/jira/browse/SPARK-12470) | Incorrect calculation of row size in o.a.s.sql.catalyst.expressions.codegen.GenerateUnsafeRowJoiner |  Minor | SQL | Pete Robbins | Pete Robbins |
| [SPARK-12466](https://issues.apache.org/jira/browse/SPARK-12466) | Harmless Master NPE in tests |  Major | Deploy, Tests | Andrew Or | Andrew Or |
| [SPARK-12453](https://issues.apache.org/jira/browse/SPARK-12453) | Spark Streaming Kinesis Example broken due to wrong AWS Java SDK version |  Critical | Streaming | Martin Schade | Brian London |
| [SPARK-12442](https://issues.apache.org/jira/browse/SPARK-12442) | Build testing failed |  Blocker | Build | Xiao Li | Reynold Xin |
| [SPARK-12441](https://issues.apache.org/jira/browse/SPARK-12441) | Fixing missingInput in all Logical/Physical operators |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-12439](https://issues.apache.org/jira/browse/SPARK-12439) | Fix toCatalystArray and MapObjects |  Major | SQL | Liang-Chi Hsieh | Liang-Chi Hsieh |
| [SPARK-12424](https://issues.apache.org/jira/browse/SPARK-12424) | The implementation of ParamMap#filter is wrong. |  Major | ML | Kousuke Saruta | Kousuke Saruta |
| [SPARK-12421](https://issues.apache.org/jira/browse/SPARK-12421) | Fix copy() method of GenericRow |  Minor | SQL | doepfner | Herman van Hovell |
| [SPARK-12399](https://issues.apache.org/jira/browse/SPARK-12399) | Display correct error message when accessing REST API with an unknown app Id |  Minor | Web UI | Carson Wang | Carson Wang |
| [SPARK-12396](https://issues.apache.org/jira/browse/SPARK-12396) | Once driver client registered successfully,it still retry to connected to master. |  Minor | Spark Core | echo | echo |
| [SPARK-12395](https://issues.apache.org/jira/browse/SPARK-12395) | Result of DataFrame.join(usingColumns) could be wrong for outer join |  Blocker | SQL | Davies Liu | Davies Liu |
| [SPARK-12390](https://issues.apache.org/jira/browse/SPARK-12390) | Clean up unused serializer parameter in BlockManager |  Major | Block Manager, Spark Core | Andrew Or | Andrew Or |
| [SPARK-12380](https://issues.apache.org/jira/browse/SPARK-12380) | MLLib should use existing SQLContext instead create new one |  Major | MLlib, PySpark | Davies Liu | Davies Liu |
| [SPARK-12365](https://issues.apache.org/jira/browse/SPARK-12365) | Use ShutdownHookManager where Runtime.getRuntime.addShutdownHook() is called |  Minor | Spark Core | Ted Yu | Ted Yu |
| [SPARK-12363](https://issues.apache.org/jira/browse/SPARK-12363) | PowerIterationClustering test case failed if we deprecated KMeans.setRuns |  Minor | MLlib | Yanbo Liang | Liang-Chi Hsieh |
| [SPARK-12353](https://issues.apache.org/jira/browse/SPARK-12353) | wrong output for countByValue and countByValueAndWindow |  Major | Documentation, Input/Output, PySpark, Streaming | Bo Jin | Saisai Shao |
| [SPARK-12350](https://issues.apache.org/jira/browse/SPARK-12350) | VectorAssembler#transform() initially throws an exception |  Major | Spark Core, Spark Shell | Jakob Odersky | Marcelo Vanzin |
| [SPARK-12346](https://issues.apache.org/jira/browse/SPARK-12346) | GLM summary crashes with NoSuchElementException if attributes are missing names |  Major | SparkR | Eric Liang | Eric Liang |
| [SPARK-12340](https://issues.apache.org/jira/browse/SPARK-12340) | overstep the bounds of Int in SparkPlan.executeTake |  Major | SQL | QiangCai | QiangCai |
| [SPARK-12339](https://issues.apache.org/jira/browse/SPARK-12339) | NullPointerException on stage kill from web UI |  Major | Web UI | Jacek Laskowski | Alex Bozarth |
| [SPARK-12330](https://issues.apache.org/jira/browse/SPARK-12330) | Mesos coarse executor does not cleanup blockmgr properly on termination if data is stored on disk |  Major | Block Manager, Mesos | Charles Allen | Apache Spark |
| [SPARK-12327](https://issues.apache.org/jira/browse/SPARK-12327) | lint-r checks fail with commented code |  Major | SparkR | Shivaram Venkataraman | Felix Cheung |
| [SPARK-12324](https://issues.apache.org/jira/browse/SPARK-12324) | The documentation sidebar does not collapse properly |  Minor | Documentation | Timothy Hunter | Timothy Hunter |
| [SPARK-12318](https://issues.apache.org/jira/browse/SPARK-12318) | Save mode in SparkR should be error by default |  Minor | SparkR | Jeff Zhang | Jeff Zhang |
| [SPARK-12311](https://issues.apache.org/jira/browse/SPARK-12311) | [CORE] Restore previous value of "os.arch" property in test suites after forcing to set specific value to "os.arch" property |  Minor | Spark Core | Kazuaki Ishizaki | Kazuaki Ishizaki |
| [SPARK-12300](https://issues.apache.org/jira/browse/SPARK-12300) | Fix schema inferance on local collections |  Minor | PySpark, SQL | holdenk | holdenk |
| [SPARK-12298](https://issues.apache.org/jira/browse/SPARK-12298) | Infinite loop in DataFrame.sortWithinPartitions(String, String\*) |  Major | SQL | Ankur Dave | Ankur Dave |
| [SPARK-12275](https://issues.apache.org/jira/browse/SPARK-12275) | No plan for BroadcastHint in some condition |  Major | SQL | yucai | yucai |
| [SPARK-12271](https://issues.apache.org/jira/browse/SPARK-12271) | Improve error message for Dataset.as[] when the schema is incompatible. |  Major | SQL | Nong Li | Apache Spark |
| [SPARK-12268](https://issues.apache.org/jira/browse/SPARK-12268) | pyspark shell uses execfile which breaks python3 compatibility |  Major | PySpark | Erik Selin | Erik Selin |
| [SPARK-12265](https://issues.apache.org/jira/browse/SPARK-12265) | Spark calls System.exit inside driver instead of throwing exception |  Major | Mesos | Iulian Dragos | Nilanjan Raychaudhuri |
| [SPARK-12232](https://issues.apache.org/jira/browse/SPARK-12232) | Create new R API for read.table to avoid conflict |  Minor | SparkR | Felix Cheung | Felix Cheung |
| [SPARK-12231](https://issues.apache.org/jira/browse/SPARK-12231) | Failed to generate predicate Error when using dropna |  Major | PySpark, SQL | yahsuan, chang | kevin yu |
| [SPARK-12230](https://issues.apache.org/jira/browse/SPARK-12230) | WeightedLeastSquares.fit() should handle division by zero properly if standard deviation of target variable is zero. |  Trivial | ML | Imran Younus | Imran Younus |
| [SPARK-12222](https://issues.apache.org/jira/browse/SPARK-12222) | deserialize RoaringBitmap using Kryo serializer throw Buffer underflow exception |  Major | Spark Core | Fei Wang | Fei Wang |
| [SPARK-12218](https://issues.apache.org/jira/browse/SPARK-12218) | Invalid splitting of nested AND expressions in Data Source filter API |  Blocker | SQL | Irakli Machabeli | Yin Huai |
| [SPARK-12186](https://issues.apache.org/jira/browse/SPARK-12186) | stage web URI will redirect to the wrong location if it is the first URI from the application to be requested from the history server |  Minor | Web UI | Rohit Agarwal | Rohit Agarwal |
| [SPARK-12168](https://issues.apache.org/jira/browse/SPARK-12168) | Need test for conflicted function in R |  Minor | SparkR | Felix Cheung | Felix Cheung |
| [SPARK-12158](https://issues.apache.org/jira/browse/SPARK-12158) | [R] [SQL] Fix 'sample' functions that break R unit test cases |  Critical | SparkR, SQL | Xiao Li | Xiao Li |
| [SPARK-12153](https://issues.apache.org/jira/browse/SPARK-12153) | Word2Vec uses a fixed length for sentences which is not reasonable for reality, and similarity functions and fields are not accessible |  Minor | MLlib | YongGang Cao | YongGang Cao |
| [SPARK-12142](https://issues.apache.org/jira/browse/SPARK-12142) | Can't request executor when container allocator is not ready |  Major | Spark Core | meiyoula | meiyoula |
| [SPARK-12136](https://issues.apache.org/jira/browse/SPARK-12136) | rddToFileName does not properly handle prefix and suffix parameters |  Minor | Streaming | Brian Webb | Bo Meng |
| [SPARK-12132](https://issues.apache.org/jira/browse/SPARK-12132) | Cltr-C should clear current line in pyspark shell |  Major | PySpark | Davies Liu | Davies Liu |
| [SPARK-12131](https://issues.apache.org/jira/browse/SPARK-12131) | Cannot create ExpressionEncoder for Array[T] where T is a nested class |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12112](https://issues.apache.org/jira/browse/SPARK-12112) | Upgrade to SBT 0.13.9 |  Major | Build | Josh Rosen | Josh Rosen |
| [SPARK-12109](https://issues.apache.org/jira/browse/SPARK-12109) | Expressions's simpleString should delegate to its toString |  Major | SQL | Yin Huai | Yin Huai |
| [SPARK-12107](https://issues.apache.org/jira/browse/SPARK-12107) | Update spark-ec2 versions |  Minor | EC2 | Nicholas Chammas | Nicholas Chammas |
| [SPARK-12104](https://issues.apache.org/jira/browse/SPARK-12104) | collect() does not handle multiple columns with same name |  Critical | SparkR | Hossein Falaki | Sun Rui |
| [SPARK-12102](https://issues.apache.org/jira/browse/SPARK-12102) | Cast a non-nullable struct field to a nullable field during analysis |  Major | SQL | Yin Huai | Dilip Biswal |
| [SPARK-12091](https://issues.apache.org/jira/browse/SPARK-12091) | [PySpark] Removal of the JAVA-specific deserialized storage levels |  Minor | PySpark | Xiao Li | Xiao Li |
| [SPARK-12090](https://issues.apache.org/jira/browse/SPARK-12090) | Coalesce does not consider shuffle in PySpark |  Major | . | Davies Liu | Davies Liu |
| [SPARK-12088](https://issues.apache.org/jira/browse/SPARK-12088) | check connection.isClose before connection.getAutoCommit in JDBCRDD.close |  Minor | SQL | Huaxin Gao | Huaxin Gao |
| [SPARK-12084](https://issues.apache.org/jira/browse/SPARK-12084) | Fix codes that uses ByteBuffer.array incorrectly |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12082](https://issues.apache.org/jira/browse/SPARK-12082) | NettyBlockTransferSecuritySuite "security mismatch auth off on client" test is flaky |  Major | Tests | Josh Rosen | Josh Rosen |
| [SPARK-12062](https://issues.apache.org/jira/browse/SPARK-12062) | Master rebuilding historical SparkUI should be asynchronous |  Major | Deploy | Andrew Or | Bryan Cutler |
| [SPARK-12048](https://issues.apache.org/jira/browse/SPARK-12048) | JDBCRDD calls close() twice - SQLite then throws an exception |  Minor | SQL | R. H. | R. H. |
| [SPARK-12039](https://issues.apache.org/jira/browse/SPARK-12039) | HiveSparkSubmitSuite's SPARK-9757 Persist Parquet relation with decimal column is very flaky |  Major | SQL, Tests | Yin Huai | Yin Huai |
| [SPARK-12031](https://issues.apache.org/jira/browse/SPARK-12031) | Integer overflow when do sampling. |  Major | Spark Core | uncleGen | uncleGen |
| [SPARK-12028](https://issues.apache.org/jira/browse/SPARK-12028) | [SQL] get\_json\_object is unable to return a correct result for null literals |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-12026](https://issues.apache.org/jira/browse/SPARK-12026) | ChiSqTest gets slower and slower over time when number of features is large |  Major | MLlib | Hunter Kelly | yuhao yang |
| [SPARK-12019](https://issues.apache.org/jira/browse/SPARK-12019) | SparkR.init does not support character vector for sparkJars and sparkPackages |  Minor | SparkR | liushiqi9 | Felix Cheung |
| [SPARK-12010](https://issues.apache.org/jira/browse/SPARK-12010) | Spark JDBC requires support for column-name-free INSERT syntax |  Major | SQL | Christian Kurz | Christian Kurz |
| [SPARK-12006](https://issues.apache.org/jira/browse/SPARK-12006) | GaussianMixture.train crashes if an initial model is not None |  Major | MLlib, PySpark | Maciej Szymkiewicz | Maciej Szymkiewicz |
| [SPARK-12003](https://issues.apache.org/jira/browse/SPARK-12003) | Expanded star  should use field name as column name |  Major | . | Davies Liu | Davies Liu |
| [SPARK-12001](https://issues.apache.org/jira/browse/SPARK-12001) | StreamingContext cannot be completely stopped if the stop() call is interrupted |  Major | Streaming | Josh Rosen | Josh Rosen |
| [SPARK-11994](https://issues.apache.org/jira/browse/SPARK-11994) | Word2VecModel load and save cause SparkException when model is bigger than spark.kryoserializer.buffer.max |  Major | MLlib | Antonio Murgia | Antonio Murgia |
| [SPARK-11991](https://issues.apache.org/jira/browse/SPARK-11991) | spark\_ec2.py does not perform sanity checks on hostnames |  Major | EC2 | Jeremy Derr | Jeremy Derr |
| [SPARK-11972](https://issues.apache.org/jira/browse/SPARK-11972) | [Spark SQL] the value of 'hiveconf' parameter in CLI can't be got after enter spark-sql session |  Critical | SQL | Yi Zhou | Adrian Wang |
| [SPARK-11969](https://issues.apache.org/jira/browse/SPARK-11969) | SQL UI does not work with PySpark |  Critical | SQL | Davies Liu | Davies Liu |
| [SPARK-11956](https://issues.apache.org/jira/browse/SPARK-11956) | Test failures potentially related to SPARK-11140 |  Major | Spark Core | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-11832](https://issues.apache.org/jira/browse/SPARK-11832) | Spark shell does not work from sbt with scala 2.11 |  Minor | Spark Shell | Jakob Odersky | Jakob Odersky |
| [SPARK-11762](https://issues.apache.org/jira/browse/SPARK-11762) | TransportResponseHandler should consider open streams when counting outstanding requests |  Minor | Spark Core | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-11715](https://issues.apache.org/jira/browse/SPARK-11715) | R support corr for Column Aggregration |  Minor | SparkR | Felix Cheung | Felix Cheung |
| [SPARK-11627](https://issues.apache.org/jira/browse/SPARK-11627) | Spark Streaming backpressure mechanism  has no initial input rate limit,receivers receive data at the maximum speed , it might cause OOM exception |  Major | Streaming | junhaoMg | junhaoMg |
| [SPARK-11624](https://issues.apache.org/jira/browse/SPARK-11624) | Spark SQL CLI will set sessionstate twice |  Critical | SQL | Adrian Wang | Adrian Wang |
| [SPARK-11619](https://issues.apache.org/jira/browse/SPARK-11619) | cannot use UDTF in DataFrame.selectExpr |  Minor | SQL | Wenchen Fan | Dilip Biswal |
| [SPARK-11518](https://issues.apache.org/jira/browse/SPARK-11518) | The script spark-submit.cmd can not handle spark directory with space. |  Minor | Deploy, Windows | Cele Liu | Jon Maurer |
| [SPARK-11511](https://issues.apache.org/jira/browse/SPARK-11511) | Creating an InputDStream but not using it throws NPE |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-11500](https://issues.apache.org/jira/browse/SPARK-11500) | Not deterministic order of columns when using merging schemas. |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-11497](https://issues.apache.org/jira/browse/SPARK-11497) | PySpark RowMatrix Constructor Has Type Erasure Issue |  Minor | MLlib, PySpark | Mike Dusenberry | Mike Dusenberry |
| [SPARK-11394](https://issues.apache.org/jira/browse/SPARK-11394) | PostgreDialect cannot handle BYTE types |  Major | SQL | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-11218](https://issues.apache.org/jira/browse/SPARK-11218) | `./sbin/start-slave.sh --help` should print out the help message |  Minor | Deploy | Jacek Laskowski | Charles Yeh |
| [SPARK-11193](https://issues.apache.org/jira/browse/SPARK-11193) | Spark 1.5+ Kinesis Streaming - ClassCastException when starting KinesisReceiver |  Major | Streaming | Phil Kallos | Jean-Baptiste Onofré |
| [SPARK-11137](https://issues.apache.org/jira/browse/SPARK-11137) | Make StreamingContext.stop() exception-safe |  Minor | Streaming | Felix Cheung | Jayadevan M |
| [SPARK-11043](https://issues.apache.org/jira/browse/SPARK-11043) | Hive Thrift Server will log warn "Couldn't find log associated with operation handle" |  Major | SQL | SaintBacchus | SaintBacchus |
| [SPARK-10873](https://issues.apache.org/jira/browse/SPARK-10873) | Change history to use datatables to support sorting columns and searching |  Major | Web UI | Thomas Graves | Zhuo Liu |
| [SPARK-10847](https://issues.apache.org/jira/browse/SPARK-10847) | Pyspark - DataFrame - Optional Metadata with `None` triggers cryptic failure |  Minor | PySpark, SQL | Shea Parkes | Jason C Lee |
| [SPARK-10777](https://issues.apache.org/jira/browse/SPARK-10777) | order by fails when column is aliased and projection includes windowed aggregate |  Major | SQL | N Campbell | Xiao Li |
| [SPARK-10647](https://issues.apache.org/jira/browse/SPARK-10647) | Mesos HA mode misuses spark.deploy.zookeeper.dir property; configs should be documented |  Minor | Mesos | Alan Braithwaite | Timothy Chen |
| [SPARK-10582](https://issues.apache.org/jira/browse/SPARK-10582) | using dynamic-executor-allocation, if AM failed. the new AM will be started. But the new AM does not allocate executors to dirver |  Major | Spark Core | KaiXinXIaoLei | Saisai Shao |
| [SPARK-10524](https://issues.apache.org/jira/browse/SPARK-10524) | Decision tree binary classification with ordered categorical features: incorrect centroid |  Major | ML, MLlib | Joseph K. Bradley | Liang-Chi Hsieh |
| [SPARK-10116](https://issues.apache.org/jira/browse/SPARK-10116) | XORShiftRandom should generate uniform seeds |  Minor | Spark Core | Imran Rashid | Imran Rashid |
| [SPARK-9886](https://issues.apache.org/jira/browse/SPARK-9886) | Validate usages of Runtime.getRuntime.addShutdownHook |  Minor | Spark Core | Michel Lemay | Naveen Kumar Minchu |
| [SPARK-9844](https://issues.apache.org/jira/browse/SPARK-9844) | File appender race condition during SparkWorker shutdown |  Major | Spark Core | Alex Liu | Bryan Cutler |
| [SPARK-9026](https://issues.apache.org/jira/browse/SPARK-9026) | SimpleFutureAction.onComplete should not tie up a separate thread for each callback |  Major | Spark Core | Josh Rosen | Richard W. Eggert II |
| [SPARK-7780](https://issues.apache.org/jira/browse/SPARK-7780) | The intercept in LogisticRegressionWithLBFGS should not be regularized |  Major | MLlib | DB Tsai | holdenk |
| [SPARK-7615](https://issues.apache.org/jira/browse/SPARK-7615) | MLLIB Word2Vec wordVectors divided by Euclidean Norm equals to zero |  Minor | MLlib | Eric Li | Sean Owen |
| [SPARK-6847](https://issues.apache.org/jira/browse/SPARK-6847) | Stack overflow on updateStateByKey which followed by a dstream with checkpoint set |  Critical | Streaming | Jack Hu | Shixiong Zhu |
| [SPARK-4514](https://issues.apache.org/jira/browse/SPARK-4514) | SparkContext localProperties does not inherit property updates across thread reuse |  Critical | Spark Core | Erik Erlandson | Richard W. Eggert II |
| [SPARK-3650](https://issues.apache.org/jira/browse/SPARK-3650) | Triangle Count handles reverse edges incorrectly |  Critical | GraphX | Joseph E. Gonzalez | Robin East |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13302](https://issues.apache.org/jira/browse/SPARK-13302) | Cleanup persistence Docstests in ml |  Trivial | PySpark, Tests | holdenk | holdenk |
| [SPARK-13150](https://issues.apache.org/jira/browse/SPARK-13150) | Flaky test: org.apache.spark.sql.hive.thriftserver.SingleSessionSuite.test single session |  Major | SQL | Davies Liu | Herman van Hovell |
| [SPARK-12592](https://issues.apache.org/jira/browse/SPARK-12592) | TestHive.reset hides Spark testing logs |  Major | Tests | Cheng Lian | Cheng Lian |
| [SPARK-12560](https://issues.apache.org/jira/browse/SPARK-12560) | SqlTestUtils.stripSparkFilter needs to copy utf8strings |  Minor | SQL | Imran Rashid | Imran Rashid |
| [SPARK-12446](https://issues.apache.org/jira/browse/SPARK-12446) | Add unit tests for JDBCRDD internal functions |  Major | SQL | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-12236](https://issues.apache.org/jira/browse/SPARK-12236) | JDBC filter tests all pass if filters are not really pushed down |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-11694](https://issues.apache.org/jira/browse/SPARK-11694) | Parquet logical types are not being tested properly |  Minor | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-11677](https://issues.apache.org/jira/browse/SPARK-11677) | ORC filter tests all pass if filters are actually not pushed down. |  Critical | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-11676](https://issues.apache.org/jira/browse/SPARK-11676) | Parquet filter tests all pass if filters are not really pushed down |  Critical | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-10248](https://issues.apache.org/jira/browse/SPARK-10248) | DAGSchedulerSuite should check there were no errors in EventProcessLoop |  Major | Spark Core | Imran Rashid | Imran Rashid |
| [SPARK-5882](https://issues.apache.org/jira/browse/SPARK-5882) | Add a test for GraphLoader.edgeListFile |  Trivial | GraphX | Takeshi Yamamuro | Takeshi Yamamuro |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13426](https://issues.apache.org/jira/browse/SPARK-13426) | Remove the support of SIMR cluster manager |  Major | Scheduler, Spark Core | Saisai Shao | Saisai Shao |
| [SPARK-13420](https://issues.apache.org/jira/browse/SPARK-13420) | Rename Subquery logical plan to SubqueryAlias |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13413](https://issues.apache.org/jira/browse/SPARK-13413) | Remove SparkContext.metricsSystem |  Major | Spark Core | Reynold Xin | Reynold Xin |
| [SPARK-13381](https://issues.apache.org/jira/browse/SPARK-13381) | Support for loading CSV with a single function call |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-13306](https://issues.apache.org/jira/browse/SPARK-13306) | Initial implementation for uncorrelated scalar subquery |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-13296](https://issues.apache.org/jira/browse/SPARK-13296) | Move UserDefinedFunction into sql.expressions package |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13282](https://issues.apache.org/jira/browse/SPARK-13282) | LogicalPlan toSql should just return a String rather than Option[String] |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13263](https://issues.apache.org/jira/browse/SPARK-13263) | SQL generation support for tablesample |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-13261](https://issues.apache.org/jira/browse/SPARK-13261) | Expose maxCharactersPerColumn as a user configurable option |  Major | SQL | Hossein Falaki | Hossein Falaki |
| [SPARK-13236](https://issues.apache.org/jira/browse/SPARK-13236) | SQL generation support for Set Operations |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-13220](https://issues.apache.org/jira/browse/SPARK-13220) | Deprecate "yarn-client" and "yarn-cluster" |  Major | YARN | Andrew Or | Saisai Shao |
| [SPARK-13208](https://issues.apache.org/jira/browse/SPARK-13208) | Replace Pair with tuples |  Trivial | Examples, Spark Core, SQL, Streaming | Jakob Odersky | Jakob Odersky |
| [SPARK-13205](https://issues.apache.org/jira/browse/SPARK-13205) | SQL generation support for self join |  Major | SQL | Xiao Li | Xiao Li |
| [SPARK-13201](https://issues.apache.org/jira/browse/SPARK-13201) | Make a private non-deprecated version of setRuns |  Trivial | MLlib, PySpark | holdenk | holdenk |
| [SPARK-13200](https://issues.apache.org/jira/browse/SPARK-13200) | Investigate math.round on integer number in MFDataGenerator.scala:109 |  Minor | MLlib | holdenk | holdenk |
| [SPARK-13186](https://issues.apache.org/jira/browse/SPARK-13186) | Migrate away from SynchronizedMap which is deprecated |  Trivial | Spark Core, SQL, Streaming | holdenk | Huaxin Gao |
| [SPARK-13177](https://issues.apache.org/jira/browse/SPARK-13177) | Update ActorWordCount example to not directly use low level linked list as it is deprecated. |  Minor | Examples | holdenk | Sachin Aggarwal |
| [SPARK-13176](https://issues.apache.org/jira/browse/SPARK-13176) | Ignore deprecation warning for ProcessBuilder lines\_! |  Trivial | Spark Core | holdenk | Jakob Odersky |
| [SPARK-13172](https://issues.apache.org/jira/browse/SPARK-13172) | Stop using RichException.getStackTrace it is deprecated |  Trivial | Spark Core | holdenk | Sean Owen |
| [SPARK-13171](https://issues.apache.org/jira/browse/SPARK-13171) | Update promise & future to Promise and Future as the old ones are deprecated |  Trivial | . | holdenk | Jakob Odersky |
| [SPARK-13170](https://issues.apache.org/jira/browse/SPARK-13170) | Investigate replacing SynchronizedQueue as it is deprecated |  Trivial | Streaming, Tests | holdenk | Sean Owen |
| [SPARK-13166](https://issues.apache.org/jira/browse/SPARK-13166) | Remove DataStreamReader/Writer |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13165](https://issues.apache.org/jira/browse/SPARK-13165) | Replace deprecated synchronizedBuffer in streaming |  Trivial | Streaming | holdenk | holdenk |
| [SPARK-13164](https://issues.apache.org/jira/browse/SPARK-13164) | Replace deprecated synchronizedBuffer in core |  Minor | Spark Core | holdenk | holdenk |
| [SPARK-13149](https://issues.apache.org/jira/browse/SPARK-13149) | Add FileStreamSource |  Major | SQL | Shixiong Zhu | Shixiong Zhu |
| [SPARK-13137](https://issues.apache.org/jira/browse/SPARK-13137) | NullPoingException in schema inference for CSV when the first line is empty |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-13114](https://issues.apache.org/jira/browse/SPARK-13114) | java.lang.NegativeArraySizeException in CSV |  Critical | SQL | Davies Liu | Hyukjin Kwon |
| [SPARK-13091](https://issues.apache.org/jira/browse/SPARK-13091) | Rewrite/Propagate constraints for Aliases |  Major | SQL | Sameer Agarwal | Sameer Agarwal |
| [SPARK-13090](https://issues.apache.org/jira/browse/SPARK-13090) | Add initial support for constraint propagation in SparkSQL |  Major | SQL | Sameer Agarwal | Sameer Agarwal |
| [SPARK-13080](https://issues.apache.org/jira/browse/SPARK-13080) | Implementation of the internal catalog API using Hive |  Major | SQL | Reynold Xin | Andrew Or |
| [SPARK-13079](https://issues.apache.org/jira/browse/SPARK-13079) | Provide an in-memory implementation of the catalog API |  Major | SQL | Reynold Xin | Andrew Or |
| [SPARK-13078](https://issues.apache.org/jira/browse/SPARK-13078) | Create internal catalog API |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13076](https://issues.apache.org/jira/browse/SPARK-13076) | Rename ClientInterface to HiveClient |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-13045](https://issues.apache.org/jira/browse/SPARK-13045) | Clean up ColumnarBatch.Row and Column.Struct |  Minor | SQL | Nong Li | Nong Li |
| [SPARK-13043](https://issues.apache.org/jira/browse/SPARK-13043) | Support remaining types in ColumnarBatch |  Major | SQL | Nong Li | Nong Li |
| [SPARK-13037](https://issues.apache.org/jira/browse/SPARK-13037) | PySpark ml.recommendation support export/import |  Major | ML, PySpark | Yanbo Liang | Kai Jiang |
| [SPARK-13035](https://issues.apache.org/jira/browse/SPARK-13035) | PySpark ml.clustering support export/import |  Minor | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-13032](https://issues.apache.org/jira/browse/SPARK-13032) | Basic ML Pipeline export/import functions for PySpark |  Major | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-13018](https://issues.apache.org/jira/browse/SPARK-13018) | Replace example code in mllib-pmml-model-export.md using include\_example |  Minor | Documentation | Xusen Yin | Xin Ren |
| [SPARK-13016](https://issues.apache.org/jira/browse/SPARK-13016) | Replace example code in mllib-dimensionality-reduction.md using include\_example |  Minor | Documentation | Xusen Yin | Devaraj K |
| [SPARK-13012](https://issues.apache.org/jira/browse/SPARK-13012) | Replace example code in ml-guide.md using include\_example |  Minor | Documentation | Xusen Yin | Devaraj K |
| [SPARK-12995](https://issues.apache.org/jira/browse/SPARK-12995) | Remove deprecate APIs from GraphX |  Major | GraphX | Takeshi Yamamuro | Takeshi Yamamuro |
| [SPARK-12993](https://issues.apache.org/jira/browse/SPARK-12993) | Remove usage of ADD\_FILES in pyspark |  Minor | PySpark | Jeff Zhang | Jeff Zhang |
| [SPARK-12968](https://issues.apache.org/jira/browse/SPARK-12968) | Implement command to set current database |  Critical | SQL | Reynold Xin | Liang-Chi Hsieh |
| [SPARK-12938](https://issues.apache.org/jira/browse/SPARK-12938) | Bloom filter DataFrame API integration |  Major | SQL | Cheng Lian | Wenchen Fan |
| [SPARK-12937](https://issues.apache.org/jira/browse/SPARK-12937) | Bloom filter serialization |  Major | SQL | Cheng Lian | Wenchen Fan |
| [SPARK-12936](https://issues.apache.org/jira/browse/SPARK-12936) | Initial bloom filter implementation |  Major | SQL | Cheng Lian | Wenchen Fan |
| [SPARK-12935](https://issues.apache.org/jira/browse/SPARK-12935) | Count-min sketch DataFrame API integration |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12934](https://issues.apache.org/jira/browse/SPARK-12934) | Count-min sketch serialization |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12933](https://issues.apache.org/jira/browse/SPARK-12933) | Initial count-min sketch implementation |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12901](https://issues.apache.org/jira/browse/SPARK-12901) | Refector options to be correctly formed in a case class |  Minor | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12896](https://issues.apache.org/jira/browse/SPARK-12896) | Send only accumulator updates, not TaskMetrics, to the driver |  Major | Spark Core | Andrew Or | Andrew Or |
| [SPARK-12895](https://issues.apache.org/jira/browse/SPARK-12895) | Implement TaskMetrics using accumulators |  Major | Spark Core | Andrew Or | Andrew Or |
| [SPARK-12891](https://issues.apache.org/jira/browse/SPARK-12891) | Add support for complex types in ColumnarBatch |  Major | SQL | Nong Li | Nong Li |
| [SPARK-12889](https://issues.apache.org/jira/browse/SPARK-12889) | Rename ParserDialect -\> ParserInterface |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12887](https://issues.apache.org/jira/browse/SPARK-12887) | Do not expose var's in TaskMetrics |  Major | Spark Core | Andrew Or | Andrew Or |
| [SPARK-12885](https://issues.apache.org/jira/browse/SPARK-12885) | Rename 3 fields in ShuffleWriteMetrics |  Minor | Spark Core | Andrew Or | Andrew Or |
| [SPARK-12884](https://issues.apache.org/jira/browse/SPARK-12884) | Move \*Metrics and \*Accum\* classes to their own files |  Minor | Spark Core | Andrew Or | Andrew Or |
| [SPARK-12871](https://issues.apache.org/jira/browse/SPARK-12871) | Support to specify the option for compression codec. |  Major | SQL | Hyukjin Kwon | Hyukjin Kwon |
| [SPARK-12866](https://issues.apache.org/jira/browse/SPARK-12866) | Migrate the ExtendedHiveQlParser to the new parser |  Major | SQL | Herman van Hovell | Herman van Hovell |
| [SPARK-12865](https://issues.apache.org/jira/browse/SPARK-12865) | Migrate the SparkSQLParser to the new parser |  Major | SQL | Herman van Hovell | Herman van Hovell |
| [SPARK-12855](https://issues.apache.org/jira/browse/SPARK-12855) | Remove parser pluggability |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12850](https://issues.apache.org/jira/browse/SPARK-12850) | Support bucket pruning (predicate pushdown for bucketed tables) |  Major | SQL | Reynold Xin | Xiao Li |
| [SPARK-12848](https://issues.apache.org/jira/browse/SPARK-12848) | Parse numbers as decimals rather than doubles |  Major | SQL | Davies Liu | Herman van Hovell |
| [SPARK-12847](https://issues.apache.org/jira/browse/SPARK-12847) | Remove StreamingListenerBus and post all Streaming events to the same thread as Spark events |  Major | Spark Core, Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12833](https://issues.apache.org/jira/browse/SPARK-12833) | Initial import of databricks/spark-csv |  Major | SQL | Reynold Xin | Hossein Falaki |
| [SPARK-12830](https://issues.apache.org/jira/browse/SPARK-12830) | Java style: disallow trailing whitespaces |  Major | Build | Reynold Xin | Reynold Xin |
| [SPARK-12829](https://issues.apache.org/jira/browse/SPARK-12829) | Turn Java style checker on |  Major | Build | Reynold Xin | Reynold Xin |
| [SPARK-12819](https://issues.apache.org/jira/browse/SPARK-12819) | Deprecate TaskContext.isRunningLocally() |  Major | Spark Core | Josh Rosen | Josh Rosen |
| [SPARK-12813](https://issues.apache.org/jira/browse/SPARK-12813) | Eliminate serialization for back to back operations |  Critical | SQL | Michael Armbrust | Michael Armbrust |
| [SPARK-12799](https://issues.apache.org/jira/browse/SPARK-12799) | Simplify various string output for expressions |  Major | SQL | Reynold Xin | Cheng Lian |
| [SPARK-12791](https://issues.apache.org/jira/browse/SPARK-12791) | Simplify CaseWhen by breaking "branches" into "conditions" and "values" |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12790](https://issues.apache.org/jira/browse/SPARK-12790) | Remove HistoryServer old multiple files format |  Major | Deploy | Andrew Or | Felix Cheung |
| [SPARK-12771](https://issues.apache.org/jira/browse/SPARK-12771) | Improve code generation for CaseWhen |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12770](https://issues.apache.org/jira/browse/SPARK-12770) | Implement rules for branch elimination for CaseWhen in SimplifyConditionals |  Major | Optimizer, SQL | Reynold Xin | Reynold Xin |
| [SPARK-12768](https://issues.apache.org/jira/browse/SPARK-12768) | Remove CaseKeyWhen expression |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12762](https://issues.apache.org/jira/browse/SPARK-12762) | Add unit test for simplifying if expression |  Major | Optimizer, SQL | Reynold Xin | Reynold Xin |
| [SPARK-12756](https://issues.apache.org/jira/browse/SPARK-12756) | use hash expression in Exchange |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12728](https://issues.apache.org/jira/browse/SPARK-12728) | Integrate SQL generation feature with native view |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12725](https://issues.apache.org/jira/browse/SPARK-12725) | SQL generation suffers from name conficts introduced by some analysis rules |  Major | SQL | Cheng Lian | Xiao Li |
| [SPARK-12724](https://issues.apache.org/jira/browse/SPARK-12724) | SQL generation support for persisted data source relations |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12723](https://issues.apache.org/jira/browse/SPARK-12723) | Comprehensive SQL generation support for expressions |  Major | SQL | Cheng Lian | Xiao Li |
| [SPARK-12716](https://issues.apache.org/jira/browse/SPARK-12716) | Executor UI improvement suggestions - Totals |  Major | Web UI | Alex Bozarth | Alex Bozarth |
| [SPARK-12707](https://issues.apache.org/jira/browse/SPARK-12707) | Remove submit python/R scripts through pyspark/sparkR |  Major | Spark Submit | Jeff Zhang | Jeff Zhang |
| [SPARK-12706](https://issues.apache.org/jira/browse/SPARK-12706) | support grouping/grouping\_id function together group set |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12705](https://issues.apache.org/jira/browse/SPARK-12705) | Sorting column can't be resolved if it's not in projection |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12692](https://issues.apache.org/jira/browse/SPARK-12692) | Scala style: check no white space before comma |  Major | Project Infra | Kousuke Saruta | Kousuke Saruta |
| [SPARK-12689](https://issues.apache.org/jira/browse/SPARK-12689) | Migrate DDL parsing to the newly absorbed parser |  Major | SQL | Reynold Xin | Liang-Chi Hsieh |
| [SPARK-12687](https://issues.apache.org/jira/browse/SPARK-12687) | Support from clause surrounded by `()` |  Major | SQL | Davies Liu | Liang-Chi Hsieh |
| [SPARK-12681](https://issues.apache.org/jira/browse/SPARK-12681) | Split IdentifiersParser.g to avoid single huge java source |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12668](https://issues.apache.org/jira/browse/SPARK-12668) | Renaming CSV options to be similar to Pandas and R |  Major | SQL | Hossein Falaki | Hyukjin Kwon |
| [SPARK-12667](https://issues.apache.org/jira/browse/SPARK-12667) | Remove block manager's internal "external block store" API |  Major | Block Manager, Spark Core | Reynold Xin | Reynold Xin |
| [SPARK-12665](https://issues.apache.org/jira/browse/SPARK-12665) | Remove Vector, VectorSuite and GraphKryoRegistrator which are deprecated and no longer used |  Major | GraphX, Spark Core | Kousuke Saruta | Kousuke Saruta |
| [SPARK-12658](https://issues.apache.org/jira/browse/SPARK-12658) | Revert SPARK-12511 |  Major | PySpark | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12657](https://issues.apache.org/jira/browse/SPARK-12657) | Revert SPARK-12617 |  Major | PySpark | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12649](https://issues.apache.org/jira/browse/SPARK-12649) | support reading bucketed table |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12644](https://issues.apache.org/jira/browse/SPARK-12644) | Basic support for vectorize/batch Parquet decoding |  Major | SQL | Nong Li | Nong Li |
| [SPARK-12641](https://issues.apache.org/jira/browse/SPARK-12641) | Remove unused code related to Hadoop 0.23 |  Minor | Spark Core | Kousuke Saruta | Kousuke Saruta |
| [SPARK-12632](https://issues.apache.org/jira/browse/SPARK-12632) | Make Parameter Descriptions Consistent for PySpark MLlib FPM and Recommendation |  Trivial | Documentation, PySpark | Bryan Cutler | Bryan Cutler |
| [SPARK-12631](https://issues.apache.org/jira/browse/SPARK-12631) | Make Parameter Descriptions Consistent for PySpark MLlib Clustering |  Trivial | Documentation, PySpark | Bryan Cutler | Bryan Cutler |
| [SPARK-12630](https://issues.apache.org/jira/browse/SPARK-12630) | Make Parameter Descriptions Consistent for PySpark MLlib Classification |  Trivial | Documentation, PySpark | Bryan Cutler | Vijay Kiran |
| [SPARK-12627](https://issues.apache.org/jira/browse/SPARK-12627) | Remove SparkContext preferred locations constructor |  Blocker | Spark Core | Andrew Or | Reynold Xin |
| [SPARK-12618](https://issues.apache.org/jira/browse/SPARK-12618) | Clean up build warnings: 2.0.0 edition |  Minor | Spark Core, SQL, Streaming | Sean Owen | Sean Owen |
| [SPARK-12615](https://issues.apache.org/jira/browse/SPARK-12615) | Remove some deprecated APIs in RDD/SparkContext |  Major | Spark Core | Reynold Xin | Reynold Xin |
| [SPARK-12604](https://issues.apache.org/jira/browse/SPARK-12604) | Java count(AprroxDistinct)ByKey methods return Scala Long not Java |  Minor | Java API, Spark Core | Sean Owen | Sean Owen |
| [SPARK-12600](https://issues.apache.org/jira/browse/SPARK-12600) | Remove deprecated methods in SQL / DataFrames |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-12593](https://issues.apache.org/jira/browse/SPARK-12593) | Convert basic resolved logical plans back to SQL query strings |  Major | SQL | Cheng Lian | Cheng Lian |
| [SPARK-12588](https://issues.apache.org/jira/browse/SPARK-12588) | Remove HTTPBroadcast |  Major | Spark Core | Josh Rosen | Reynold Xin |
| [SPARK-12578](https://issues.apache.org/jira/browse/SPARK-12578) | Parser should not silently ignore the distinct keyword used in an aggregate function when OVER clause is used |  Major | SQL | Reynold Xin | Liang-Chi Hsieh |
| [SPARK-12577](https://issues.apache.org/jira/browse/SPARK-12577) | better support of parentheses in partition by and order by clause of window function's over clause |  Major | SQL | Reynold Xin | Liang-Chi Hsieh |
| [SPARK-12576](https://issues.apache.org/jira/browse/SPARK-12576) | Enable expression parsing (used in DataFrames) |  Major | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-12575](https://issues.apache.org/jira/browse/SPARK-12575) | Grammar parity with existing SQL parser |  Major | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-12574](https://issues.apache.org/jira/browse/SPARK-12574) | Move parser from hive module to catalyst (or sql-core) module |  Major | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-12573](https://issues.apache.org/jira/browse/SPARK-12573) | Add acknowledge that the parser was initially from Hive |  Major | SQL | Reynold Xin | Herman van Hovell |
| [SPARK-12572](https://issues.apache.org/jira/browse/SPARK-12572) | Initial import of the Hive parser |  Major | SQL | Reynold Xin | Nong Li |
| [SPARK-12568](https://issues.apache.org/jira/browse/SPARK-12568) | Add BINARY to Encoders |  Major | SQL | Michael Armbrust | Apache Spark |
| [SPARK-12561](https://issues.apache.org/jira/browse/SPARK-12561) | Remove JobLogger |  Major | Spark Core | Andrew Or | Reynold Xin |
| [SPARK-12539](https://issues.apache.org/jira/browse/SPARK-12539) | support writing bucketed table |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12495](https://issues.apache.org/jira/browse/SPARK-12495) | use true as default value for propagateNull in NewInstance |  Major | SQL | Wenchen Fan | Apache Spark |
| [SPARK-12481](https://issues.apache.org/jira/browse/SPARK-12481) | Remove usage of Hadoop deprecated APIs and reflection that supported 1.x |  Major | Spark Core, SQL, Streaming | Sean Owen | Sean Owen |
| [SPARK-12480](https://issues.apache.org/jira/browse/SPARK-12480) | add Hash expression that can calculate hash value for a group of expressions |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12456](https://issues.apache.org/jira/browse/SPARK-12456) | Add ExpressionDescription to misc functions |  Major | SQL | Yin Huai | Xiu (Joe) Guo |
| [SPARK-12414](https://issues.apache.org/jira/browse/SPARK-12414) | Remove closure serializer |  Major | Spark Core | Andrew Or | Sean Owen |
| [SPARK-12393](https://issues.apache.org/jira/browse/SPARK-12393) | Add read.text and write.text for SparkR |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12371](https://issues.apache.org/jira/browse/SPARK-12371) | Make sure non-nullable arguments of NewInstance don't receive null input data |  Major | SQL | Cheng Lian | Apache Spark |
| [SPARK-12342](https://issues.apache.org/jira/browse/SPARK-12342) | Corr (Pearson correlation) should be nullable |  Major | SQL | Cheng Lian | Davies Liu |
| [SPARK-12341](https://issues.apache.org/jira/browse/SPARK-12341) | The "comment" field of DESCRIBE result set should be nullable |  Minor | SQL | Cheng Lian | Davies Liu |
| [SPARK-12336](https://issues.apache.org/jira/browse/SPARK-12336) | Outer join using multiple columns results in wrong nullability |  Major | SQL | Cheng Lian | Davies Liu |
| [SPARK-12335](https://issues.apache.org/jira/browse/SPARK-12335) | CentralMomentAgg should be nullable |  Major | SQL | Cheng Lian | Davies Liu |
| [SPARK-12320](https://issues.apache.org/jira/browse/SPARK-12320) | throw exception if the number of fields does not line up for Tuple encoder |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12310](https://issues.apache.org/jira/browse/SPARK-12310) | Add write.json and write.parquet for SparkR |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12296](https://issues.apache.org/jira/browse/SPARK-12296) | Feature parity for pyspark.mllib StandardScalerModel |  Minor | MLlib, PySpark | Joseph K. Bradley | holdenk |
| [SPARK-12274](https://issues.apache.org/jira/browse/SPARK-12274) | WrapOption should not have type constraint for child |  Major | SQL | Wenchen Fan | Apache Spark |
| [SPARK-12252](https://issues.apache.org/jira/browse/SPARK-12252) | refactor MapObjects to make it less hacky |  Major | SQL | Wenchen Fan | Wenchen Fan |
| [SPARK-12247](https://issues.apache.org/jira/browse/SPARK-12247) | Documentation for spark.ml's ALS and collaborative filtering in general |  Major | Documentation, MLlib | Timothy Hunter | Benjamin Fradet |
| [SPARK-12215](https://issues.apache.org/jira/browse/SPARK-12215) | User guide section for KMeans in spark.ml |  Major | Documentation, ML | Joseph K. Bradley | Yu Ishikawa |
| [SPARK-12212](https://issues.apache.org/jira/browse/SPARK-12212) | Clarify the distinction between spark.mllib and spark.ml |  Major | Documentation | Timothy Hunter | Timothy Hunter |
| [SPARK-12199](https://issues.apache.org/jira/browse/SPARK-12199) | Follow-up: Refine example code in ml-features.md |  Major | Documentation | Xusen Yin | Xusen Yin |
| [SPARK-12174](https://issues.apache.org/jira/browse/SPARK-12174) | Slow test: BlockManagerSuite."SPARK-9591: getRemoteBytes from another location when Exception throw" |  Major | Tests | Josh Rosen | Josh Rosen |
| [SPARK-12152](https://issues.apache.org/jira/browse/SPARK-12152) | Speed up Scalastyle by only running one SBT command instead of four |  Major | Project Infra | Josh Rosen | Josh Rosen |
| [SPARK-12149](https://issues.apache.org/jira/browse/SPARK-12149) | Executor UI improvement suggestions - Color UI |  Major | Web UI | Alex Bozarth | Alex Bozarth |
| [SPARK-12146](https://issues.apache.org/jira/browse/SPARK-12146) | SparkR jsonFile should support multiple input files |  Major | SparkR | Yanbo Liang | Yanbo Liang |
| [SPARK-12041](https://issues.apache.org/jira/browse/SPARK-12041) | Add columnSimilarities to IndexedRowMatrix for PySpark |  Minor | MLlib, PySpark | Yanbo Liang | Kai Jiang |
| [SPARK-11978](https://issues.apache.org/jira/browse/SPARK-11978) | Move dataset\_example.py to examples/ml and rename to dataframe\_example.py |  Minor | ML, MLlib, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-11965](https://issues.apache.org/jira/browse/SPARK-11965) | Update user guide for RFormula feature interactions |  Major | Documentation, ML | Joseph K. Bradley | Yanbo Liang |
| [SPARK-11964](https://issues.apache.org/jira/browse/SPARK-11964) | Create user guide section explaining export/import |  Major | Documentation, ML | Joseph K. Bradley | Bill Chambers |
| [SPARK-11945](https://issues.apache.org/jira/browse/SPARK-11945) | Add computeCost to KMeansModel for PySpark spark.ml |  Minor | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-11944](https://issues.apache.org/jira/browse/SPARK-11944) | Python API for mllib.clustering.BisectingKMeans |  Minor | Documentation, ML, MLlib, PySpark | Yanbo Liang | holdenk |
| [SPARK-11925](https://issues.apache.org/jira/browse/SPARK-11925) | Add PySpark missing methods for ml.feature during Spark 1.6 QA |  Minor | ML, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-11923](https://issues.apache.org/jira/browse/SPARK-11923) | Python API for ml.feature.ChiSqSelector |  Minor | ML, PySpark | Yanbo Liang | Xusen Yin |
| [SPARK-11922](https://issues.apache.org/jira/browse/SPARK-11922) | Python API for ml.feature.QuantileDiscretizer |  Minor | ML, PySpark | Yanbo Liang | holdenk |
| [SPARK-11815](https://issues.apache.org/jira/browse/SPARK-11815) | PySpark DecisionTreeClassifier & DecisionTreeRegressor should support setSeed |  Minor | MLlib, PySpark | Yanbo Liang | Yanbo Liang |
| [SPARK-11807](https://issues.apache.org/jira/browse/SPARK-11807) | Remove support for Hadoop \< 2.2 (i.e. Hadoop 1 and 2.0) |  Major | Build | Reynold Xin | Reynold Xin |
| [SPARK-11608](https://issues.apache.org/jira/browse/SPARK-11608) | ML 1.6 QA: Programming guide update and migration guide |  Major | Documentation, ML, MLlib | Joseph K. Bradley | Joseph K. Bradley |
| [SPARK-11605](https://issues.apache.org/jira/browse/SPARK-11605) | ML 1.6 QA: API: Java compatibility, docs |  Major | Documentation, Java API, ML, MLlib | Joseph K. Bradley | yuhao yang |
| [SPARK-11602](https://issues.apache.org/jira/browse/SPARK-11602) | ML 1.6 QA: API: New Scala APIs, docs |  Major | Documentation, ML, MLlib | Joseph K. Bradley | yuhao yang |
| [SPARK-11563](https://issues.apache.org/jira/browse/SPARK-11563) | Use RpcEnv to transfer generated classes in spark-shell |  Major | Spark Shell | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-11314](https://issues.apache.org/jira/browse/SPARK-11314) | Add service API and test service for Yarn Cluster schedulers |  Major | YARN | Steve Loughran | Steve Loughran |
| [SPARK-11199](https://issues.apache.org/jira/browse/SPARK-11199) | Improve R context management story and add getOrCreate |  Minor | SparkR | Felix Cheung | Hossein Falaki |
| [SPARK-11140](https://issues.apache.org/jira/browse/SPARK-11140) | Replace file server in driver with RPC-based alternative |  Major | Spark Core | Marcelo Vanzin | Marcelo Vanzin |
| [SPARK-11097](https://issues.apache.org/jira/browse/SPARK-11097) | Add connection established callback to lower level RPC layer so we don't need to check for new connections in NettyRpcHandler.receive |  Major | Spark Core | Reynold Xin | Shixiong Zhu |
| [SPARK-11031](https://issues.apache.org/jira/browse/SPARK-11031) | SparkR str() method on DataFrame objects |  Major | SparkR | Oscar D. Lara Yejas | Oscar D. Lara Yejas |
| [SPARK-10820](https://issues.apache.org/jira/browse/SPARK-10820) | Initial infrastructure |  Major | SQL | Reynold Xin | Michael Armbrust |
| [SPARK-10814](https://issues.apache.org/jira/browse/SPARK-10814) | API design: convergence of batch and streaming DataFrame |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-10759](https://issues.apache.org/jira/browse/SPARK-10759) | Missing Python code example in model selection user guide |  Minor | Documentation, ML | Raela Wang | Jeremy |
| [SPARK-10580](https://issues.apache.org/jira/browse/SPARK-10580) | Remove Bagel |  Major | GraphX | Sean Owen | Reynold Xin |
| [SPARK-10264](https://issues.apache.org/jira/browse/SPARK-10264) | Add @Since annotation to ml.recoomendation |  Minor | Documentation, ML | Xiangrui Meng | Tijo Thomas |
| [SPARK-10263](https://issues.apache.org/jira/browse/SPARK-10263) | Add @Since annotation to ml.param and ml.\* |  Minor | Documentation, ML | Xiangrui Meng | Hiroshi Takahashi |
| [SPARK-9972](https://issues.apache.org/jira/browse/SPARK-9972) | Add `struct`, `encode` and `decode` function in SparkR |  Major | SparkR | Yu Ishikawa | Sun Rui |
| [SPARK-9694](https://issues.apache.org/jira/browse/SPARK-9694) | Add random seed Param to Scala CrossValidator |  Minor | ML | Joseph K. Bradley | Yanbo Liang |
| [SPARK-9690](https://issues.apache.org/jira/browse/SPARK-9690) | Add random seed Param to PySpark CrossValidator |  Minor | ML, PySpark | Martin Menestret | Martin Menestret |
| [SPARK-9622](https://issues.apache.org/jira/browse/SPARK-9622) | DecisionTreeRegressor: provide variance of prediction |  Minor | ML | Joseph K. Bradley | Yanbo Liang |
| [SPARK-9307](https://issues.apache.org/jira/browse/SPARK-9307) | Logging: Make it either stable or private[spark] |  Minor | Spark Core | Santiago M. Mola | Sean Owen |
| [SPARK-9297](https://issues.apache.org/jira/browse/SPARK-9297) | covar\_pop and covar\_samp aggregate functions |  Major | SQL | Yin Huai | Liang-Chi Hsieh |
| [SPARK-9057](https://issues.apache.org/jira/browse/SPARK-9057) | Add Scala, Java and Python example to show DStream.transform |  Major | Streaming | Tathagata Das | Jeff Lam |
| [SPARK-8641](https://issues.apache.org/jira/browse/SPARK-8641) | Native Spark Window Functions |  Major | SQL | Herman van Hovell | Herman van Hovell |
| [SPARK-7997](https://issues.apache.org/jira/browse/SPARK-7997) | Remove the developer api SparkEnv.actorSystem and AkkaUtils |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-7995](https://issues.apache.org/jira/browse/SPARK-7995) | Remove AkkaRpcEnv and remove Akka from the dependencies of Core |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-7994](https://issues.apache.org/jira/browse/SPARK-7994) | Remove "StreamingContext.actorStream" |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-7799](https://issues.apache.org/jira/browse/SPARK-7799) | Move "StreamingContext.actorStream" to a separate project and deprecate it in StreamingContext |  Major | Streaming | Shixiong Zhu | Shixiong Zhu |
| [SPARK-7689](https://issues.apache.org/jira/browse/SPARK-7689) | Remove TTL-based metadata cleaning (spark.cleaner.ttl) |  Major | Spark Core | Josh Rosen | Josh Rosen |
| [SPARK-7683](https://issues.apache.org/jira/browse/SPARK-7683) | Confusing behavior of fold function of RDD in pyspark |  Minor | PySpark | Ai He | Sean Owen |
| [SPARK-6761](https://issues.apache.org/jira/browse/SPARK-6761) | Approximate quantile |  Major | SQL | Reynold Xin | Liang-Chi Hsieh |
| [SPARK-6724](https://issues.apache.org/jira/browse/SPARK-6724) | Model import/export for FPGrowth |  Minor | MLlib | Joseph K. Bradley | Yanbo Liang |
| [SPARK-6518](https://issues.apache.org/jira/browse/SPARK-6518) | Add example code and user guide for bisecting k-means |  Major | Documentation, MLlib | Yu Ishikawa | Yu Ishikawa |
| [SPARK-6280](https://issues.apache.org/jira/browse/SPARK-6280) | Remove Akka systemName from Spark |  Major | Spark Core | Shixiong Zhu | Shixiong Zhu |
| [SPARK-4819](https://issues.apache.org/jira/browse/SPARK-4819) | Remove Guava's "Optional" from public API |  Major | Spark Core | Marcelo Vanzin | Sean Owen |
| [SPARK-3873](https://issues.apache.org/jira/browse/SPARK-3873) | Scala style: check import ordering |  Major | Project Infra | Reynold Xin | Marcelo Vanzin |
| [SPARK-3369](https://issues.apache.org/jira/browse/SPARK-3369) | Java mapPartitions Iterator-\>Iterable is inconsistent with Scala's Iterator-\>Iterator |  Major | Java API | Sean Owen | Sean Owen |
| [SPARK-2331](https://issues.apache.org/jira/browse/SPARK-2331) | SparkContext.emptyRDD should return RDD[T] not EmptyRDD[T] |  Minor | Spark Core | Ian Hummel | Reynold Xin |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [SPARK-13380](https://issues.apache.org/jira/browse/SPARK-13380) | Document Rand(seed) and Randn(seed) Return Indeterministic Results When Data Partitions are not fixed |  Minor | SQL | Xiao Li | Xiao Li |
| [SPARK-13350](https://issues.apache.org/jira/browse/SPARK-13350) | Configuration documentation incorrectly states that PYSPARK\_PYTHON's default is "python" |  Trivial | Documentation | Christopher Aycock | Christopher Aycock |
| [SPARK-13274](https://issues.apache.org/jira/browse/SPARK-13274) | Fix Aggregator Links on GroupedDataset Scala API |  Trivial | Documentation | Raela Wang | Raela Wang |
| [SPARK-13214](https://issues.apache.org/jira/browse/SPARK-13214) | Fix dynamic allocation docs |  Trivial | Documentation | Bill Chambers | Bill Chambers |
| [SPARK-13040](https://issues.apache.org/jira/browse/SPARK-13040) | JDBC using SPARK\_CLASSPATH is deprecated but is the only way documented |  Minor | Documentation, Examples | Sebastián Ramírez | Sebastián Ramírez |
| [SPARK-12983](https://issues.apache.org/jira/browse/SPARK-12983) | Correct metrics.properties.template |  Minor | Documentation, Spark Core | Benjamin Fradet | Benjamin Fradet |
| [SPARK-12894](https://issues.apache.org/jira/browse/SPARK-12894) | Add deploy instructions for Python in Kinesis integration doc |  Major | Documentation | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12814](https://issues.apache.org/jira/browse/SPARK-12814) | Add deploy instructions for Python in flume integration doc |  Major | Documentation | Shixiong Zhu | Shixiong Zhu |
| [SPARK-12786](https://issues.apache.org/jira/browse/SPARK-12786) | Actor demo does not demonstrate usable code |  Minor | Streaming | Brian London | Tathagata Das |
| [SPARK-12758](https://issues.apache.org/jira/browse/SPARK-12758) | Add note to Spark SQL Migration section about SPARK-11724 |  Minor | SQL | Brandon Bradley | Brandon Bradley |
| [SPARK-12722](https://issues.apache.org/jira/browse/SPARK-12722) | Typo in Spark Pipeline example |  Trivial | Documentation | Tom Chan | Jeff Lam |
| [SPARK-12703](https://issues.apache.org/jira/browse/SPARK-12703) | Spark KMeans Documentation Python Api |  Minor | MLlib | Anton | Joseph K. Bradley |
| [SPARK-12570](https://issues.apache.org/jira/browse/SPARK-12570) | DecisionTreeRegressor: provide variance of prediction: user guide update |  Minor | Documentation, ML | Joseph K. Bradley | Yanbo Liang |
| [SPARK-12507](https://issues.apache.org/jira/browse/SPARK-12507) | Expose closeFileAfterWrite and allowBatching configurations for Streaming |  Minor | Documentation, Streaming | Shixiong Zhu | Apache Spark |
| [SPARK-12351](https://issues.apache.org/jira/browse/SPARK-12351) | Add documentation of submitting Mesos jobs with cluster mode |  Major | . | Timothy Chen | Timothy Chen |
| [SPARK-12286](https://issues.apache.org/jira/browse/SPARK-12286) | Support UnsafeRow in all SparkPlan (if possible) |  Major | SQL | Davies Liu | Davies Liu |
| [SPARK-12217](https://issues.apache.org/jira/browse/SPARK-12217) | Document invalid handling for StringIndexer |  Minor | ML | Benjamin Fradet | Benjamin Fradet |
| [SPARK-12211](https://issues.apache.org/jira/browse/SPARK-12211) | Incorrect version number in graphx doc for migration from 1.1 |  Minor | Documentation, GraphX | Andrew Ray | Andrew Ray |
| [SPARK-12159](https://issues.apache.org/jira/browse/SPARK-12159) | Add user guide section for IndexToString transformer |  Minor | ML | Joseph K. Bradley | Benjamin Fradet |
| [SPARK-12093](https://issues.apache.org/jira/browse/SPARK-12093) | Fix the error of comment in DDLParser |  Trivial | Documentation | Yadong Qi | Yadong Qi |
| [SPARK-11476](https://issues.apache.org/jira/browse/SPARK-11476) | Incorrect function referred to in MLib Random data generation documentation |  Minor | Documentation | Jason Blochowiak | Sean Owen |
| [SPARK-9571](https://issues.apache.org/jira/browse/SPARK-9571) | Improve expression function coverage |  Major | SQL | Reynold Xin | Reynold Xin |
| [SPARK-5293](https://issues.apache.org/jira/browse/SPARK-5293) | Enable Spark user applications to use different versions of Akka |  Major | Spark Core | Reynold Xin | Shixiong Zhu |
| [SPARK-12640](https://issues.apache.org/jira/browse/SPARK-12640) | Add benchmarks to measure the speed ups of UnsafeRowParquetReaderReader. |  Minor | SQL | Nong Li | Nong Li |
| [SPARK-12465](https://issues.apache.org/jira/browse/SPARK-12465) | Remove spark.deploy.mesos.zookeeper.dir and use spark.deploy.zookeeper.dir |  Major | Mesos | Timothy Chen | Apache Spark |
| [SPARK-12464](https://issues.apache.org/jira/browse/SPARK-12464) | Remove spark.deploy.mesos.zookeeper.url and use spark.deploy.zookeeper.url |  Major | Mesos | Timothy Chen | Apache Spark |
| [SPARK-12463](https://issues.apache.org/jira/browse/SPARK-12463) | Remove spark.deploy.mesos.recoveryMode and use spark.deploy.recoveryMode |  Major | Mesos | Timothy Chen | Apache Spark |
| [SPARK-10620](https://issues.apache.org/jira/browse/SPARK-10620) | Look into whether accumulator mechanism can replace TaskMetrics |  Major | Spark Core | Patrick Wendell | Andrew Or |


