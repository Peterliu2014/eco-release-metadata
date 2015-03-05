# Hadoop Changelog

## Release 2.7.0 - 2015-03-05

### INCOMPATIBLE CHANGES:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11498](https://issues.apache.org/jira/browse/HADOOP-11498) | Bump the version of HTrace to 3.1.0-incubating |  Major |  | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11385](https://issues.apache.org/jira/browse/HADOOP-11385) | Prevent cross site scripting attack on JMXJSONServlet |  Critical |  | Haohui Mai | Haohui Mai |
| [HADOOP-11311](https://issues.apache.org/jira/browse/HADOOP-11311) | Restrict uppercase key names from being created with JCEKS |  Major | (security) | Andrew Wang | Andrew Wang |
| [HADOOP-10530](https://issues.apache.org/jira/browse/HADOOP-10530) | Make hadoop trunk build on Java7+ only |  Blocker | (build) | Steve Loughran | Steve Loughran |
| [HDFS-6651](https://issues.apache.org/jira/browse/HDFS-6651) | Deletion failure can leak inodes permanently |  Critical |  | Kihwal Lee | Jing Zhao |
| [HDFS-6252](https://issues.apache.org/jira/browse/HDFS-6252) | Phase out the old web UI in HDFS |  Minor | (namenode) | Fengdong Yu | Haohui Mai |


### NEW FEATURES:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11510](https://issues.apache.org/jira/browse/HADOOP-11510) | Expose truncate API via FileContext |  Major | (fs) | Yi Liu | Yi Liu |
| [HADOOP-11490](https://issues.apache.org/jira/browse/HADOOP-11490) | Expose truncate API via FileSystem and shell command |  Major | (fs) | Konstantin Shvachko | Milan Desai |
| [HADOOP-11341](https://issues.apache.org/jira/browse/HADOOP-11341) | KMS support for whitelist key ACLs |  Major | (kms , security) | Arun Suresh | Arun Suresh |
| [HADOOP-10728](https://issues.apache.org/jira/browse/HADOOP-10728) | Metrics system for Windows Azure Storage Filesystem |  Major | (tools) | Mike Liddell | Mike Liddell |
| [HADOOP-9629](https://issues.apache.org/jira/browse/HADOOP-9629) | Support Windows Azure Storage - Blob as a file system in Hadoop |  Major | (tools) | Mostafa Elhemali | Chris Nauroth |
| [HADOOP-8989](https://issues.apache.org/jira/browse/HADOOP-8989) | hadoop fs -find feature |  Major |  | Marco Nicosia | Jonathan Allen |
| [HADOOP-7984](https://issues.apache.org/jira/browse/HADOOP-7984) | Add hadoop --loglevel option to change log level |  Minor | (scripts) | Eli Collins | Akira AJISAKA |
| [HDFS-7584](https://issues.apache.org/jira/browse/HDFS-7584) | Enable Quota Support for Storage Types |  Major | (datanode , namenode) | Xiaoyu Yao | Xiaoyu Yao |
| [HDFS-7449](https://issues.apache.org/jira/browse/HDFS-7449) | Add metrics to NFS gateway |  Major | (nfs) | Brandon Li | Brandon Li |
| [HDFS-7424](https://issues.apache.org/jira/browse/HDFS-7424) | Add web UI for NFS gateway |  Major | (nfs) | Brandon Li | Brandon Li |
| [HDFS-7222](https://issues.apache.org/jira/browse/HDFS-7222) | Expose DataNode network errors as a metric |  Minor | (datanode) | Charles Lamb | Charles Lamb |
| [HDFS-6982](https://issues.apache.org/jira/browse/HDFS-6982) | nntop: top&#173;-like tool for name node users |  Major |  | Maysam Yabandeh | Maysam Yabandeh |
| [HDFS-6663](https://issues.apache.org/jira/browse/HDFS-6663) | Admin command to track file and locations from block id |  Major |  | Kihwal Lee | Chen He |
| [HDFS-3689](https://issues.apache.org/jira/browse/HDFS-3689) | Add support for variable length block |  Major | (datanode , hdfs-client , namenode) | Suresh Srinivas | Jing Zhao |
| [HDFS-3107](https://issues.apache.org/jira/browse/HDFS-3107) | HDFS truncate |  Major | (datanode , namenode) | Lei Chang | Plamen Jeliazkov |
| [HDFS-1362](https://issues.apache.org/jira/browse/HDFS-1362) | Provide volume management functionality for DataNode |  Major | (datanode) | Wang Xu | Wang Xu |
| [MAPREDUCE-6228](https://issues.apache.org/jira/browse/MAPREDUCE-6228) | Add truncate operation to SLive |  Major | (benchmarks , test) | Konstantin Shvachko | Plamen Jeliazkov |
| [MAPREDUCE-6227](https://issues.apache.org/jira/browse/MAPREDUCE-6227) | DFSIO for truncate |  Major | (benchmarks , test) | Konstantin Shvachko | Konstantin Shvachko |
| [YARN-2837](https://issues.apache.org/jira/browse/YARN-2837) | Timeline server needs to recover the timeline DT when restarting |  Blocker | (timelineserver) | Zhijie Shen | Zhijie Shen |
| [YARN-2574](https://issues.apache.org/jira/browse/YARN-2574) | Add support for FairScheduler to the ReservationSystem |  Major | (fairscheduler) | Subru Krishnan | Anubhav Dhoot |
| [YARN-2427](https://issues.apache.org/jira/browse/YARN-2427) | Add support for moving apps between queues in RM web services |  Major | (resourcemanager) | Varun Vasudev | Varun Vasudev |
| [YARN-2360](https://issues.apache.org/jira/browse/YARN-2360) | Fair Scheduler: Display dynamic fair share for queues on the scheduler page |  Major | (fairscheduler) | Ashwin Shankar | Ashwin Shankar |


### IMPROVEMENTS:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11658](https://issues.apache.org/jira/browse/HADOOP-11658) | Externalize io.compression.codecs property |  Minor |  | Kai Zheng | Kai Zheng |
| [HADOOP-11648](https://issues.apache.org/jira/browse/HADOOP-11648) | Set DomainSocketWatcher thread name explicitly |  Major | (net) | Liang Xie | Liang Xie |
| [HADOOP-11632](https://issues.apache.org/jira/browse/HADOOP-11632) | Cleanup Find.java to remove SupressWarnings annotations |  Minor |  | Akira AJISAKA | Akira AJISAKA |
| [HADOOP-11620](https://issues.apache.org/jira/browse/HADOOP-11620) | Add support for load balancing across a group of KMS for HA |  Major | (kms) | Arun Suresh | Arun Suresh |
| [HADOOP-11607](https://issues.apache.org/jira/browse/HADOOP-11607) | Reduce log spew in S3AFileSystem |  Trivial | (fs/s3) | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HADOOP-11599](https://issues.apache.org/jira/browse/HADOOP-11599) | Client#getTimeout should use IPC_CLIENT_PING_DEFAULT when IPC_CLIENT_PING_KEY is not configured. |  Minor | (ipc) | zhihai xu | zhihai xu |
| [HADOOP-11589](https://issues.apache.org/jira/browse/HADOOP-11589) | NetUtils.createSocketAddr should trim the input URI |  Minor | (net) | Akira AJISAKA | Rakesh R |
| [HADOOP-11586](https://issues.apache.org/jira/browse/HADOOP-11586) | Update use of Iterator to Iterable in AbstractMetricsContext.java |  Minor | (metrics) | Ray Chiang | Ray Chiang |
| [HADOOP-11579](https://issues.apache.org/jira/browse/HADOOP-11579) | Documentation for truncate |  Major | (documentation) | Steve Loughran | Konstantin Shvachko |
| [HADOOP-11569](https://issues.apache.org/jira/browse/HADOOP-11569) | Provide Merge API for MapFile to merge multiple similar MapFiles to one MapFile |  Major |  | Vinayakumar B | Vinayakumar B |
| [HADOOP-11544](https://issues.apache.org/jira/browse/HADOOP-11544) | Remove unused configuration keys for tracing |  Trivial |  | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11543](https://issues.apache.org/jira/browse/HADOOP-11543) | Improve help message for hadoop/yarn command |  Trivial | (scripts) | Jagadesh Kiran N | Brahma Reddy Battula |
| [HADOOP-11520](https://issues.apache.org/jira/browse/HADOOP-11520) | Clean incomplete multi-part uploads in S3A tests |  Minor | (fs/s3) | Thomas Demoor | Thomas Demoor |
| [HADOOP-11506](https://issues.apache.org/jira/browse/HADOOP-11506) | Configuration variable expansion regex expensive for long values |  Major | (conf) | Dmitriy V. Ryaboy | Gera Shegalov |
| [HADOOP-11495](https://issues.apache.org/jira/browse/HADOOP-11495) | Convert site documentation from apt to markdown |  Major | (documentation) | Allen Wittenauer | Masatake Iwasaki |
| [HADOOP-11483](https://issues.apache.org/jira/browse/HADOOP-11483) | HardLink.java should use the jdk7 createLink method |  Major |  | Colin Patrick McCabe | Akira AJISAKA |
| [HADOOP-11481](https://issues.apache.org/jira/browse/HADOOP-11481) | ClassCastException while using a key created by keytool to create encryption zone.  |  Minor |  | Yi Yao | Charles Lamb |
| [HADOOP-11464](https://issues.apache.org/jira/browse/HADOOP-11464) | Reinstate support for launching Hadoop processes on Windows using Cygwin. |  Major | (bin) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11455](https://issues.apache.org/jira/browse/HADOOP-11455) | KMS and Credential CLI should request confirmation for deletion by default |  Minor | (security) | Charles Lamb | Charles Lamb |
| [HADOOP-11448](https://issues.apache.org/jira/browse/HADOOP-11448) | Fix findbugs warnings in FileBasedIPList |  Minor |  | Akira AJISAKA | Tsuyoshi Ozawa |
| [HADOOP-11442](https://issues.apache.org/jira/browse/HADOOP-11442) | hadoop-azure: Create test jar |  Major | (tools) | shashank | shashank |
| [HADOOP-11441](https://issues.apache.org/jira/browse/HADOOP-11441) | Hadoop-azure: Change few methods scope to public |  Minor | (tools) | shashank | shashank |
| [HADOOP-11440](https://issues.apache.org/jira/browse/HADOOP-11440) | Use "test.build.data" instead of "build.test.dir" for testing in ClientBaseWithFixes |  Minor |  | Akira AJISAKA | Kengo Seki |
| [HADOOP-11430](https://issues.apache.org/jira/browse/HADOOP-11430) | Add GenericTestUtils#disableLog, GenericTestUtils#setLogLevel |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11427](https://issues.apache.org/jira/browse/HADOOP-11427) | ChunkedArrayList: fix removal via iterator and implement get |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11422](https://issues.apache.org/jira/browse/HADOOP-11422) | Check CryptoCodec is AES-CTR for Crypto input/output stream |  Minor |  | Yi Liu | Yi Liu |
| [HADOOP-11421](https://issues.apache.org/jira/browse/HADOOP-11421) | Add IOUtils#listDirectory |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11419](https://issues.apache.org/jira/browse/HADOOP-11419) | improve hadoop-maven-plugins |  Minor | (build) | Herv&#233; Boutemy | Herv&#233; Boutemy |
| [HADOOP-11416](https://issues.apache.org/jira/browse/HADOOP-11416) | Move ChunkedArrayList into hadoop-common |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11410](https://issues.apache.org/jira/browse/HADOOP-11410) | make the rpath of libhadoop.so configurable  |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11399](https://issues.apache.org/jira/browse/HADOOP-11399) | Java Configuration file and .xml files should be automatically cross-compared |  Minor |  | Ray Chiang | Ray Chiang |
| [HADOOP-11396](https://issues.apache.org/jira/browse/HADOOP-11396) | Provide navigation in the site documentation linking to the Hadoop Compatible File Systems. |  Major | (documentation) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11395](https://issues.apache.org/jira/browse/HADOOP-11395) | Add site documentation for Azure Storage FileSystem integration. |  Major | (documentation) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11390](https://issues.apache.org/jira/browse/HADOOP-11390) | Metrics 2 ganglia provider to include hostname in unresolved address problems |  Minor | (metrics) | Steve Loughran | Varun Saxena |
| [HADOOP-11323](https://issues.apache.org/jira/browse/HADOOP-11323) | WritableComparator#compare keeps reference to byte array |  Major | (performance) | Wilfred Spiegelenburg | Wilfred Spiegelenburg |
| [HADOOP-11313](https://issues.apache.org/jira/browse/HADOOP-11313) | Adding a document about NativeLibraryChecker |  Major | (documentation) | Tsuyoshi Ozawa | Tsuyoshi Ozawa |
| [HADOOP-11301](https://issues.apache.org/jira/browse/HADOOP-11301) | [optionally] update jmx cache to drop old metrics |  Major |  | Maysam Yabandeh | Maysam Yabandeh |
| [HADOOP-11291](https://issues.apache.org/jira/browse/HADOOP-11291) | Log the cause of SASL connection failures |  Minor | (security) | Stephen Chu | Stephen Chu |
| [HADOOP-11261](https://issues.apache.org/jira/browse/HADOOP-11261) | Set custom endpoint for S3A |  Major | (fs/s3) | Thomas Demoor | Thomas Demoor |
| [HADOOP-11257](https://issues.apache.org/jira/browse/HADOOP-11257) | Update "hadoop jar" documentation to warn against using it for launching yarn jars |  Major |  | Allen Wittenauer | Masatake Iwasaki |
| [HADOOP-11231](https://issues.apache.org/jira/browse/HADOOP-11231) | Remove dead code in ServletUtil |  Minor |  | Haohui Mai | Li Lu |
| [HADOOP-11188](https://issues.apache.org/jira/browse/HADOOP-11188) | hadoop-azure: automatically expand page blobs when they become full |  Major | (fs) | Eric Hanson | Eric Hanson |
| [HADOOP-11173](https://issues.apache.org/jira/browse/HADOOP-11173) | Improve error messages for some KeyShell commands |  Minor |  | Andrew Wang | Andrew Wang |
| [HADOOP-11172](https://issues.apache.org/jira/browse/HADOOP-11172) | Improve error message in Shell#runCommand on OutOfMemoryError |  Major |  | Yongjun Zhang | Yongjun Zhang |
| [HADOOP-11171](https://issues.apache.org/jira/browse/HADOOP-11171) | Enable using a proxy server to connect to S3a. |  Major | (fs/s3) | Thomas Demoor | Thomas Demoor |
| [HADOOP-11045](https://issues.apache.org/jira/browse/HADOOP-11045) | Introducing a tool to detect flaky tests of hadoop jenkins test job |  Major | (build , tools) | Yongjun Zhang | Yongjun Zhang |
| [HADOOP-11032](https://issues.apache.org/jira/browse/HADOOP-11032) | Replace use of Guava's Stopwatch with Hadoop's StopWatch |  Major |  | Gary Steelman | Tsuyoshi Ozawa |
| [HADOOP-10987](https://issues.apache.org/jira/browse/HADOOP-10987) | Provide an iterator-based listing API for FileSystem |  Major |  | Kihwal Lee | Kihwal Lee |
| [HADOOP-10976](https://issues.apache.org/jira/browse/HADOOP-10976) | moving the source code of hadoop-tools docs to the directory under hadoop-tools |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-10847](https://issues.apache.org/jira/browse/HADOOP-10847) | Remove the usage of sun.security.x509.* in testing code |  Minor | (security) | Kai Zheng | pascal oliva |
| [HADOOP-10809](https://issues.apache.org/jira/browse/HADOOP-10809) | hadoop-azure: page blob support |  Major | (tools) | Mike Liddell | Eric Hanson |
| [HADOOP-10786](https://issues.apache.org/jira/browse/HADOOP-10786) | Fix UGI#reloginFromKeytab on Java 8 |  Major | (security) | Tobi Vollebregt | Stephen Chu |
| [HADOOP-10626](https://issues.apache.org/jira/browse/HADOOP-10626) | Limit Returning Attributes for LDAP search |  Major | (security) | Jason Hubbard | Jason Hubbard |
| [HADOOP-10563](https://issues.apache.org/jira/browse/HADOOP-10563) | Remove the dependency of jsp in trunk |  Major |  | Haohui Mai | Haohui Mai |
| [HADOOP-10525](https://issues.apache.org/jira/browse/HADOOP-10525) | Remove DRFA.MaxBackupIndex config from log4j.properties |  Minor |  | Akira AJISAKA | Akira AJISAKA |
| [HADOOP-10140](https://issues.apache.org/jira/browse/HADOOP-10140) | Specification of HADOOP_CONF_DIR via the environment in hadoop_config.cmd |  Minor | (scripts) | Ian Jackson | Kiran Kumar M R |
| [HADOOP-9992](https://issues.apache.org/jira/browse/HADOOP-9992) | Modify the NN loadGenerator to optionally run as a MapReduce job |  Major | (test) | Akshay Radia | Akshay Radia |
| [HADOOP-9869](https://issues.apache.org/jira/browse/HADOOP-9869) |  Configuration.getSocketAddr()/getEnum() should use getTrimmed() |  Minor | (conf) | Steve Loughran | Tsuyoshi Ozawa |
| [HADOOP-8757](https://issues.apache.org/jira/browse/HADOOP-8757) | Metrics should disallow names with invalid characters |  Minor | (metrics) | Todd Lipcon | Ray Chiang |
| [HADOOP-4297](https://issues.apache.org/jira/browse/HADOOP-4297) | Enable Java assertions when running tests |  Major | (build) | Yoram Kulbak | Tsz Wo Nicholas Sze |
| [HDFS-7832](https://issues.apache.org/jira/browse/HDFS-7832) | Show 'Last Modified' in Namenode's 'Browse Filesystem' |  Major | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7808](https://issues.apache.org/jira/browse/HDFS-7808) | Remove obsolete -ns options in in DFSHAAdmin.java |  Minor |  | Arshad Mohammad | Arshad Mohammad |
| [HDFS-7797](https://issues.apache.org/jira/browse/HDFS-7797) | Add audit log for setQuota operation |  Major | (namenode) | Rakesh R | Rakesh R |
| [HDFS-7795](https://issues.apache.org/jira/browse/HDFS-7795) | Show warning if not all favored nodes were chosen by namenode |  Minor |  | Kihwal Lee | Kihwal Lee |
| [HDFS-7790](https://issues.apache.org/jira/browse/HDFS-7790) | Do not create optional fields in DFSInputStream unless they are needed |  Minor | (dfsclient) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7789](https://issues.apache.org/jira/browse/HDFS-7789) | DFSck should resolve the path to support cross-FS symlinks |  Major | (tools) | Gera Shegalov | Gera Shegalov |
| [HDFS-7780](https://issues.apache.org/jira/browse/HDFS-7780) | Update use of Iterator to Iterable in DataXceiverServer and SnapshotDiffInfo |  Minor |  | Ray Chiang | Ray Chiang |
| [HDFS-7773](https://issues.apache.org/jira/browse/HDFS-7773) | Additional metrics in HDFS to be accessed via jmx. |  Major | (datanode , namenode) | Anu Engineer | Anu Engineer |
| [HDFS-7772](https://issues.apache.org/jira/browse/HDFS-7772) | Document hdfs balancer -exclude/-include option in HDFSCommands.html |  Trivial | (documentation) | Xiaoyu Yao | Xiaoyu Yao |
| [HDFS-7771](https://issues.apache.org/jira/browse/HDFS-7771) | fuse_dfs should permit FILE: on the front of KRB5CCNAME |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7761](https://issues.apache.org/jira/browse/HDFS-7761) | cleanup unnecssary code logic in LocatedBlock |  Minor |  | Yi Liu | Yi Liu |
| [HDFS-7757](https://issues.apache.org/jira/browse/HDFS-7757) | Misleading error messages in FSImage.java |  Major | (namenode) | Arpit Agarwal | Brahma Reddy Battula |
| [HDFS-7752](https://issues.apache.org/jira/browse/HDFS-7752) | Improve description for "dfs.namenode.num.extra.edits.retained" and "dfs.namenode.num.checkpoints.retained" properties on hdfs-default.xml |  Minor | (documentation) | Wellington Chevreuil | Wellington Chevreuil |
| [HDFS-7743](https://issues.apache.org/jira/browse/HDFS-7743) | Code cleanup of BlockInfo and rename BlockInfo to BlockInfoContiguous |  Minor | (namenode) | Jing Zhao | Jing Zhao |
| [HDFS-7732](https://issues.apache.org/jira/browse/HDFS-7732) | Fix the order of the parameters in DFSConfigKeys |  Trivial |  | Akira AJISAKA | Brahma Reddy Battula |
| [HDFS-7710](https://issues.apache.org/jira/browse/HDFS-7710) | Remove dead code in BackupImage.java |  Minor |  | Xiaoyu Yao | Xiaoyu Yao |
| [HDFS-7706](https://issues.apache.org/jira/browse/HDFS-7706) | Switch BlockManager logging to use slf4j |  Minor | (namenode) | Andrew Wang | Andrew Wang |
| [HDFS-7703](https://issues.apache.org/jira/browse/HDFS-7703) | Support favouredNodes for the append for new blocks |  Major |  | Vinayakumar B | Vinayakumar B |
| [HDFS-7694](https://issues.apache.org/jira/browse/HDFS-7694) | FSDataInputStream should support "unbuffer" |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7685](https://issues.apache.org/jira/browse/HDFS-7685) | Document dfs.namenode.heartbeat.recheck-interval in hdfs-default.xml |  Minor | (documentation) | Frank Lanitz | Kai Sasaki |
| [HDFS-7684](https://issues.apache.org/jira/browse/HDFS-7684) | The host:port settings of the daemons should be trimmed before use |  Major |  | Tianyin Xu | Anu Engineer |
| [HDFS-7683](https://issues.apache.org/jira/browse/HDFS-7683) | Combine usages and percent stats in NameNode UI |  Minor | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7675](https://issues.apache.org/jira/browse/HDFS-7675) | Remove unused member DFSClient#spanReceiverHost |  Trivial | (dfsclient) | Konstantin Shvachko | Colin Patrick McCabe |
| [HDFS-7668](https://issues.apache.org/jira/browse/HDFS-7668) | Convert site documentation from apt to markdown |  Major | (documentation) | Allen Wittenauer | Masatake Iwasaki |
| [HDFS-7640](https://issues.apache.org/jira/browse/HDFS-7640) | print NFS Client in the NFS log |  Trivial | (nfs) | Brandon Li | Brandon Li |
| [HDFS-7604](https://issues.apache.org/jira/browse/HDFS-7604) | Track and display failed DataNode storage locations in NameNode. |  Major | (datanode , namenode) | Chris Nauroth | Chris Nauroth |
| [HDFS-7600](https://issues.apache.org/jira/browse/HDFS-7600) | Refine hdfs admin classes to reuse common code |  Major | (tools) | Yi Liu | Jing Zhao |
| [HDFS-7598](https://issues.apache.org/jira/browse/HDFS-7598) | Remove dependency on old version of Guava in TestDFSClientCache#testEviction |  Minor | (test) | Sangjin Lee | Sangjin Lee |
| [HDFS-7591](https://issues.apache.org/jira/browse/HDFS-7591) | hdfs classpath command should support same options as hadoop classpath. |  Minor | (scripts) | Chris Nauroth | Varun Saxena |
| [HDFS-7579](https://issues.apache.org/jira/browse/HDFS-7579) | Improve log reporting during block report rpc failure |  Minor | (datanode) | Charles Lamb | Charles Lamb |
| [HDFS-7564](https://issues.apache.org/jira/browse/HDFS-7564) | NFS gateway dynamically reload UID/GID mapping file /etc/nfs.map |  Minor | (nfs) | Hari Sekhon | Yongjun Zhang |
| [HDFS-7557](https://issues.apache.org/jira/browse/HDFS-7557) | Fix spacing for a few keys in DFSConfigKeys.java |  Minor |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7555](https://issues.apache.org/jira/browse/HDFS-7555) | Remove the support of unmanaged connectors in HttpServer2 |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7537](https://issues.apache.org/jira/browse/HDFS-7537) | fsck is confusing when dfs.namenode.replication.min &gt; 1 &amp;&amp; missing replicas &amp;&amp; NN restart |  Major | (namenode) | Allen Wittenauer | GAO Rui |
| [HDFS-7535](https://issues.apache.org/jira/browse/HDFS-7535) | Utilize Snapshot diff report for distcp |  Major | (distcp , snapshots) | Jing Zhao | Jing Zhao |
| [HDFS-7531](https://issues.apache.org/jira/browse/HDFS-7531) | Improve the concurrent access on FsVolumeList |  Major | (datanode) | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7513](https://issues.apache.org/jira/browse/HDFS-7513) | HDFS inotify: add defaultBlockSize to CreateEvent |  Major | (namenode) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7484](https://issues.apache.org/jira/browse/HDFS-7484) | Make FSDirectory#addINode take existing INodes as its parameter |  Major |  | Haohui Mai | Jing Zhao |
| [HDFS-7478](https://issues.apache.org/jira/browse/HDFS-7478) | Move org.apache.hadoop.hdfs.server.namenode.NNConf to FSNamesystem |  Major |  | Li Lu | Li Lu |
| [HDFS-7463](https://issues.apache.org/jira/browse/HDFS-7463) | Simplify FSNamesystem#getBlockLocationsUpdateTimes |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7458](https://issues.apache.org/jira/browse/HDFS-7458) | Add description to the nfs ports in core-site.xml used by nfs test to avoid confusion |  Minor | (nfs , test) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7454](https://issues.apache.org/jira/browse/HDFS-7454) | Reduce memory footprint for AclEntries in NameNode |  Major | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7446](https://issues.apache.org/jira/browse/HDFS-7446) | HDFS inotify should have the ability to determine what txid it has read up to |  Major | (dfsclient) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7439](https://issues.apache.org/jira/browse/HDFS-7439) | Add BlockOpResponseProto's message to DFSClient's exception message |  Minor | (balancer &amp; mover , datanode , hdfs-client) | Ming Ma | Takanobu Asanuma |
| [HDFS-7434](https://issues.apache.org/jira/browse/HDFS-7434) | DatanodeID hashCode should not be mutable |  Major | (namenode) | Daryn Sharp | Daryn Sharp |
| [HDFS-7430](https://issues.apache.org/jira/browse/HDFS-7430) | Rewrite the BlockScanner to use O(1) memory and use multiple threads |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7426](https://issues.apache.org/jira/browse/HDFS-7426) | Change nntop JMX format to be a JSON blob |  Major | (namenode) | Andrew Wang | Andrew Wang |
| [HDFS-7419](https://issues.apache.org/jira/browse/HDFS-7419) | Improve error messages for DataNode hot swap drive feature |  Major | (datanode) | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7409](https://issues.apache.org/jira/browse/HDFS-7409) | Allow dead nodes to finish decommissioning if all files are fully replicated |  Minor |  | Andrew Wang | Andrew Wang |
| [HDFS-7404](https://issues.apache.org/jira/browse/HDFS-7404) | Remove o.a.h.hdfs.server.datanode.web.resources |  Major |  | Haohui Mai | Li Lu |
| [HDFS-7398](https://issues.apache.org/jira/browse/HDFS-7398) | Reset cached thread-local FSEditLogOp's on every FSEditLog#logEdit |  Major | (namenode) | Gera Shegalov | Gera Shegalov |
| [HDFS-7386](https://issues.apache.org/jira/browse/HDFS-7386) | Replace check "port number &lt; 1024" with shared isPrivilegedPort method  |  Trivial | (datanode , security) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7384](https://issues.apache.org/jira/browse/HDFS-7384) | 'getfacl' command and 'getAclStatus' output should be in sync |  Major | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7381](https://issues.apache.org/jira/browse/HDFS-7381) | Decouple the management of block id and gen stamps from FSNamesystem |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7375](https://issues.apache.org/jira/browse/HDFS-7375) | Move FSClusterStats to o.a.h.h.hdfs.server.blockmanagement |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7365](https://issues.apache.org/jira/browse/HDFS-7365) | Remove hdfs.server.blockmanagement.MutableBlockCollection |  Minor |  | Li Lu | Li Lu |
| [HDFS-7357](https://issues.apache.org/jira/browse/HDFS-7357) | FSNamesystem.checkFileProgress should log file path |  Minor | (namenode) | Tsz Wo Nicholas Sze | Tsz Wo Nicholas Sze |
| [HDFS-7356](https://issues.apache.org/jira/browse/HDFS-7356) | Use DirectoryListing.hasMore() directly in nfs |  Minor | (nfs) | Haohui Mai | Li Lu |
| [HDFS-7336](https://issues.apache.org/jira/browse/HDFS-7336) | Unused member DFSInputStream.buffersize |  Major | (hdfs-client) | Konstantin Shvachko | Milan Desai |
| [HDFS-7335](https://issues.apache.org/jira/browse/HDFS-7335) | Redundant checkOperation() in FSN.analyzeFileState() |  Major | (namenode) | Konstantin Shvachko | Milan Desai |
| [HDFS-7333](https://issues.apache.org/jira/browse/HDFS-7333) | Improve log message in Storage.tryLock() |  Major | (datanode , namenode) | Konstantin Shvachko | Konstantin Shvachko |
| [HDFS-7331](https://issues.apache.org/jira/browse/HDFS-7331) | Add Datanode network counts to datanode jmx page |  Minor | (datanode) | Charles Lamb | Charles Lamb |
| [HDFS-7329](https://issues.apache.org/jira/browse/HDFS-7329) | MiniDFSCluster should log the exception when createNameNodesAndSetConf() fails. |  Major | (test) | Konstantin Shvachko | Byron Wong |
| [HDFS-7326](https://issues.apache.org/jira/browse/HDFS-7326) | Add documentation for hdfs debug commands |  Minor | (documentation) | Colin Patrick McCabe | Vijay Bhat |
| [HDFS-7323](https://issues.apache.org/jira/browse/HDFS-7323) | Move the get/setStoragePolicy commands out from dfsadmin |  Major | (hdfs-client) | Tsz Wo Nicholas Sze | Jing Zhao |
| [HDFS-7310](https://issues.apache.org/jira/browse/HDFS-7310) | Mover can give first priority to local DN if it has target storage type available in local DN |  Major | (balancer &amp; mover) | Uma Maheswara Rao G | Vinayakumar B |
| [HDFS-7308](https://issues.apache.org/jira/browse/HDFS-7308) | DFSClient write packet size may &gt; 64kB |  Minor | (hdfs-client) | Tsz Wo Nicholas Sze | Takuya Fukudome |
| [HDFS-7283](https://issues.apache.org/jira/browse/HDFS-7283) | Bump DataNode OOM log from WARN to ERROR |  Trivial | (datanode) | Stephen Chu | Stephen Chu |
| [HDFS-7280](https://issues.apache.org/jira/browse/HDFS-7280) | Use netty 4 in WebImageViewer |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7279](https://issues.apache.org/jira/browse/HDFS-7279) | Use netty to implement DatanodeWebHdfsMethods |  Major | (datanode , webhdfs) | Haohui Mai | Haohui Mai |
| [HDFS-7278](https://issues.apache.org/jira/browse/HDFS-7278) | Add a command that allows sysadmins to manually trigger full block reports from a DN |  Major | (datanode) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7270](https://issues.apache.org/jira/browse/HDFS-7270) | Add congestion signaling capability to DataNode write protocol |  Major | (datanode) | Haohui Mai | Haohui Mai |
| [HDFS-7266](https://issues.apache.org/jira/browse/HDFS-7266) | HDFS Peercache enabled check should not lock on object |  Minor | (hdfs-client) | Gopal V | Andrew Wang |
| [HDFS-7257](https://issues.apache.org/jira/browse/HDFS-7257) | Add the time of last HA state transition to NN's /jmx page |  Minor | (namenode) | Charles Lamb | Charles Lamb |
| [HDFS-7252](https://issues.apache.org/jira/browse/HDFS-7252) | small refinement to the use of isInAnEZ in FSNamesystem |  Trivial |  | Yi Liu | Yi Liu |
| [HDFS-7242](https://issues.apache.org/jira/browse/HDFS-7242) | Code improvement for FSN#checkUnreadableBySuperuser |  Minor | (namenode) | Yi Liu | Yi Liu |
| [HDFS-7223](https://issues.apache.org/jira/browse/HDFS-7223) | Tracing span description of IPC client is too long |  Minor |  | Masatake Iwasaki | Masatake Iwasaki |
| [HDFS-7210](https://issues.apache.org/jira/browse/HDFS-7210) | Avoid two separate RPC's namenode.append() and namenode.getFileInfo() for an append call from DFSClient |  Major | (hdfs-client , namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7190](https://issues.apache.org/jira/browse/HDFS-7190) | Bad use of Preconditions in startFileInternal() |  Major | (namenode) | Konstantin Shvachko | Dawson Choong |
| [HDFS-7186](https://issues.apache.org/jira/browse/HDFS-7186) | Document the "hadoop trace" command. |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [HDFS-7182](https://issues.apache.org/jira/browse/HDFS-7182) | JMX metrics aren't accessible when NN is busy |  Major |  | Ming Ma | Ming Ma |
| [HDFS-7165](https://issues.apache.org/jira/browse/HDFS-7165) | Separate block metrics for files with replication count 1 |  Major | (namenode) | Andrew Wang | Zhe Zhang |
| [HDFS-7026](https://issues.apache.org/jira/browse/HDFS-7026) | Introduce a string constant for "Failed to obtain user group info..." |  Trivial |  | Yongjun Zhang | Yongjun Zhang |
| [HDFS-6741](https://issues.apache.org/jira/browse/HDFS-6741) | Improve permission denied message when FSPermissionChecker#checkOwner fails |  Trivial |  | Stephen Chu | Harsh J |
| [HDFS-6735](https://issues.apache.org/jira/browse/HDFS-6735) | A minor optimization to avoid pread() be blocked by read() inside the same DFSInputStream |  Major | (hdfs-client) | Liang Xie | Lars Hofhansl |
| [HDFS-6565](https://issues.apache.org/jira/browse/HDFS-6565) | Use jackson instead jetty json in hdfs-client |  Major |  | Haohui Mai | Akira AJISAKA |
| [HDFS-6133](https://issues.apache.org/jira/browse/HDFS-6133) | Make Balancer support exclude specified path |  Major | (balancer &amp; mover , datanode) | zhaoyunjiong | zhaoyunjiong |
| [HDFS-5853](https://issues.apache.org/jira/browse/HDFS-5853) | Add "hadoop.user.group.metrics.percentiles.intervals" to hdfs-default.xml |  Minor | (documentation , namenode) | Akira AJISAKA | Akira AJISAKA |
| [HDFS-3342](https://issues.apache.org/jira/browse/HDFS-3342) | SocketTimeoutException in BlockSender.sendChunks could have a better error message |  Minor | (datanode) | Todd Lipcon | Yongjun Zhang |
| [HDFS-2219](https://issues.apache.org/jira/browse/HDFS-2219) | Fsck should work with fully qualified file paths. |  Minor | (tools) | Jitendra Nath Pandey | Tsz Wo Nicholas Sze |
| [HDFS-316](https://issues.apache.org/jira/browse/HDFS-316) | Balancer should run for a configurable # of iterations |  Minor | (balancer &amp; mover) | Brian Bockelman | Xiaoyu Yao |
| [MAPREDUCE-6267](https://issues.apache.org/jira/browse/MAPREDUCE-6267) | Refactor JobSubmitter#copyAndConfigureFiles into it's own class |  Minor |  | Chris Trezzo | Chris Trezzo |
| [MAPREDUCE-6256](https://issues.apache.org/jira/browse/MAPREDUCE-6256) | Removed unused private methods in o.a.h.mapreduce.Job.java |  Minor |  | Devaraj K | Naganarasimha G R |
| [MAPREDUCE-6255](https://issues.apache.org/jira/browse/MAPREDUCE-6255) | Fix JobCounter's format to use grouping separator |  Minor | (client) | Ryu Kobayashi | Ryu Kobayashi |
| [MAPREDUCE-6253](https://issues.apache.org/jira/browse/MAPREDUCE-6253) | Update use of Iterator to Iterable |  Minor |  | Ray Chiang | Ray Chiang |
| [MAPREDUCE-6248](https://issues.apache.org/jira/browse/MAPREDUCE-6248) | Allow users to get the MR job information for distcp |  Major | (distcp) | Jing Zhao | Jing Zhao |
| [MAPREDUCE-6194](https://issues.apache.org/jira/browse/MAPREDUCE-6194) | Bubble up final exception in failures during creation of output collectors |  Minor | (task) | Harsh J | Varun Saxena |
| [MAPREDUCE-6173](https://issues.apache.org/jira/browse/MAPREDUCE-6173) | Document the configuration of deploying MR over distributed cache with enabling wired encryption at the same time |  Major | (distributed-cache , documentation) | Junping Du | Junping Du |
| [MAPREDUCE-6169](https://issues.apache.org/jira/browse/MAPREDUCE-6169) | MergeQueue should release reference to the current item from key and value at the end of the iteration to save memory. |  Major | (mrv2) | zhihai xu | zhihai xu |
| [MAPREDUCE-6151](https://issues.apache.org/jira/browse/MAPREDUCE-6151) | Update document of GridMix |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [MAPREDUCE-6150](https://issues.apache.org/jira/browse/MAPREDUCE-6150) | Update document of Rumen |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [MAPREDUCE-6149](https://issues.apache.org/jira/browse/MAPREDUCE-6149) | Document override log4j.properties in MR job |  Major | (documentation) | Junping Du | Junping Du |
| [MAPREDUCE-6143](https://issues.apache.org/jira/browse/MAPREDUCE-6143) | add configuration for  mapreduce speculative execution in MR2 |  Major | (mrv2) | zhihai xu | zhihai xu |
| [MAPREDUCE-6141](https://issues.apache.org/jira/browse/MAPREDUCE-6141) | History server leveldb recovery store |  Major | (jobhistoryserver) | Jason Lowe | Jason Lowe |
| [MAPREDUCE-6059](https://issues.apache.org/jira/browse/MAPREDUCE-6059) | Speed up history server startup time |  Major |  | Siqi Li | Siqi Li |
| [MAPREDUCE-6046](https://issues.apache.org/jira/browse/MAPREDUCE-6046) | Change the class name for logs in RMCommunicator.java |  Minor | (mr-am) | Devaraj K | Sahil Takiar |
| [MAPREDUCE-5932](https://issues.apache.org/jira/browse/MAPREDUCE-5932) | Provide an option to use a dedicated reduce-side shuffle log |  Major | (mrv2) | Gera Shegalov | Gera Shegalov |
| [MAPREDUCE-5800](https://issues.apache.org/jira/browse/MAPREDUCE-5800) | Use Job#getInstance instead of deprecated constructors |  Minor |  | Akira AJISAKA | Akira AJISAKA |
| [MAPREDUCE-5612](https://issues.apache.org/jira/browse/MAPREDUCE-5612) | Add javadoc for TaskCompletionEvent.Status |  Minor | (documentation) | Sandy Ryza | Chris Palmer |
| [MAPREDUCE-5583](https://issues.apache.org/jira/browse/MAPREDUCE-5583) | Ability to limit running map and reduce tasks |  Major | (mr-am , mrv2) | Jason Lowe | Jason Lowe |
| [MAPREDUCE-5335](https://issues.apache.org/jira/browse/MAPREDUCE-5335) | Rename Job Tracker terminology in ShuffleSchedulerImpl |  Major | (applicationmaster) | Devaraj K | Devaraj K |
| [MAPREDUCE-4431](https://issues.apache.org/jira/browse/MAPREDUCE-4431) | mapred command should print the reason on killing already completed jobs |  Minor | (mrv2) | Nishan Shetty | Devaraj K |
| [YARN-3285](https://issues.apache.org/jira/browse/YARN-3285) | Convert branch-2 .apt.vm files of YARN to markdown |  Major | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [YARN-3272](https://issues.apache.org/jira/browse/YARN-3272) | Surface container locality info in RM web UI |  Major |  | Jian He | Jian He |
| [YARN-3262](https://issues.apache.org/jira/browse/YARN-3262) |  Surface application outstanding resource requests table in RM web UI |  Major | (yarn) | Jian He | Jian He |
| [YARN-3249](https://issues.apache.org/jira/browse/YARN-3249) | Add a "kill application" button to Resource Manager's Web UI |  Minor | (resourcemanager) | Ryu Kobayashi | Ryu Kobayashi |
| [YARN-3236](https://issues.apache.org/jira/browse/YARN-3236) | cleanup RMAuthenticationFilter#AUTH_HANDLER_PROPERTY. |  Trivial | (resourcemanager) | zhihai xu | zhihai xu |
| [YARN-3230](https://issues.apache.org/jira/browse/YARN-3230) | Clarify application states on the web UI |  Major |  | Jian He | Jian He |
| [YARN-3203](https://issues.apache.org/jira/browse/YARN-3203) | Correct a log message in AuxServices |  Minor |  | Brahma Reddy Battula | Brahma Reddy Battula |
| [YARN-3195](https://issues.apache.org/jira/browse/YARN-3195) | Add -help to yarn logs and nodes CLI command |  Minor | (client) | Jagadesh Kiran N | Jagadesh Kiran N |
| [YARN-3182](https://issues.apache.org/jira/browse/YARN-3182) | Cleanup switch statement in ApplicationMasterLauncher#handle() |  Minor |  | Ray Chiang | Ray Chiang |
| [YARN-3181](https://issues.apache.org/jira/browse/YARN-3181) | FairScheduler: Fix up outdated findbugs issues |  Major |  | Karthik Kambatla | Karthik Kambatla |
| [YARN-3179](https://issues.apache.org/jira/browse/YARN-3179) | Update use of Iterator to Iterable |  Minor |  | Ray Chiang | Ray Chiang |
| [YARN-3158](https://issues.apache.org/jira/browse/YARN-3158) | Correct log messages in ResourceTrackerService |  Major |  | Devaraj K | Varun Saxena |
| [YARN-3157](https://issues.apache.org/jira/browse/YARN-3157) | Refactor the exception handling in ConverterUtils#to*Id |  Minor | (resourcemanager) | Bibin A Chundatt | Bibin A Chundatt |
| [YARN-3147](https://issues.apache.org/jira/browse/YARN-3147) | Clean up RM web proxy code  |  Major | (webapp) | Steve Loughran | Steve Loughran |
| [YARN-3144](https://issues.apache.org/jira/browse/YARN-3144) | Configuration for making delegation token failures to timeline server not-fatal |  Major |  | Jonathan Eagles | Jonathan Eagles |
| [YARN-3123](https://issues.apache.org/jira/browse/YARN-3123) | Make YARN CLI show a single completed container even if the app is running |  Major | (client) | Zhijie Shen | Naganarasimha G R |
| [YARN-3108](https://issues.apache.org/jira/browse/YARN-3108) | ApplicationHistoryServer doesn't process -D arguments |  Major |  | Chang Li | Chang Li |
| [YARN-3100](https://issues.apache.org/jira/browse/YARN-3100) | Make YARN authorization pluggable |  Major |  | Jian He | Jian He |
| [YARN-3086](https://issues.apache.org/jira/browse/YARN-3086) | Make NodeManager memory configurable in MiniYARNCluster |  Minor | (test) | Robert Metzger | Robert Metzger |
| [YARN-3085](https://issues.apache.org/jira/browse/YARN-3085) | Application summary should include the application type |  Major | (resourcemanager) | Jason Lowe | Rohith |
| [YARN-3077](https://issues.apache.org/jira/browse/YARN-3077) | RM should create yarn.resourcemanager.zk-state-store.parent-path recursively |  Major | (resourcemanager) | Chun Chen | Chun Chen |
| [YARN-3056](https://issues.apache.org/jira/browse/YARN-3056) | add verification for containerLaunchDuration in TestNodeManagerMetrics. |  Trivial | (test) | zhihai xu | zhihai xu |
| [YARN-3022](https://issues.apache.org/jira/browse/YARN-3022) | Expose Container resource information from NodeManager for monitoring |  Major |  | Anubhav Dhoot | Anubhav Dhoot |
| [YARN-3005](https://issues.apache.org/jira/browse/YARN-3005) | [JDK7] Use switch statement for String instead of if-else statement in RegistrySecurity.java |  Trivial |  | Akira AJISAKA |  |
| [YARN-2996](https://issues.apache.org/jira/browse/YARN-2996) | Refine fs operations in FileSystemRMStateStore and few fixes |  Major | (resourcemanager) | Yi Liu | Yi Liu |
| [YARN-2957](https://issues.apache.org/jira/browse/YARN-2957) | Create unit test to automatically compare YarnConfiguration and yarn-default.xml |  Minor |  | Ray Chiang | Ray Chiang |
| [YARN-2950](https://issues.apache.org/jira/browse/YARN-2950) | Change message to mandate, not suggest JS requirement on UI |  Minor | (webapp) | Harsh J | Dustin Cote |
| [YARN-2940](https://issues.apache.org/jira/browse/YARN-2940) | Fix new findbugs warnings in rest of the hadoop-yarn components |  Major |  | Varun Saxena | Li Lu |
| [YARN-2939](https://issues.apache.org/jira/browse/YARN-2939) | Fix new findbugs warnings in hadoop-yarn-common |  Major |  | Varun Saxena | Li Lu |
| [YARN-2938](https://issues.apache.org/jira/browse/YARN-2938) | Fix new findbugs warnings in hadoop-yarn-resourcemanager and hadoop-yarn-applicationhistoryservice |  Major |  | Varun Saxena | Varun Saxena |
| [YARN-2937](https://issues.apache.org/jira/browse/YARN-2937) | Fix new findbugs warnings in hadoop-yarn-nodemanager |  Major |  | Varun Saxena | Varun Saxena |
| [YARN-2891](https://issues.apache.org/jira/browse/YARN-2891) | Failed Container Executor does not provide a clear error message |  Minor | (nodemanager) | Dustin Cote | Dustin Cote |
| [YARN-2878](https://issues.apache.org/jira/browse/YARN-2878) | Fix DockerContainerExecutor.apt.vm formatting |  Major | (documentation) | Abin Shahab | Abin Shahab |
| [YARN-2820](https://issues.apache.org/jira/browse/YARN-2820) |  Retry in FileSystemRMStateStore when FS's operations fail due to IOException. |  Major | (resourcemanager) | zhihai xu | zhihai xu |
| [YARN-2802](https://issues.apache.org/jira/browse/YARN-2802) | ClusterMetrics to include AM launch and register delays |  Major | (resourcemanager) | zhihai xu | zhihai xu |
| [YARN-2799](https://issues.apache.org/jira/browse/YARN-2799) | cleanup TestLogAggregationService based on the change in YARN-90 |  Minor | (test) | zhihai xu | zhihai xu |
| [YARN-2797](https://issues.apache.org/jira/browse/YARN-2797) | TestWorkPreservingRMRestart should use ParametrizedSchedulerTestBase |  Minor |  | Karthik Kambatla | Karthik Kambatla |
| [YARN-2780](https://issues.apache.org/jira/browse/YARN-2780) | Log aggregated resource allocation in rm-appsummary.log |  Minor | (resourcemanager) | Koji Noguchi | Eric Payne |
| [YARN-2679](https://issues.apache.org/jira/browse/YARN-2679) | Add metric for container launch duration |  Major | (nodemanager) | zhihai xu | zhihai xu |
| [YARN-2669](https://issues.apache.org/jira/browse/YARN-2669) | FairScheduler: queue names shouldn't allow periods |  Major |  | Wei Yan | Wei Yan |
| [YARN-2643](https://issues.apache.org/jira/browse/YARN-2643) | Don't create a new DominantResourceCalculator on every FairScheduler.allocate call |  Trivial |  | Sandy Ryza | Karthik Kambatla |
| [YARN-2641](https://issues.apache.org/jira/browse/YARN-2641) | Decommission nodes on -refreshNodes instead of next NM-RM heartbeat |  Major | (resourcemanager) | zhihai xu | zhihai xu |
| [YARN-2604](https://issues.apache.org/jira/browse/YARN-2604) | Scheduler should consider max-allocation-* in conjunction with the largest node |  Major | (scheduler) | Karthik Kambatla | Robert Kanter |
| [YARN-2301](https://issues.apache.org/jira/browse/YARN-2301) | Improve yarn container command |  Major |  | Jian He | Naganarasimha G R |
| [YARN-2254](https://issues.apache.org/jira/browse/YARN-2254) | TestRMWebServicesAppsModification should run against both CS and FS |  Minor |  | zhihai xu | zhihai xu |
| [YARN-2157](https://issues.apache.org/jira/browse/YARN-2157) | Document YARN metrics |  Major | (documentation) | Akira AJISAKA | Akira AJISAKA |
| [YARN-1582](https://issues.apache.org/jira/browse/YARN-1582) | Capacity Scheduler: add a maximum-allocation-mb setting per queue  |  Major | (capacityscheduler) | Thomas Graves | Thomas Graves |
| [YARN-1393](https://issues.apache.org/jira/browse/YARN-1393) | SLS: Add how-to-use instructions |  Major |  | Wei Yan | Wei Yan |
| [YARN-1299](https://issues.apache.org/jira/browse/YARN-1299) | Improve a log message in AppSchedulingInfo by adding application id |  Major | (resourcemanager) | Devaraj K |  |
| [YARN-1156](https://issues.apache.org/jira/browse/YARN-1156) | Enhance NodeManager AllocatedGB and AvailableGB metrics for aggregation of decimal values |  Major |  | Akira AJISAKA | Tsuyoshi Ozawa |


### BUG FIXES:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11674](https://issues.apache.org/jira/browse/HADOOP-11674) | oneByteBuf in CryptoInputStream and CryptoOutputStream should be non static |  Critical | (io) | Sean Busbey | Sean Busbey |
| [HADOOP-11666](https://issues.apache.org/jira/browse/HADOOP-11666) | Revert the format change of du output introduced by HADOOP-6857 |  Major |  | Akira AJISAKA | Byron Wong |
| [HADOOP-11634](https://issues.apache.org/jira/browse/HADOOP-11634) | Description of webhdfs' principal/keytab should switch places each other |  Major | (documentation) | Brahma Reddy Battula | Brahma Reddy Battula |
| [HADOOP-11629](https://issues.apache.org/jira/browse/HADOOP-11629) | WASB filesystem should not start BandwidthGaugeUpdater if fs.azure.skip.metrics set to true |  Major | (tools) | shanyu zhao | shanyu zhao |
| [HADOOP-11619](https://issues.apache.org/jira/browse/HADOOP-11619) | FTPFileSystem should override getDefaultPort |  Major | (fs) | Gera Shegalov | Brahma Reddy Battula |
| [HADOOP-11615](https://issues.apache.org/jira/browse/HADOOP-11615) | Update ServiceLevelAuth.md for YARN |  Minor | (documentation) | Akira AJISAKA | Brahma Reddy Battula |
| [HADOOP-11605](https://issues.apache.org/jira/browse/HADOOP-11605) | FilterFileSystem#create with ChecksumOpt should propagate it to wrapped FS |  Minor | (fs) | Gera Shegalov | Gera Shegalov |
| [HADOOP-11604](https://issues.apache.org/jira/browse/HADOOP-11604) | Prevent ConcurrentModificationException while closing domain sockets during shutdown of DomainSocketWatcher thread. |  Critical | (net) | Liang Xie | Chris Nauroth |
| [HADOOP-11595](https://issues.apache.org/jira/browse/HADOOP-11595) | Add default implementation for AbstractFileSystem#truncate |  Major | (fs) | Yi Liu | Yi Liu |
| [HADOOP-11587](https://issues.apache.org/jira/browse/HADOOP-11587) | TestMapFile#testMainMethodMapFile creates test files in hadoop-common project root |  Trivial | (test) | Xiaoyu Yao | Xiaoyu Yao |
| [HADOOP-11549](https://issues.apache.org/jira/browse/HADOOP-11549) | flaky test detection tool failed to handle special control characters in test result |  Major | (tools) | Yongjun Zhang | Yongjun Zhang |
| [HADOOP-11548](https://issues.apache.org/jira/browse/HADOOP-11548) | checknative should display a nicer error message when openssl support is not compiled in |  Major | (build , native) | Colin Patrick McCabe | Anu Engineer |
| [HADOOP-11547](https://issues.apache.org/jira/browse/HADOOP-11547) | hadoop-common native compilation fails on Windows due to missing support for __attribute__ declaration. |  Major | (native) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11546](https://issues.apache.org/jira/browse/HADOOP-11546) | Checkstyle failing: Unable to instantiate DoubleCheckedLockingCheck |  Major | (build) | Steve Loughran | Tsuyoshi Ozawa |
| [HADOOP-11545](https://issues.apache.org/jira/browse/HADOOP-11545) | ArrayIndexOutOfBoundsException is thrown with "hadoop credential list -provider" |  Minor | (security) | Brahma Reddy Battula | Brahma Reddy Battula |
| [HADOOP-11529](https://issues.apache.org/jira/browse/HADOOP-11529) | Fix findbugs warnings in hadoop-archives |  Minor | (tools) | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11526](https://issues.apache.org/jira/browse/HADOOP-11526) | Memory leak in Bzip2Compressor and Bzip2Decompressor |  Major | (io , native) | Ian Rogers | Anu Engineer |
| [HADOOP-11523](https://issues.apache.org/jira/browse/HADOOP-11523) | StorageException complaining " no lease ID" when updating FolderLastModifiedTime in WASB |  Major | (tools) | Duo Xu | Duo Xu |
| [HADOOP-11512](https://issues.apache.org/jira/browse/HADOOP-11512) | Use getTrimmedStrings when reading serialization keys |  Minor | (io) | Harsh J | Ryan P |
| [HADOOP-11509](https://issues.apache.org/jira/browse/HADOOP-11509) | change parsing sequence in GenericOptionsParser to parse -D parameters first |  Major |  | Xuan Gong | Xuan Gong |
| [HADOOP-11507](https://issues.apache.org/jira/browse/HADOOP-11507) | Hadoop RPC Authentication problem with different user locale |  Minor |  | Talat UYARER | Talat UYARER |
| [HADOOP-11500](https://issues.apache.org/jira/browse/HADOOP-11500) | InputStream is left unclosed in ApplicationClassLoader |  Major |  | Ted Yu | Ted Yu |
| [HADOOP-11499](https://issues.apache.org/jira/browse/HADOOP-11499) | Check of executorThreadsStarted in ValueQueue#submitRefillTask() evades lock acquisition |  Minor |  | Ted Yu | Ted Yu |
| [HADOOP-11497](https://issues.apache.org/jira/browse/HADOOP-11497) | Fix typo in ClusterSetup.html#Hadoop_Startup |  Major | (documentation) | Christian Winkler | Christian Winkler |
| [HADOOP-11494](https://issues.apache.org/jira/browse/HADOOP-11494) | Lock acquisition on WrappedInputStream#unwrappedRpcBuffer may race with another thread |  Minor |  | Ted Yu | Ted Yu |
| [HADOOP-11493](https://issues.apache.org/jira/browse/HADOOP-11493) | Fix some typos in kms-acls.xml description |  Trivial | (kms) | Charles Lamb | Charles Lamb |
| [HADOOP-11488](https://issues.apache.org/jira/browse/HADOOP-11488) | Difference in default connection timeout for S3A FS |  Minor | (fs/s3) | Harsh J | Daisuke Kobayashi |
| [HADOOP-11482](https://issues.apache.org/jira/browse/HADOOP-11482) | Use correct UGI when KMSClientProvider is called by a proxy user |  Major |  | Arun Suresh | Arun Suresh |
| [HADOOP-11480](https://issues.apache.org/jira/browse/HADOOP-11480) | Typo in hadoop-aws/index.md uses wrong scheme for test.fs.s3.name |  Minor | (documentation) | Ted Yu | Ted Yu |
| [HADOOP-11470](https://issues.apache.org/jira/browse/HADOOP-11470) | Remove some uses of obsolete guava APIs from the hadoop codebase |  Major |  | Sangjin Lee | Sangjin Lee |
| [HADOOP-11469](https://issues.apache.org/jira/browse/HADOOP-11469) | KMS should skip default.key.acl and whitelist.key.acl when loading key acl |  Minor | (kms) | Dian Fu | Dian Fu |
| [HADOOP-11467](https://issues.apache.org/jira/browse/HADOOP-11467) | KerberosAuthenticator can connect to a non-secure cluster |  Critical | (security) | Robert Kanter | Yongjun Zhang |
| [HADOOP-11462](https://issues.apache.org/jira/browse/HADOOP-11462) | TestSocketIOWithTimeout needs change for PowerPC platform |  Major | (test) | Ayappan | Ayappan |
| [HADOOP-11459](https://issues.apache.org/jira/browse/HADOOP-11459) | Fix recent findbugs in ActiveStandbyElector, NetUtils and ShellBasedIdMapping |  Minor |  | Vinayakumar B | Vinayakumar B |
| [HADOOP-11449](https://issues.apache.org/jira/browse/HADOOP-11449) | [JDK8] Cannot build on Windows: error: unexpected end tag: &lt;/ul&gt; |  Major | (build) | Alec Taylor | Chris Nauroth |
| [HADOOP-11446](https://issues.apache.org/jira/browse/HADOOP-11446) | S3AOutputStream should use shared thread pool to avoid OutOfMemoryError |  Major | (fs/s3) | Ted Yu | Ted Yu |
| [HADOOP-11445](https://issues.apache.org/jira/browse/HADOOP-11445) | Bzip2Codec: Data block is skipped when position of newly created stream is equal to start of split |  Critical |  | Ankit Kamboj | Ankit Kamboj |
| [HADOOP-11431](https://issues.apache.org/jira/browse/HADOOP-11431) | clean up redundant maven-site-plugin configuration |  Major |  | Herv&#233; Boutemy | Herv&#233; Boutemy |
| [HADOOP-11428](https://issues.apache.org/jira/browse/HADOOP-11428) | Remove obsolete reference to Cygwin in BUILDING.txt |  Major | (documentation) | Arpit Agarwal | Arpit Agarwal |
| [HADOOP-11420](https://issues.apache.org/jira/browse/HADOOP-11420) | Use latest maven-site-plugin and replace link to svn with link to git |  Trivial | (site) | Herv&#233; Boutemy | Herv&#233; Boutemy |
| [HADOOP-11414](https://issues.apache.org/jira/browse/HADOOP-11414) | FileBasedIPList#readLines() can leak file descriptors |  Minor |  | Ted Yu | Tsuyoshi Ozawa |
| [HADOOP-11412](https://issues.apache.org/jira/browse/HADOOP-11412) | POMs mention "The Apache Software License" rather than "Apache License" |  Trivial |  | Herv&#233; Boutemy | Herv&#233; Boutemy |
| [HADOOP-11411](https://issues.apache.org/jira/browse/HADOOP-11411) | Hive build failure on hadoop-2.7 due to HADOOP-11356 |  Major |  | Jason Dere |  |
| [HADOOP-11409](https://issues.apache.org/jira/browse/HADOOP-11409) | FileContext.getFileContext can stack overflow if default fs misconfigured |  Major |  | Jason Lowe | Gera Shegalov |
| [HADOOP-11403](https://issues.apache.org/jira/browse/HADOOP-11403) | Avoid using sys_errlist on Solaris, which lacks support for it |  Major |  | Malcolm Kavalsky | Malcolm Kavalsky |
| [HADOOP-11402](https://issues.apache.org/jira/browse/HADOOP-11402) | Negative user-to-group cache entries are never cleared for never-again-accessed users |  Major |  | Colin Patrick McCabe | Varun Saxena |
| [HADOOP-11400](https://issues.apache.org/jira/browse/HADOOP-11400) | GraphiteSink does not reconnect to Graphite after 'broken pipe' |  Major | (metrics) | Kamil Gorlo | Kamil Gorlo |
| [HADOOP-11394](https://issues.apache.org/jira/browse/HADOOP-11394) | hadoop-aws documentation missing. |  Major | (documentation) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11388](https://issues.apache.org/jira/browse/HADOOP-11388) | Remove deprecated o.a.h.metrics.file.FileContext |  Minor |  | Haohui Mai | Li Lu |
| [HADOOP-11386](https://issues.apache.org/jira/browse/HADOOP-11386) | Replace \n by %n in format hadoop-common format strings |  Major |  | Li Lu | Li Lu |
| [HADOOP-11368](https://issues.apache.org/jira/browse/HADOOP-11368) | Fix SSLFactory truststore reloader thread leak in KMSClientProvider |  Major | (kms) | Arun Suresh | Arun Suresh |
| [HADOOP-11363](https://issues.apache.org/jira/browse/HADOOP-11363) | Hadoop maven surefire-plugin uses must set heap size |  Major | (build) | Steve Loughran | Steve Loughran |
| [HADOOP-11355](https://issues.apache.org/jira/browse/HADOOP-11355) | When accessing data in HDFS and the key has been deleted, a Null Pointer Exception is shown. |  Minor |  | Arun Suresh | Arun Suresh |
| [HADOOP-11354](https://issues.apache.org/jira/browse/HADOOP-11354) | ThrottledInputStream doesn't perform effective throttling |  Major |  | Ted Yu | Ted Yu |
| [HADOOP-11350](https://issues.apache.org/jira/browse/HADOOP-11350) | The size of header buffer of HttpServer is too small when HTTPS is enabled |  Major | (security) | Benoy Antony | Benoy Antony |
| [HADOOP-11349](https://issues.apache.org/jira/browse/HADOOP-11349) | RawLocalFileSystem leaks file descriptor while creating a file if creat succeeds but chmod fails. |  Minor | (fs) | Chris Nauroth | Varun Saxena |
| [HADOOP-11348](https://issues.apache.org/jira/browse/HADOOP-11348) | Remove unused variable from CMake error message for finding openssl |  Minor |  | Dian Fu | Dian Fu |
| [HADOOP-11344](https://issues.apache.org/jira/browse/HADOOP-11344) | KMS kms-config.sh sets a default value for the keystore password even in non-ssl setup |  Major |  | Arun Suresh | Arun Suresh |
| [HADOOP-11343](https://issues.apache.org/jira/browse/HADOOP-11343) | Overflow is not properly handled in caclulating final iv for AES CTR |  Blocker | (security) | Jerry Chen | Jerry Chen |
| [HADOOP-11342](https://issues.apache.org/jira/browse/HADOOP-11342) | KMS key ACL should ignore ALL operation for default key ACL and whitelist key ACL |  Major | (kms , security) | Dian Fu | Dian Fu |
| [HADOOP-11337](https://issues.apache.org/jira/browse/HADOOP-11337) | KeyAuthorizationKeyProvider access checks need to be done atomically |  Major |  | Dian Fu | Dian Fu |
| [HADOOP-11333](https://issues.apache.org/jira/browse/HADOOP-11333) | Fix deadlock in DomainSocketWatcher when the notification pipe is full |  Major |  | zhaoyunjiong | zhaoyunjiong |
| [HADOOP-11332](https://issues.apache.org/jira/browse/HADOOP-11332) | KerberosAuthenticator#doSpnegoSequence should check if kerberos TGT is available in the subject  |  Major | (security) | Dian Fu | Dian Fu |
| [HADOOP-11329](https://issues.apache.org/jira/browse/HADOOP-11329) | Add JAVA_LIBRARY_PATH to KMS startup options |  Major | (kms , security) | Dian Fu | Arun Suresh |
| [HADOOP-11327](https://issues.apache.org/jira/browse/HADOOP-11327) | BloomFilter#not() omits the last bit, resulting in an incorrect filter |  Minor | (util) | Tim Luo | Eric Payne |
| [HADOOP-11322](https://issues.apache.org/jira/browse/HADOOP-11322) | key based ACL check in KMS always check KeyOpType.MANAGEMENT even actual KeyOpType is not MANAGEMENT  |  Major | (security) | Dian Fu | Dian Fu |
| [HADOOP-11321](https://issues.apache.org/jira/browse/HADOOP-11321) | copyToLocal cannot save a file to an SMB share unless the user has Full Control permissions. |  Major | (fs) | Chris Nauroth | Chris Nauroth |
| [HADOOP-11318](https://issues.apache.org/jira/browse/HADOOP-11318) | Update the document for hadoop fs -stat |  Major | (documentation) | Akira AJISAKA | Akira AJISAKA |
| [HADOOP-11316](https://issues.apache.org/jira/browse/HADOOP-11316) | "mvn package -Pdist,docs -DskipTests -Dtar" fails because of non-ascii characters |  Blocker |  | Tsuyoshi Ozawa | Tsuyoshi Ozawa |
| [HADOOP-11312](https://issues.apache.org/jira/browse/HADOOP-11312) | Fix unit tests to not use uppercase key names |  Major | (security) | Andrew Wang | Andrew Wang |
| [HADOOP-11309](https://issues.apache.org/jira/browse/HADOOP-11309) | System class pattern package.Foo should match package.Foo$Bar, too |  Blocker |  | Gera Shegalov | Gera Shegalov |
| [HADOOP-11300](https://issues.apache.org/jira/browse/HADOOP-11300) | KMS startup scripts must not display the keystore / truststore passwords |  Major | (kms) | Arun Suresh | Arun Suresh |
| [HADOOP-11295](https://issues.apache.org/jira/browse/HADOOP-11295) | RPC Server Reader thread can't shutdown if RPCCallQueue is full |  Major |  | Ming Ma | Ming Ma |
| [HADOOP-11294](https://issues.apache.org/jira/browse/HADOOP-11294) | Nfs3FileAttributes should not change the values of rdev, nlink and size in the constructor  |  Minor | (nfs) | Brandon Li | Brandon Li |
| [HADOOP-11289](https://issues.apache.org/jira/browse/HADOOP-11289) | Fix typo in RpcUtil log message |  Trivial | (net) | Charles Lamb | Charles Lamb |
| [HADOOP-11287](https://issues.apache.org/jira/browse/HADOOP-11287) | Simplify UGI#reloginFromKeytab for Java 7+ |  Major |  | Haohui Mai | Li Lu |
| [HADOOP-11283](https://issues.apache.org/jira/browse/HADOOP-11283) | Potentially unclosed SequenceFile.Writer in DistCpV1#setup() |  Minor |  | Ted Yu | Varun Saxena |
| [HADOOP-11273](https://issues.apache.org/jira/browse/HADOOP-11273) | TestMiniKdc failure: login options not compatible with IBM JDK |  Major | (test) | Gao Zhong Liang | Gao Zhong Liang |
| [HADOOP-11272](https://issues.apache.org/jira/browse/HADOOP-11272) | Allow ZKSignerSecretProvider and ZKDelegationTokenSecretManager to use the same curator client |  Major |  | Arun Suresh | Arun Suresh |
| [HADOOP-11271](https://issues.apache.org/jira/browse/HADOOP-11271) | Use Time.monotonicNow() in Shell.java instead of Time.now() |  Minor |  | Vinayakumar B | Vinayakumar B |
| [HADOOP-11269](https://issues.apache.org/jira/browse/HADOOP-11269) | Add java 8 profile for hadoop-annotations |  Major |  | Haohui Mai | Li Lu |
| [HADOOP-11268](https://issues.apache.org/jira/browse/HADOOP-11268) | Update BUILDING.txt to remove the workaround for tools.jar |  Minor |  | Haohui Mai | Li Lu |
| [HADOOP-11267](https://issues.apache.org/jira/browse/HADOOP-11267) | TestSecurityUtil fails when run with JDK8 because of empty principal names |  Minor | (security , test) | Stephen Chu | Stephen Chu |
| [HADOOP-11266](https://issues.apache.org/jira/browse/HADOOP-11266) | Remove no longer supported activation properties for packaging from pom |  Trivial | (build) | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11256](https://issues.apache.org/jira/browse/HADOOP-11256) | Some site docs have inconsistent appearance |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11248](https://issues.apache.org/jira/browse/HADOOP-11248) | Add hadoop configuration to disable Azure Filesystem metrics collection |  Major | (fs) | shanyu zhao | shanyu zhao |
| [HADOOP-11246](https://issues.apache.org/jira/browse/HADOOP-11246) | Move jenkins to Java 7 |  Major |  | Haohui Mai | Steve Loughran |
| [HADOOP-11236](https://issues.apache.org/jira/browse/HADOOP-11236) | NFS: Fix javadoc warning in RpcProgram.java |  Trivial | (documentation) | Abhiraj Butala | Abhiraj Butala |
| [HADOOP-11230](https://issues.apache.org/jira/browse/HADOOP-11230) | Add missing dependency of bouncycastle for kms, httpfs, hdfs, MR and YARN |  Major | (test) | Robert Kanter | Robert Kanter |
| [HADOOP-11213](https://issues.apache.org/jira/browse/HADOOP-11213) | Typos in html pages: SecureMode and EncryptedShuffle |  Minor |  | Wei Yan | Wei Yan |
| [HADOOP-11211](https://issues.apache.org/jira/browse/HADOOP-11211) | mapreduce.job.classloader.system.classes semantics should be order-independent |  Major |  | Yitong Zhou | Yitong Zhou |
| [HADOOP-11209](https://issues.apache.org/jira/browse/HADOOP-11209) | Configuration#updatingResource/finalParameters are not thread-safe |  Major | (conf) | Josh Rosen | Varun Saxena |
| [HADOOP-11201](https://issues.apache.org/jira/browse/HADOOP-11201) | Hadoop Archives should support globs resolving to files |  Blocker | (tools) | Gera Shegalov | Gera Shegalov |
| [HADOOP-11187](https://issues.apache.org/jira/browse/HADOOP-11187) | NameNode - KMS communication fails after a long period of inactivity |  Major |  | Arun Suresh | Arun Suresh |
| [HADOOP-11186](https://issues.apache.org/jira/browse/HADOOP-11186) | documentation should talk about hadoop.htrace.spanreceiver.classes, not hadoop.trace.spanreceiver.classes |  Minor |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HADOOP-11166](https://issues.apache.org/jira/browse/HADOOP-11166) | Remove ulimit from test-patch.sh |  Major |  | Andrew Wang | Andrew Wang |
| [HADOOP-11157](https://issues.apache.org/jira/browse/HADOOP-11157) | ZKDelegationTokenSecretManager never shuts down listenerThreadPool |  Major | (security) | Gregory Chanan | Arun Suresh |
| [HADOOP-11156](https://issues.apache.org/jira/browse/HADOOP-11156) | DelegateToFileSystem should implement getFsStatus(final Path f). |  Major | (fs) | zhihai xu | zhihai xu |
| [HADOOP-11039](https://issues.apache.org/jira/browse/HADOOP-11039) | ByteBufferReadable API doc is inconsistent with the implementations. |  Minor | (documentation) | Yi Liu | Yi Liu |
| [HADOOP-11008](https://issues.apache.org/jira/browse/HADOOP-11008) | Remove duplicated description about proxy-user in site documents |  Minor | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [HADOOP-11000](https://issues.apache.org/jira/browse/HADOOP-11000) | HAServiceProtocol's health state is incorrectly transitioned to SERVICE_NOT_RESPONDING |  Major |  | Ming Ma | Ming Ma |
| [HADOOP-10953](https://issues.apache.org/jira/browse/HADOOP-10953) | NetworkTopology#add calls NetworkTopology#toString without holding the netlock |  Minor | (net) | Liang Xie | Liang Xie |
| [HADOOP-10852](https://issues.apache.org/jira/browse/HADOOP-10852) | NetgroupCache is not thread-safe |  Major | (security) | Benoy Antony | Benoy Antony |
| [HADOOP-10840](https://issues.apache.org/jira/browse/HADOOP-10840) | Fix OutOfMemoryError caused by metrics system in Azure File System |  Major | (metrics) | shanyu zhao | shanyu zhao |
| [HADOOP-10748](https://issues.apache.org/jira/browse/HADOOP-10748) | HttpServer2 should not load JspServlet |  Major |  | Haohui Mai | Haohui Mai |
| [HADOOP-10717](https://issues.apache.org/jira/browse/HADOOP-10717) | HttpServer2 should load jsp DTD from local jars instead of going remote |  Blocker |  | Dapeng Sun | Dapeng Sun |
| [HADOOP-10714](https://issues.apache.org/jira/browse/HADOOP-10714) | AmazonS3Client.deleteObjects() need to be limited to 1000 entries per call |  Critical | (fs/s3) | David S. Wang | Juan Yu |
| [HADOOP-10690](https://issues.apache.org/jira/browse/HADOOP-10690) | Lack of synchronization on access to InputStream in NativeAzureFileSystem#NativeAzureFsInputStream#close() |  Minor | (tools) | Ted Yu | Chen He |
| [HADOOP-10689](https://issues.apache.org/jira/browse/HADOOP-10689) | InputStream is not closed in AzureNativeFileSystemStore#retrieve() |  Minor | (tools) | Ted Yu | Chen He |
| [HADOOP-10181](https://issues.apache.org/jira/browse/HADOOP-10181) | GangliaContext does not work with multicast ganglia setup |  Minor | (metrics) | Andrew Otto | Andrew Johnson |
| [HADOOP-10134](https://issues.apache.org/jira/browse/HADOOP-10134) | [JDK8] Fix Javadoc errors caused by incorrect or illegal tags in doc comments  |  Minor |  | Andrew Purtell | Andrew Purtell |
| [HADOOP-10062](https://issues.apache.org/jira/browse/HADOOP-10062) | race condition in MetricsSystemImpl#publishMetricsNow that causes incorrect results |  Major | (metrics) | Shinichi Yamashita | Sangjin Lee |
| [HADOOP-9922](https://issues.apache.org/jira/browse/HADOOP-9922) | hadoop windows native build will fail in 32 bit machine |  Major | (build , native) | Vinayakumar B | Kiran Kumar M R |
| [HADOOP-9907](https://issues.apache.org/jira/browse/HADOOP-9907) | Webapp http://hostname:port/metrics  link is not working  |  Critical |  | Jian He | Akira AJISAKA |
| [HADOOP-9137](https://issues.apache.org/jira/browse/HADOOP-9137) | Support connection limiting in IPC server |  Major |  | Sanjay Radia | Kihwal Lee |
| [HADOOP-9087](https://issues.apache.org/jira/browse/HADOOP-9087) | Queue size metric for metric sinks isn't actually maintained |  Minor | (metrics) | Mostafa Elhemali | Akira AJISAKA |
| [HADOOP-8642](https://issues.apache.org/jira/browse/HADOOP-8642) | Document that io.native.lib.available only controls native bz2 and zlib compression codecs |  Major | (documentation , native) | Eli Collins | Akira AJISAKA |
| [HADOOP-6221](https://issues.apache.org/jira/browse/HADOOP-6221) | RPC Client operations cannot be interrupted |  Minor | (ipc) | Steve Loughran | Steve Loughran |
| [HDFS-7879](https://issues.apache.org/jira/browse/HDFS-7879) | hdfs.dll does not export functions of the public libhdfs API |  Major | (build , libhdfs) | Chris Nauroth | Chris Nauroth |
| [HDFS-7871](https://issues.apache.org/jira/browse/HDFS-7871) | NameNodeEditLogRoller can keep printing "Swallowing exception" message |  Critical |  | Jing Zhao | Jing Zhao |
| [HDFS-7869](https://issues.apache.org/jira/browse/HDFS-7869) | Inconsistency in the return information while performing rolling upgrade |  Major |  | J.Andreina | J.Andreina |
| [HDFS-7831](https://issues.apache.org/jira/browse/HDFS-7831) | Fix the starting index and end condition of the loop in FileDiffList.findEarlierSnapshotBlocks() |  Major |  | Konstantin Shvachko | Konstantin Shvachko |
| [HDFS-7813](https://issues.apache.org/jira/browse/HDFS-7813) | TestDFSHAAdminMiniCluster#testFencer testcase is failing frequently |  Major | (ha , test) | Rakesh R | Rakesh R |
| [HDFS-7807](https://issues.apache.org/jira/browse/HDFS-7807) | libhdfs htable.c: fix htable resizing, add unit test |  Major | (native) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7805](https://issues.apache.org/jira/browse/HDFS-7805) | NameNode recovery prompt should be printed on console |  Major | (namenode) | surendra singh lilhore | surendra singh lilhore |
| [HDFS-7798](https://issues.apache.org/jira/browse/HDFS-7798) | Checkpointing failure caused by shared KerberosAuthenticator |  Critical | (security) | Chengbing Liu | Chengbing Liu |
| [HDFS-7788](https://issues.apache.org/jira/browse/HDFS-7788) | Post-2.6 namenode may not start up with an image containing inodes created with an old release. |  Blocker |  | Kihwal Lee | Rushabh S Shah |
| [HDFS-7785](https://issues.apache.org/jira/browse/HDFS-7785) | Improve diagnostics information for HttpPutFailedException |  Major | (namenode) | Chengbing Liu | Chengbing Liu |
| [HDFS-7778](https://issues.apache.org/jira/browse/HDFS-7778) | Rename FsVolumeListTest to TestFsVolumeList and commit it to branch-2 |  Major | (datanode , test) | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7774](https://issues.apache.org/jira/browse/HDFS-7774) | Unresolved symbols error while compiling HDFS on Windows 7/32 bit |  Critical | (build , native) | Venkatasubramaniam Ramakrishnan | Kiran Kumar M R |
| [HDFS-7769](https://issues.apache.org/jira/browse/HDFS-7769) | TestHDFSCLI create files in hdfs project root dir |  Trivial | (test) | Tsz Wo Nicholas Sze |  |
| [HDFS-7763](https://issues.apache.org/jira/browse/HDFS-7763) | fix zkfc hung issue due to not catching exception in a corner case |  Major | (ha) | Liang Xie | Liang Xie |
| [HDFS-7756](https://issues.apache.org/jira/browse/HDFS-7756) | Restore method signature for LocatedBlock#getLocations() |  Major |  | Ted Yu | Ted Yu |
| [HDFS-7753](https://issues.apache.org/jira/browse/HDFS-7753) | Fix Multithreaded correctness Warnings in BackupImage.java |  Major |  | Rakesh R | Konstantin Shvachko |
| [HDFS-7744](https://issues.apache.org/jira/browse/HDFS-7744) | Fix potential NPE in DFSInputStream after setDropBehind or setReadahead is called |  Major | (dfsclient) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7741](https://issues.apache.org/jira/browse/HDFS-7741) | Remove unnecessary synchronized in FSDataInputStream and HdfsDataInputStream |  Minor |  | Yi Liu | Yi Liu |
| [HDFS-7734](https://issues.apache.org/jira/browse/HDFS-7734) | Class cast exception in NameNode#main |  Blocker | (namenode) | Arpit Agarwal | Yi Liu |
| [HDFS-7721](https://issues.apache.org/jira/browse/HDFS-7721) | The HDFS BlockScanner may run fast during the first hour |  Major | (datanode) | Tsz Wo Nicholas Sze | Colin Patrick McCabe |
| [HDFS-7719](https://issues.apache.org/jira/browse/HDFS-7719) | BlockPoolSliceStorage#removeVolumes fails to remove some in-memory state associated with volumes |  Major |  | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7718](https://issues.apache.org/jira/browse/HDFS-7718) | Store KeyProvider in ClientContext to avoid leaking key provider threads when using FileContext |  Major |  | Arun Suresh | Arun Suresh |
| [HDFS-7714](https://issues.apache.org/jira/browse/HDFS-7714) | Simultaneous restart of HA NameNodes and DataNode can cause DataNode to register successfully with only one NameNode. |  Major | (datanode) | Chris Nauroth | Vinayakumar B |
| [HDFS-7709](https://issues.apache.org/jira/browse/HDFS-7709) | Fix findbug warnings in httpfs |  Major |  | Rakesh R | Rakesh R |
| [HDFS-7707](https://issues.apache.org/jira/browse/HDFS-7707) | Edit log corruption due to delayed block removal again |  Major | (namenode) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7704](https://issues.apache.org/jira/browse/HDFS-7704) | DN heartbeat to Active NN may be blocked and expire if connection to Standby NN continues to time out.  |  Major | (datanode , namenode) | Rushabh S Shah | Rushabh S Shah |
| [HDFS-7698](https://issues.apache.org/jira/browse/HDFS-7698) | Fix locking on HDFS read statistics and add a method for clearing them. |  Major |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7696](https://issues.apache.org/jira/browse/HDFS-7696) | FsDatasetImpl.getTmpInputStreams(..) may leak file descriptors |  Minor | (datanode) | Tsz Wo Nicholas Sze | Tsz Wo Nicholas Sze |
| [HDFS-7686](https://issues.apache.org/jira/browse/HDFS-7686) | Re-add rapid rescan of possibly corrupt block feature to the block scanner |  Blocker |  | Rushabh S Shah | Colin Patrick McCabe |
| [HDFS-7682](https://issues.apache.org/jira/browse/HDFS-7682) | {{DistributedFileSystem#getFileChecksum}} of a snapshotted file includes non-snapshotted content |  Major |  | Charles Lamb | Charles Lamb |
| [HDFS-7660](https://issues.apache.org/jira/browse/HDFS-7660) | BlockReceiver#close() might be called multiple times, which causes the fsvolume reference being released incorrectly. |  Minor |  | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7647](https://issues.apache.org/jira/browse/HDFS-7647) | DatanodeManager.sortLocatedBlocks sorts DatanodeInfos but not StorageIDs |  Major |  | Milan Desai | Milan Desai |
| [HDFS-7644](https://issues.apache.org/jira/browse/HDFS-7644) | minor typo in HttpFS doc |  Trivial | (documentation) | Charles Lamb | Charles Lamb |
| [HDFS-7641](https://issues.apache.org/jira/browse/HDFS-7641) | Update archival storage user doc for list/set/get block storage policies |  Minor | (documentation) | Yi Liu | Yi Liu |
| [HDFS-7637](https://issues.apache.org/jira/browse/HDFS-7637) | Fix the check condition for reserved path |  Minor |  | Yi Liu | Yi Liu |
| [HDFS-7635](https://issues.apache.org/jira/browse/HDFS-7635) | Remove TestCorruptFilesJsp from branch-2. |  Minor | (test) | Chris Nauroth | Chris Nauroth |
| [HDFS-7632](https://issues.apache.org/jira/browse/HDFS-7632) | MiniDFSCluster configures DataNode data directories incorrectly if using more than 1 DataNode and more than 2 storage locations per DataNode. |  Major | (test) | Chris Nauroth | Chris Nauroth |
| [HDFS-7615](https://issues.apache.org/jira/browse/HDFS-7615) | Remove longReadLock |  Major |  | Kihwal Lee | Kihwal Lee |
| [HDFS-7611](https://issues.apache.org/jira/browse/HDFS-7611) | deleteSnapshot and delete of a file can leave orphaned blocks in the blocksMap on NameNode restart. |  Critical | (namenode) | Konstantin Shvachko | Jing Zhao |
| [HDFS-7610](https://issues.apache.org/jira/browse/HDFS-7610) | Fix removal of dynamically added DN volumes |  Major | (datanode) | Lei (Eddy) Xu | Lei (Eddy) Xu |
| [HDFS-7606](https://issues.apache.org/jira/browse/HDFS-7606) | Missing null check in INodeFile#getBlocks() |  Minor |  | Ted Yu | Byron Wong |
| [HDFS-7603](https://issues.apache.org/jira/browse/HDFS-7603) | The background replication queue initialization may not let others run |  Critical | (rolling upgrades) | Kihwal Lee | Kihwal Lee |
| [HDFS-7596](https://issues.apache.org/jira/browse/HDFS-7596) | NameNode should prune dead storages from storageMap |  Major | (namenode) | Arpit Agarwal | Arpit Agarwal |
| [HDFS-7583](https://issues.apache.org/jira/browse/HDFS-7583) | Fix findbug in TransferFsImage.java |  Minor | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7575](https://issues.apache.org/jira/browse/HDFS-7575) | Upgrade should generate a unique storage ID for each volume |  Critical |  | Lars Francke | Arpit Agarwal |
| [HDFS-7572](https://issues.apache.org/jira/browse/HDFS-7572) | TestLazyPersistFiles#testDnRestartWithSavedReplicas is flaky on Windows |  Major | (test) | Arpit Agarwal | Arpit Agarwal |
| [HDFS-7566](https://issues.apache.org/jira/browse/HDFS-7566) | Remove obsolete entries from hdfs-default.xml |  Major |  | Ray Chiang | Ray Chiang |
| [HDFS-7563](https://issues.apache.org/jira/browse/HDFS-7563) | NFS gateway parseStaticMap NumberFormatException |  Major | (nfs) | Hari Sekhon | Yongjun Zhang |
| [HDFS-7561](https://issues.apache.org/jira/browse/HDFS-7561) | TestFetchImage should write fetched-image-dir under target. |  Major |  | Konstantin Shvachko | Liang Xie |
| [HDFS-7560](https://issues.apache.org/jira/browse/HDFS-7560) | ACLs removed by removeDefaultAcl() will be back after NameNode restart/failover |  Critical | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7552](https://issues.apache.org/jira/browse/HDFS-7552) | change FsVolumeList toString() to fix TestDataNodeVolumeFailureToleration  |  Major | (datanode , test) | Liang Xie | Liang Xie |
| [HDFS-7548](https://issues.apache.org/jira/browse/HDFS-7548) | Corrupt block reporting delayed until datablock scanner thread detects it |  Major |  | Rushabh S Shah | Rushabh S Shah |
| [HDFS-7536](https://issues.apache.org/jira/browse/HDFS-7536) | Remove unused CryptoCodec in org.apache.hadoop.fs.Hdfs |  Minor | (security) | Yi Liu | Yi Liu |
| [HDFS-7533](https://issues.apache.org/jira/browse/HDFS-7533) | Datanode sometimes does not shutdown on receiving upgrade shutdown command |  Major |  | Kihwal Lee | Eric Payne |
| [HDFS-7530](https://issues.apache.org/jira/browse/HDFS-7530) | Allow renaming of encryption zone roots |  Minor | (namenode) | Charles Lamb | Charles Lamb |
| [HDFS-7517](https://issues.apache.org/jira/browse/HDFS-7517) | Remove redundant non-null checks in FSNamesystem#getBlockLocations |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7516](https://issues.apache.org/jira/browse/HDFS-7516) | Fix findbugs warnings in hadoop-nfs project |  Major | (nfs) | Brandon Li | Brandon Li |
| [HDFS-7515](https://issues.apache.org/jira/browse/HDFS-7515) | Fix new findbugs warnings in hadoop-hdfs |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7514](https://issues.apache.org/jira/browse/HDFS-7514) | TestTextCommand fails on Windows |  Major | (test) | Arpit Agarwal | Arpit Agarwal |
| [HDFS-7502](https://issues.apache.org/jira/browse/HDFS-7502) | Fix findbugs warning in hdfs-nfs project |  Major | (nfs) | Brandon Li | Brandon Li |
| [HDFS-7497](https://issues.apache.org/jira/browse/HDFS-7497) | Inconsistent report of decommissioning DataNodes between dfsadmin and NameNode webui |  Major | (datanode , namenode) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7496](https://issues.apache.org/jira/browse/HDFS-7496) | Fix FsVolume removal race conditions on the DataNode by reference-counting the volume instances |  Major |  | Colin Patrick McCabe | Lei (Eddy) Xu |
| [HDFS-7495](https://issues.apache.org/jira/browse/HDFS-7495) | Remove updatePosition argument from DFSInputStream#getBlockAt() |  Minor |  | Ted Yu | Colin Patrick McCabe |
| [HDFS-7494](https://issues.apache.org/jira/browse/HDFS-7494) | Checking of closed in DFSInputStream#pread() should be protected by synchronization |  Minor |  | Ted Yu | Ted Yu |
| [HDFS-7490](https://issues.apache.org/jira/browse/HDFS-7490) | HDFS tests OOM on Java7+ |  Major | (build , test) | Steve Loughran | Steve Loughran |
| [HDFS-7481](https://issues.apache.org/jira/browse/HDFS-7481) | Add ACL indicator to the "Permission Denied" exception. |  Minor | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7473](https://issues.apache.org/jira/browse/HDFS-7473) | Document setting dfs.namenode.fs-limits.max-directory-items to 0 is invalid |  Major | (documentation) | Jason Keller | Akira AJISAKA |
| [HDFS-7472](https://issues.apache.org/jira/browse/HDFS-7472) | Fix typo in message of ReplicaNotFoundException |  Trivial |  | Masatake Iwasaki | Masatake Iwasaki |
| [HDFS-7470](https://issues.apache.org/jira/browse/HDFS-7470) | SecondaryNameNode need twice memory when calling reloadFromImageFile |  Major | (namenode) | zhaoyunjiong | zhaoyunjiong |
| [HDFS-7457](https://issues.apache.org/jira/browse/HDFS-7457) | DatanodeID generates excessive garbage |  Major | (namenode) | Daryn Sharp | Daryn Sharp |
| [HDFS-7456](https://issues.apache.org/jira/browse/HDFS-7456) | De-duplicate AclFeature instances with same AclEntries do reduce memory footprint of NameNode |  Major | (namenode) | Vinayakumar B | Vinayakumar B |
| [HDFS-7444](https://issues.apache.org/jira/browse/HDFS-7444) | convertToBlockUnderConstruction should preserve BlockCollection |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7431](https://issues.apache.org/jira/browse/HDFS-7431) | log message for InvalidMagicNumberException may be incorrect |  Major | (security) | Yi Liu | Yi Liu |
| [HDFS-7423](https://issues.apache.org/jira/browse/HDFS-7423) | various typos and message formatting fixes in nfs daemon and doc |  Trivial | (nfs) | Charles Lamb | Charles Lamb |
| [HDFS-7406](https://issues.apache.org/jira/browse/HDFS-7406) | SimpleHttpProxyHandler puts incorrect "Connection: Close" header |  Major |  | Haohui Mai | Haohui Mai |
| [HDFS-7403](https://issues.apache.org/jira/browse/HDFS-7403) | Inaccurate javadoc of  BlockUCState#COMPLETE state |  Trivial | (namenode) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7399](https://issues.apache.org/jira/browse/HDFS-7399) | Lack of synchronization in DFSOutputStream#Packet#getLastByteOffsetBlock() |  Minor |  | Ted Yu | Vinayakumar B |
| [HDFS-7395](https://issues.apache.org/jira/browse/HDFS-7395) | BlockIdManager#clear() bails out when resetting the GenerationStampV1Limit |  Major | (namenode) | Yongjun Zhang | Haohui Mai |
| [HDFS-7394](https://issues.apache.org/jira/browse/HDFS-7394) | Log at INFO level, not WARN level, when InvalidToken is seen in ShortCircuitCache |  Minor |  | Kihwal Lee | Keith Pak |
| [HDFS-7389](https://issues.apache.org/jira/browse/HDFS-7389) | Named user ACL cannot stop the user from accessing the FS entity. |  Major | (namenode) | Chunjun Xiao | Vinayakumar B |
| [HDFS-7374](https://issues.apache.org/jira/browse/HDFS-7374) | Allow decommissioning of dead DataNodes |  Major |  | Zhe Zhang | Zhe Zhang |
| [HDFS-7373](https://issues.apache.org/jira/browse/HDFS-7373) | Clean up temporary files after fsimage transfer failures |  Major |  | Kihwal Lee | Kihwal Lee |
| [HDFS-7366](https://issues.apache.org/jira/browse/HDFS-7366) | BlockInfo should take replication as an short in the constructor |  Minor |  | Haohui Mai | Li Lu |
| [HDFS-7361](https://issues.apache.org/jira/browse/HDFS-7361) | TestCheckpoint#testStorageAlreadyLockedErrorMessage fails after change of log message related to locking violation. |  Minor | (datanode , namenode , test) | Chris Nauroth | Konstantin Shvachko |
| [HDFS-7358](https://issues.apache.org/jira/browse/HDFS-7358) | Clients may get stuck waiting when using ByteArrayManager |  Major | (hdfs-client) | Tsz Wo Nicholas Sze | Tsz Wo Nicholas Sze |
| [HDFS-7324](https://issues.apache.org/jira/browse/HDFS-7324) | haadmin command usage prints incorrect command name |  Major | (ha , tools) | Brahma Reddy Battula | Brahma Reddy Battula |
| [HDFS-7315](https://issues.apache.org/jira/browse/HDFS-7315) | DFSTestUtil.readFileBuffer opens extra FSDataInputStream |  Trivial |  | Plamen Jeliazkov | Plamen Jeliazkov |
| [HDFS-7303](https://issues.apache.org/jira/browse/HDFS-7303) | NN UI fails to distinguish datanodes on the same host |  Minor |  | Benoy Antony | Benoy Antony |
| [HDFS-7301](https://issues.apache.org/jira/browse/HDFS-7301) | TestMissingBlocksAlert should use MXBeans instead of old web UI |  Minor |  | Zhe Zhang | Zhe Zhang |
| [HDFS-7282](https://issues.apache.org/jira/browse/HDFS-7282) | Fix intermittent TestShortCircuitCache and TestBlockReaderFactory failures resulting from TemporarySocketDirectory GC |  Major | (test) | Jinghui Wang | Jinghui Wang |
| [HDFS-7277](https://issues.apache.org/jira/browse/HDFS-7277) | Remove explicit dependency on netty 3.2 in BKJournal |  Minor | (build) | Haohui Mai | Haohui Mai |
| [HDFS-7263](https://issues.apache.org/jira/browse/HDFS-7263) | Snapshot read can reveal future bytes for appended files. |  Major | (hdfs-client) | Konstantin Shvachko | Tao Luo |
| [HDFS-7258](https://issues.apache.org/jira/browse/HDFS-7258) | CacheReplicationMonitor rescan schedule log should use DEBUG level instead of INFO level |  Minor | (namenode) | Xiaoyu Yao | Xiaoyu Yao |
| [HDFS-7235](https://issues.apache.org/jira/browse/HDFS-7235) | DataNode#transferBlock should report blocks that don't exist using reportBadBlock |  Major | (datanode , namenode) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7232](https://issues.apache.org/jira/browse/HDFS-7232) | Populate hostname in httpfs audit log |  Trivial |  | Zoran Dimitrijevic | Zoran Dimitrijevic |
| [HDFS-7227](https://issues.apache.org/jira/browse/HDFS-7227) | Fix findbugs warning about NP_DEREFERENCE_OF_READLINE_VALUE in SpanReceiverHost |  Minor |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7225](https://issues.apache.org/jira/browse/HDFS-7225) | Remove stale block invalidation work when DN re-registers with different UUID |  Major | (namenode) | Zhe Zhang | Zhe Zhang |
| [HDFS-7224](https://issues.apache.org/jira/browse/HDFS-7224) | Allow reuse of NN connections via webhdfs |  Major | (webhdfs) | Eric Payne | Eric Payne |
| [HDFS-7213](https://issues.apache.org/jira/browse/HDFS-7213) | processIncrementalBlockReport performance degradation |  Critical | (namenode) | Daryn Sharp | Eric Payne |
| [HDFS-7202](https://issues.apache.org/jira/browse/HDFS-7202) | Should be able to omit package name of SpanReceiver on "hadoop trace -add" |  Minor |  | Masatake Iwasaki | Masatake Iwasaki |
| [HDFS-7201](https://issues.apache.org/jira/browse/HDFS-7201) | Fix typos in hdfs-default.xml |  Major |  | Konstantin Shvachko | Dawson Choong |
| [HDFS-7198](https://issues.apache.org/jira/browse/HDFS-7198) | Fix findbugs "unchecked conversion" warning in DFSClient#getPathTraceScope |  Trivial |  | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-7194](https://issues.apache.org/jira/browse/HDFS-7194) | Fix findbugs "inefficient new String constructor" warning in DFSClient#PATH |  Trivial |  | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7146](https://issues.apache.org/jira/browse/HDFS-7146) | NFS ID/Group lookup requires SSSD enumeration on the server |  Major | (nfs) | Yongjun Zhang | Yongjun Zhang |
| [HDFS-7097](https://issues.apache.org/jira/browse/HDFS-7097) | Allow block reports to be processed during checkpointing on standby name node |  Critical |  | Kihwal Lee | Kihwal Lee |
| [HDFS-7009](https://issues.apache.org/jira/browse/HDFS-7009) | Active NN and standby NN have different live nodes |  Major | (datanode) | Ming Ma | Ming Ma |
| [HDFS-7008](https://issues.apache.org/jira/browse/HDFS-7008) | xlator should be closed upon exit from DFSAdmin#genericRefresh() |  Minor |  | Ted Yu | Tsuyoshi Ozawa |
| [HDFS-6938](https://issues.apache.org/jira/browse/HDFS-6938) | Cleanup javac warnings in FSNamesystem |  Trivial | (namenode) | Charles Lamb | Charles Lamb |
| [HDFS-6917](https://issues.apache.org/jira/browse/HDFS-6917) | Add an hdfs debug command to validate blocks, call recoverlease, etc. |  Major | (hdfs-client) | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-6753](https://issues.apache.org/jira/browse/HDFS-6753) | Initialize checkDisk when DirectoryScanner not able to get files list for scanning |  Major |  | J.Andreina | J.Andreina |
| [HDFS-6662](https://issues.apache.org/jira/browse/HDFS-6662) | WebHDFS cannot open a file if its path contains "%" |  Critical | (namenode) | Brahma Reddy Battula | Gerson Carlos |
| [HDFS-6657](https://issues.apache.org/jira/browse/HDFS-6657) | Remove link to 'Legacy UI' in Namenode UI |  Minor |  | Vinayakumar B | Vinayakumar B |
| [HDFS-6538](https://issues.apache.org/jira/browse/HDFS-6538) | Comment format error in ShortCircuitRegistry javadoc |  Trivial | (datanode) | debugging | David Luo |
| [HDFS-6425](https://issues.apache.org/jira/browse/HDFS-6425) | Large postponedMisreplicatedBlocks has impact on blockReport latency |  Major |  | Ming Ma | Ming Ma |
| [HDFS-5578](https://issues.apache.org/jira/browse/HDFS-5578) | [JDK8] Fix Javadoc errors caused by incorrect or illegal tags in doc comments |  Minor |  | Andrew Purtell | Andrew Purtell |
| [HDFS-5445](https://issues.apache.org/jira/browse/HDFS-5445) | PacketReceiver populates the packetLen field in PacketHeader incorrectly |  Minor | (datanode) | Jonathan Mace | Jonathan Mace |
| [HDFS-3519](https://issues.apache.org/jira/browse/HDFS-3519) | Checkpoint upload may interfere with a concurrent saveNamespace |  Critical | (namenode) | Todd Lipcon | Ming Ma |
| [HDFS-1522](https://issues.apache.org/jira/browse/HDFS-1522) | Merge Block.BLOCK_FILE_PREFIX and DataStorage.BLOCK_FILE_PREFIX into one constant |  Major | (datanode) | Konstantin Shvachko | Dongming Liang |
| [HDFS-49](https://issues.apache.org/jira/browse/HDFS-49) | MiniDFSCluster.stopDataNode will always shut down a node in the cluster if a matching name is not found |  Minor | (test) | Steve Loughran | Steve Loughran |
| [MAPREDUCE-6268](https://issues.apache.org/jira/browse/MAPREDUCE-6268) | Fix typo in Task Attempt API's URL |  Minor |  | Ryu Kobayashi | Ryu Kobayashi |
| [MAPREDUCE-6261](https://issues.apache.org/jira/browse/MAPREDUCE-6261) | NullPointerException if MapOutputBuffer.flush invoked twice |  Major | (mrv2) | Jason Lowe | Tsuyoshi Ozawa |
| [MAPREDUCE-6243](https://issues.apache.org/jira/browse/MAPREDUCE-6243) | Fix findbugs warnings in hadoop-rumen |  Minor | (tools/rumen) | Akira AJISAKA | Masatake Iwasaki |
| [MAPREDUCE-6233](https://issues.apache.org/jira/browse/MAPREDUCE-6233) | org.apache.hadoop.mapreduce.TestLargeSort.testLargeSort failed in trunk |  Major | (test) | Yongjun Zhang | zhihai xu |
| [MAPREDUCE-6231](https://issues.apache.org/jira/browse/MAPREDUCE-6231) | Grep example job is not working on a fully-distributed cluster |  Major | (examples) | Akira AJISAKA | Akira AJISAKA |
| [MAPREDUCE-6230](https://issues.apache.org/jira/browse/MAPREDUCE-6230) | MR AM does not survive RM restart if RM activated a new AMRM secret key |  Blocker | (mr-am) | Jason Lowe | Jason Lowe |
| [MAPREDUCE-6225](https://issues.apache.org/jira/browse/MAPREDUCE-6225) | Fix new findbug warnings in hadoop-mapreduce-client-core |  Major |  | Jason Lowe | Varun Saxena |
| [MAPREDUCE-6221](https://issues.apache.org/jira/browse/MAPREDUCE-6221) | Stringifier is left unclosed in Chain#getChainElementConf() |  Minor |  | Ted Yu | Ted Yu |
| [MAPREDUCE-6210](https://issues.apache.org/jira/browse/MAPREDUCE-6210) | Use getApplicationAttemptId() instead of getApplicationID() for logging AttemptId in RMContainerAllocator.java |  Minor | (applicationmaster) | Leitao Guo | Leitao Guo |
| [MAPREDUCE-6206](https://issues.apache.org/jira/browse/MAPREDUCE-6206) | TestAggregatedTransferRate fails on non-US systems |  Critical |  | Jens Rabe | Jens Rabe |
| [MAPREDUCE-6199](https://issues.apache.org/jira/browse/MAPREDUCE-6199) | AbstractCounters are not reset completely on deserialization |  Major |  | Anubhav Dhoot | Anubhav Dhoot |
| [MAPREDUCE-6186](https://issues.apache.org/jira/browse/MAPREDUCE-6186) | Redundant call to requireJob() while displaying the conf page |  Minor | (jobhistoryserver) | Rohit Agarwal | Rohit Agarwal |
| [MAPREDUCE-6177](https://issues.apache.org/jira/browse/MAPREDUCE-6177) | Minor typo in the EncryptedShuffle document about ssl-client.xml |  Trivial | (documentation) | yangping wu | yangping wu |
| [MAPREDUCE-6172](https://issues.apache.org/jira/browse/MAPREDUCE-6172) | TestDbClasses timeouts are too aggressive |  Minor | (test) | Jason Lowe | Varun Saxena |
| [MAPREDUCE-6166](https://issues.apache.org/jira/browse/MAPREDUCE-6166) | Reducers do not validate checksum of map outputs when fetching directly to disk |  Major | (mrv2) | Eric Payne | Eric Payne |
| [MAPREDUCE-6162](https://issues.apache.org/jira/browse/MAPREDUCE-6162) | mapred hsadmin fails on a secure cluster |  Blocker | (jobhistoryserver) | Jason Lowe | Jason Lowe |
| [MAPREDUCE-6160](https://issues.apache.org/jira/browse/MAPREDUCE-6160) | Potential NullPointerException in MRClientProtocol interface implementation. |  Major |  | Rohith | Rohith |
| [MAPREDUCE-6136](https://issues.apache.org/jira/browse/MAPREDUCE-6136) | MRAppMaster doesn't shutdown file systems |  Major | (applicationmaster) | Noah Watkins | Brahma Reddy Battula |
| [MAPREDUCE-6049](https://issues.apache.org/jira/browse/MAPREDUCE-6049) | AM JVM does not exit if MRClientService gracefull shutdown fails |  Major | (applicationmaster , resourcemanager) | Nishan Shetty | Rohith |
| [MAPREDUCE-6045](https://issues.apache.org/jira/browse/MAPREDUCE-6045) | need close the DataInputStream after open it in TestMapReduce.java |  Minor | (test) | zhihai xu | zhihai xu |
| [MAPREDUCE-5988](https://issues.apache.org/jira/browse/MAPREDUCE-5988) | Fix dead links to the javadocs in mapreduce project |  Minor | (documentation) | Akira AJISAKA | Akira AJISAKA |
| [MAPREDUCE-5918](https://issues.apache.org/jira/browse/MAPREDUCE-5918) | LineRecordReader can return the same decompressor to CodecPool multiple times |  Major |  | Sergey Murylev | Sergey Murylev |
| [MAPREDUCE-5875](https://issues.apache.org/jira/browse/MAPREDUCE-5875) | Make Counter limits consistent across JobClient, MRAppMaster, and YarnChild |  Major | (applicationmaster , client , task) | Gera Shegalov | Gera Shegalov |
| [MAPREDUCE-5568](https://issues.apache.org/jira/browse/MAPREDUCE-5568) | JHS returns invalid string for reducer completion percentage if AM restarts with 0 reducer. |  Major |  | Jian He | MinJi Kim |
| [MAPREDUCE-4879](https://issues.apache.org/jira/browse/MAPREDUCE-4879) | TeraOutputFormat may overwrite an existing output directory |  Major | (examples) | Gera Shegalov | Gera Shegalov |
| [MAPREDUCE-4286](https://issues.apache.org/jira/browse/MAPREDUCE-4286) | TestClientProtocolProviderImpls passes on failure conditions |  Major |  | Devaraj K | Devaraj K |
| [MAPREDUCE-3283](https://issues.apache.org/jira/browse/MAPREDUCE-3283) | mapred classpath CLI does not display the complete classpath |  Minor | (scripts) | Ramya Sunil | Varun Saxena |
| [MAPREDUCE-2815](https://issues.apache.org/jira/browse/MAPREDUCE-2815) | JavaDoc does not generate correctly for MultithreadedMapRunner |  Minor | (documentation) | Shane Butler | Chris Palmer |
| [YARN-3281](https://issues.apache.org/jira/browse/YARN-3281) | Add RMStateStore to StateMachine visualization list |  Minor | (scripts) | Chengbing Liu | Chengbing Liu |
| [YARN-3270](https://issues.apache.org/jira/browse/YARN-3270) | node label expression not getting set in ApplicationSubmissionContext |  Minor |  | Rohit Agarwal | Rohit Agarwal |
| [YARN-3256](https://issues.apache.org/jira/browse/YARN-3256) | TestClientToAMTokens#testClientTokenRace is not running against all Schedulers even when using ParameterizedSchedulerTestBase |  Major |  | Anubhav Dhoot | Anubhav Dhoot |
| [YARN-3255](https://issues.apache.org/jira/browse/YARN-3255) | RM, NM, JobHistoryServer, and WebAppProxyServer's main() should support generic options |  Major | (nodemanager , resourcemanager) | Konstantin Shvachko | Konstantin Shvachko |
| [YARN-3242](https://issues.apache.org/jira/browse/YARN-3242) | Asynchrony in ZK-close can lead to ZKRMStateStore watcher receiving events for old client |  Critical | (resourcemanager) | zhihai xu | zhihai xu |
| [YARN-3239](https://issues.apache.org/jira/browse/YARN-3239) | WebAppProxy does not support a final tracking url which has query fragments and params  |  Major |  | Hitesh Shah | Jian He |
| [YARN-3238](https://issues.apache.org/jira/browse/YARN-3238) | Connection timeouts to nodemanagers are retried at multiple levels |  Blocker |  | Jason Lowe | Jason Lowe |
| [YARN-3237](https://issues.apache.org/jira/browse/YARN-3237) | AppLogAggregatorImpl fails to log error cause |  Major |  | Rushabh S Shah | Rushabh S Shah |
| [YARN-3231](https://issues.apache.org/jira/browse/YARN-3231) | FairScheduler: Changing queueMaxRunningApps interferes with pending jobs |  Critical |  | Siqi Li | Siqi Li |
| [YARN-3222](https://issues.apache.org/jira/browse/YARN-3222) | RMNodeImpl#ReconnectNodeTransition should send scheduler events in sequential order |  Critical | (resourcemanager) | Rohith | Rohith |
| [YARN-3207](https://issues.apache.org/jira/browse/YARN-3207) | secondary filter matches entites which do not have the key being filtered for. |  Major | (timelineserver) | Prakash Ramachandran | Zhijie Shen |
| [YARN-3194](https://issues.apache.org/jira/browse/YARN-3194) | RM should handle NMContainerStatuses sent by NM while registering if NM is Reconnected node |  Blocker | (resourcemanager) | Rohith | Rohith |
| [YARN-3191](https://issues.apache.org/jira/browse/YARN-3191) | Log object should be initialized with its own class |  Trivial | (nodemanager) | Rohith | Rohith |
| [YARN-3164](https://issues.apache.org/jira/browse/YARN-3164) | rmadmin command usage prints incorrect command name |  Minor | (resourcemanager) | Bibin A Chundatt | Bibin A Chundatt |
| [YARN-3160](https://issues.apache.org/jira/browse/YARN-3160) | Non-atomic operation on nodeUpdateQueue in RMNodeImpl |  Major | (resourcemanager) | Chengbing Liu | Chengbing Liu |
| [YARN-3155](https://issues.apache.org/jira/browse/YARN-3155) | Refactor the exception handling code for TimelineClientImpl's retryOn method |  Minor |  | Li Lu | Li Lu |
| [YARN-3151](https://issues.apache.org/jira/browse/YARN-3151) | On Failover tracking url wrong in application cli for KILLED application |  Minor | (client , resourcemanager) | Bibin A Chundatt | Rohith |
| [YARN-3149](https://issues.apache.org/jira/browse/YARN-3149) | Typo in message for invalid application id |  Trivial | (resourcemanager) | Bibin A Chundatt | Bibin A Chundatt |
| [YARN-3145](https://issues.apache.org/jira/browse/YARN-3145) | ConcurrentModificationException on CapacityScheduler ParentQueue#getQueueUserAclInfo |  Major |  | Jian He | Tsuyoshi Ozawa |
| [YARN-3143](https://issues.apache.org/jira/browse/YARN-3143) | RM Apps REST API can return NPE or entries missing id and other fields |  Major | (webapp) | Kendall Thrapp | Jason Lowe |
| [YARN-3131](https://issues.apache.org/jira/browse/YARN-3131) | YarnClientImpl should check FAILED and KILLED state in submitApplication |  Major |  | Chang Li | Chang Li |
| [YARN-3113](https://issues.apache.org/jira/browse/YARN-3113) | Release audit warning for "Sorting icons.psd" |  Major |  | Chang Li | Steve Loughran |
| [YARN-3104](https://issues.apache.org/jira/browse/YARN-3104) | RM generates new AMRM tokens every heartbeat between rolling and activation |  Major | (resourcemanager) | Jason Lowe | Jason Lowe |
| [YARN-3103](https://issues.apache.org/jira/browse/YARN-3103) | AMRMClientImpl does not update AMRM token properly |  Blocker | (client) | Jason Lowe | Jason Lowe |
| [YARN-3101](https://issues.apache.org/jira/browse/YARN-3101) | In Fair Scheduler, fix canceling of reservations for exceeding max share |  Major | (fairscheduler) | Anubhav Dhoot | Anubhav Dhoot |
| [YARN-3094](https://issues.apache.org/jira/browse/YARN-3094) | reset timer for liveness monitors after RM recovery |  Major | (resourcemanager) | Jun Gong | Jun Gong |
| [YARN-3090](https://issues.apache.org/jira/browse/YARN-3090) | DeletionService can silently ignore deletion task failures |  Major | (nodemanager) | Jason Lowe | Varun Saxena |
| [YARN-3089](https://issues.apache.org/jira/browse/YARN-3089) | LinuxContainerExecutor does not handle file arguments to deleteAsUser |  Blocker |  | Jason Lowe | Eric Payne |
| [YARN-3088](https://issues.apache.org/jira/browse/YARN-3088) | LinuxContainerExecutor.deleteAsUser can throw NPE if native executor returns an error |  Major | (nodemanager) | Jason Lowe | Eric Payne |
| [YARN-3079](https://issues.apache.org/jira/browse/YARN-3079) | Scheduler should also update maximumAllocation when updateNodeResource. |  Major |  | zhihai xu | zhihai xu |
| [YARN-3078](https://issues.apache.org/jira/browse/YARN-3078) | LogCLIHelpers lacks of a blank space before string 'does not exist' |  Minor | (log-aggregation) | sam liu |  |
| [YARN-3074](https://issues.apache.org/jira/browse/YARN-3074) | Nodemanager dies when localizer runner tries to write to a full disk |  Major | (nodemanager) | Jason Lowe | Varun Saxena |
| [YARN-3071](https://issues.apache.org/jira/browse/YARN-3071) | Remove invalid char from sample conf in doc of FairScheduler |  Trivial | (documentation) | Masatake Iwasaki | Masatake Iwasaki |
| [YARN-3064](https://issues.apache.org/jira/browse/YARN-3064) | TestRMRestart/TestContainerResourceUsage/TestNodeManagerResync failure with allocation timeout |  Critical | (scheduler) | Wangda Tan | Jian He |
| [YARN-3058](https://issues.apache.org/jira/browse/YARN-3058) | Fix error message of tokens' activation delay configuration |  Minor |  | Yi Liu | Yi Liu |
| [YARN-3027](https://issues.apache.org/jira/browse/YARN-3027) | Scheduler should use totalAvailable resource from node instead of availableResource for maxAllocation |  Major |  | Anubhav Dhoot | Anubhav Dhoot |
| [YARN-3024](https://issues.apache.org/jira/browse/YARN-3024) | LocalizerRunner should give DIE action when all resources are localized |  Major | (nodemanager) | Chengbing Liu | Chengbing Liu |
| [YARN-3015](https://issues.apache.org/jira/browse/YARN-3015) | yarn classpath command should support same options as hadoop classpath. |  Minor | (scripts) | Chris Nauroth | Varun Saxena |
| [YARN-3010](https://issues.apache.org/jira/browse/YARN-3010) | Fix recent findbug issue in AbstractYarnScheduler |  Minor |  | Yi Liu | Yi Liu |
| [YARN-2997](https://issues.apache.org/jira/browse/YARN-2997) | NM keeps sending already-sent completed containers to RM until containers are removed from context |  Major | (nodemanager) | Chengbing Liu | Chengbing Liu |
| [YARN-2993](https://issues.apache.org/jira/browse/YARN-2993) | Several fixes (missing acl check, error log msg ...) and some refinement in AdminService |  Major | (resourcemanager) | Yi Liu | Yi Liu |
| [YARN-2992](https://issues.apache.org/jira/browse/YARN-2992) | ZKRMStateStore crashes due to session expiry |  Blocker | (resourcemanager) | Karthik Kambatla | Karthik Kambatla |
| [YARN-2991](https://issues.apache.org/jira/browse/YARN-2991) | TestRMRestart.testDecomissionedNMsMetricsOnRMRestart intermittently fails on trunk |  Blocker |  | Zhijie Shen | Rohith |
| [YARN-2990](https://issues.apache.org/jira/browse/YARN-2990) | FairScheduler's delay-scheduling always waits for node-local and rack-local delays, even for off-rack-only requests |  Major | (fairscheduler) | Karthik Kambatla | Karthik Kambatla |
| [YARN-2988](https://issues.apache.org/jira/browse/YARN-2988) | Graph#save() may leak file descriptors |  Minor |  | Ted Yu | Ted Yu |
| [YARN-2987](https://issues.apache.org/jira/browse/YARN-2987) | ClientRMService#getQueueInfo doesn't check app ACLs |  Major |  | Jian He | Varun Saxena |
| [YARN-2983](https://issues.apache.org/jira/browse/YARN-2983) | NPE possible in ClientRMService#getQueueInfo |  Major | (resourcemanager) | Varun Saxena | Varun Saxena |
| [YARN-2978](https://issues.apache.org/jira/browse/YARN-2978) | ResourceManager crashes with NPE while getting queue info |  Critical |  | Jason Tufo | Varun Saxena |
| [YARN-2977](https://issues.apache.org/jira/browse/YARN-2977) | TestNMClient get failed intermittently  |  Major |  | Junping Du | Junping Du |
| [YARN-2975](https://issues.apache.org/jira/browse/YARN-2975) | FSLeafQueue app lists are accessed without required locks |  Blocker |  | Karthik Kambatla | Karthik Kambatla |
| [YARN-2972](https://issues.apache.org/jira/browse/YARN-2972) | DelegationTokenRenewer thread pool never expands |  Major | (resourcemanager) | Jason Lowe | Jason Lowe |
| [YARN-2964](https://issues.apache.org/jira/browse/YARN-2964) | RM prematurely cancels tokens for jobs that submit jobs (oozie) |  Blocker | (resourcemanager) | Daryn Sharp | Jian He |
| [YARN-2958](https://issues.apache.org/jira/browse/YARN-2958) | RMStateStore seems to unnecessarily and wrongly store sequence number separately |  Blocker | (resourcemanager) | Zhijie Shen | Varun Saxena |
| [YARN-2956](https://issues.apache.org/jira/browse/YARN-2956) | Some yarn-site index linked pages are difficult to discover because are not in the side bar |  Minor | (documentation) | Remus Rusanu | Masatake Iwasaki |
| [YARN-2952](https://issues.apache.org/jira/browse/YARN-2952) | Incorrect version check in RMStateStore |  Major |  | Jian He | Rohith |
| [YARN-2945](https://issues.apache.org/jira/browse/YARN-2945) | FSLeafQueue#assignContainer - document the reason for using both write and read locks |  Major |  | Tsuyoshi Ozawa | Tsuyoshi Ozawa |
| [YARN-2936](https://issues.apache.org/jira/browse/YARN-2936) | YARNDelegationTokenIdentifier doesn't set proto.builder now |  Major |  | Zhijie Shen | Varun Saxena |
| [YARN-2932](https://issues.apache.org/jira/browse/YARN-2932) | Add entry for "preemptable" status (enabled/disabled) to scheduler web UI and queue initialize/refresh logging |  Major |  | Eric Payne | Eric Payne |
| [YARN-2931](https://issues.apache.org/jira/browse/YARN-2931) | PublicLocalizer may fail until directory is initialized by LocalizeRunner |  Critical | (nodemanager) | Anubhav Dhoot | Anubhav Dhoot |
| [YARN-2922](https://issues.apache.org/jira/browse/YARN-2922) | ConcurrentModificationException in CapacityScheduler's LeafQueue |  Major | (capacityscheduler , resourcemanager , scheduler) | Jason Tufo | Rohith |
| [YARN-2917](https://issues.apache.org/jira/browse/YARN-2917) | Potential deadlock in AsyncDispatcher when system.exit called in AsyncDispatcher#dispatch and AsyscDispatcher#serviceStop from shutdown hook |  Critical | (resourcemanager) | Rohith | Rohith |
| [YARN-2912](https://issues.apache.org/jira/browse/YARN-2912) | Jersey Tests failing with port in use |  Major | (test) | Steve Loughran | Varun Saxena |
| [YARN-2910](https://issues.apache.org/jira/browse/YARN-2910) | FSLeafQueue can throw ConcurrentModificationException |  Major | (fairscheduler) | Wilfred Spiegelenburg | Wilfred Spiegelenburg |
| [YARN-2907](https://issues.apache.org/jira/browse/YARN-2907) | SchedulerNode#toString should print all resource detail instead of only memory. |  Trivial | (resourcemanager) | Rohith | Rohith |
| [YARN-2906](https://issues.apache.org/jira/browse/YARN-2906) | CapacitySchedulerPage shows HTML tags for a queue's Active Users |  Major | (capacityscheduler) | Jason Lowe | Jason Lowe |
| [YARN-2905](https://issues.apache.org/jira/browse/YARN-2905) | AggregatedLogsBlock page can infinitely loop if the aggregated log file is corrupted |  Blocker |  | Jason Lowe | Varun Saxena |
| [YARN-2899](https://issues.apache.org/jira/browse/YARN-2899) | Run TestDockerContainerExecutorWithMocks on Linux only |  Minor | (nodemanager , test) | Ming Ma | Ming Ma |
| [YARN-2897](https://issues.apache.org/jira/browse/YARN-2897) | CrossOriginFilter needs more log statements |  Major |  | Mit Desai | Mit Desai |
| [YARN-2894](https://issues.apache.org/jira/browse/YARN-2894) | When ACL's are enabled, if RM switches then application can not be viewed from web. |  Major | (resourcemanager) | Rohith | Rohith |
| [YARN-2874](https://issues.apache.org/jira/browse/YARN-2874) | Dead lock in "DelegationTokenRenewer" which blocks RM to execute any further apps |  Blocker | (resourcemanager) | Naganarasimha G R | Naganarasimha G R |
| [YARN-2870](https://issues.apache.org/jira/browse/YARN-2870) | Update examples in document of Timeline Server |  Trivial | (documentation , timelineserver) | Masatake Iwasaki | Masatake Iwasaki |
| [YARN-2869](https://issues.apache.org/jira/browse/YARN-2869) | CapacityScheduler should trim sub queue names when parse configuration |  Major | (capacityscheduler , resourcemanager) | Wangda Tan | Wangda Tan |
| [YARN-2865](https://issues.apache.org/jira/browse/YARN-2865) | Application recovery continuously fails with "Application with id already present. Cannot duplicate" |  Critical | (resourcemanager) | Rohith | Rohith |
| [YARN-2861](https://issues.apache.org/jira/browse/YARN-2861) | Timeline DT secret manager should not reuse the RM's configs. |  Major |  | Zhijie Shen | Zhijie Shen |
| [YARN-2857](https://issues.apache.org/jira/browse/YARN-2857) | ConcurrentModificationException in ContainerLogAppender |  Critical |  | Mohammad Kamrul Islam | Mohammad Kamrul Islam |
| [YARN-2856](https://issues.apache.org/jira/browse/YARN-2856) | Application recovery throw InvalidStateTransitonException: Invalid event: ATTEMPT_KILLED at ACCEPTED |  Critical | (resourcemanager) | Rohith | Rohith |
| [YARN-2847](https://issues.apache.org/jira/browse/YARN-2847) | Linux native container executor segfaults if default banned user detected |  Major | (nodemanager) | Jason Lowe | Olaf Flebbe |
| [YARN-2816](https://issues.apache.org/jira/browse/YARN-2816) | NM fail to start with NPE during container recovery |  Major | (nodemanager) | zhihai xu | zhihai xu |
| [YARN-2815](https://issues.apache.org/jira/browse/YARN-2815) | Remove jline from hadoop-yarn-server-common |  Major |  | Ferdinand Xu | Ferdinand Xu |
| [YARN-2811](https://issues.apache.org/jira/browse/YARN-2811) | In Fair Scheduler, reservation fulfillments shouldn't ignore max share |  Major |  | Siqi Li | Siqi Li |
| [YARN-2809](https://issues.apache.org/jira/browse/YARN-2809) | Implement workaround for linux kernel panic when removing cgroup |  Major | (nodemanager) | Nathan Roberts | Nathan Roberts |
| [YARN-2808](https://issues.apache.org/jira/browse/YARN-2808) | yarn client tool can not list app_attempt's container info correctly |  Major | (client) | Gordon Wang | Naganarasimha G R |
| [YARN-2749](https://issues.apache.org/jira/browse/YARN-2749) | Some testcases from TestLogAggregationService fails in trunk |  Major |  | Xuan Gong | Xuan Gong |
| [YARN-2742](https://issues.apache.org/jira/browse/YARN-2742) | FairSchedulerConfiguration should allow extra spaces between value and unit |  Minor | (fairscheduler) | Sangjin Lee | Wei Yan |
| [YARN-2735](https://issues.apache.org/jira/browse/YARN-2735) | diskUtilizationPercentageCutoff and diskUtilizationSpaceCutoff are initialized twice in DirectoryCollection |  Trivial | (nodemanager) | zhihai xu | zhihai xu |
| [YARN-2731](https://issues.apache.org/jira/browse/YARN-2731) | Fixed RegisterApplicationMasterResponsePBImpl to properly invoke maybeInitBuilder |  Major |  | Carlo Curino | Carlo Curino |
| [YARN-2713](https://issues.apache.org/jira/browse/YARN-2713) | "RM Home" link in NM should point to one of the RMs in an HA setup |  Major | (resourcemanager) | Karthik Kambatla | Karthik Kambatla |
| [YARN-2697](https://issues.apache.org/jira/browse/YARN-2697) | RMAuthenticationHandler is no longer useful |  Major | (resourcemanager) | Zhijie Shen | haosdent |
| [YARN-2675](https://issues.apache.org/jira/browse/YARN-2675) | containersKilled metrics is not updated when the container is killed during localization |  Major | (nodemanager) | zhihai xu | zhihai xu |
| [YARN-2637](https://issues.apache.org/jira/browse/YARN-2637) | maximum-am-resource-percent could be respected for both LeafQueue/User when trying to activate applications. |  Critical | (resourcemanager) | Wangda Tan | Craig Welch |
| [YARN-2461](https://issues.apache.org/jira/browse/YARN-2461) | Fix PROCFS_USE_SMAPS_BASED_RSS_ENABLED property in YarnConfiguration |  Minor |  | Ray Chiang | Ray Chiang |
| [YARN-2432](https://issues.apache.org/jira/browse/YARN-2432) | RMStateStore should process the pending events before close |  Major | (resourcemanager) | Varun Saxena | Varun Saxena |
| [YARN-2414](https://issues.apache.org/jira/browse/YARN-2414) | RM web UI: app page will crash if app is failed before any attempt has been created |  Major | (webapp) | Zhijie Shen | Wangda Tan |
| [YARN-2356](https://issues.apache.org/jira/browse/YARN-2356) | yarn status command for non-existent application/application attempt/container is too verbose  |  Minor | (client) | Sunil G | Sunil G |
| [YARN-2340](https://issues.apache.org/jira/browse/YARN-2340) | NPE thrown when RM restart after queue is STOPPED. There after RM can not recovery application's and remain in standby |  Critical | (resourcemanager , scheduler) | Nishan Shetty | Rohith |
| [YARN-2315](https://issues.apache.org/jira/browse/YARN-2315) | FairScheduler: Set current capacity in addition to capacity |  Major |  | zhihai xu | zhihai xu |
| [YARN-2246](https://issues.apache.org/jira/browse/YARN-2246) | Job History Link in RM UI is redirecting to the URL which contains Job Id twice |  Major | (webapp) | Devaraj K | Devaraj K |
| [YARN-2230](https://issues.apache.org/jira/browse/YARN-2230) | Fix description of yarn.scheduler.maximum-allocation-vcores in yarn-default.xml (or code) |  Minor | (client , documentation , scheduler) | Adam Kawa | Vijay Bhat |
| [YARN-2136](https://issues.apache.org/jira/browse/YARN-2136) | RMStateStore can explicitly handle store/update events when fenced |  Major |  | Jian He | Varun Saxena |
| [YARN-1703](https://issues.apache.org/jira/browse/YARN-1703) | Too many connections are opened for proxy server when applicationMaster UI is accessed. |  Critical |  | Rohith | Rohith |
| [YARN-1615](https://issues.apache.org/jira/browse/YARN-1615) | Fix typos in description about delay scheduling |  Trivial | (documentation , scheduler) | Akira AJISAKA | Akira AJISAKA |
| [YARN-1580](https://issues.apache.org/jira/browse/YARN-1580) | Documentation error regarding "container-allocation.expiry-interval-ms" |  Trivial | (documentation) | German Florez-Larrahondo | Brahma Reddy Battula |
| [YARN-1237](https://issues.apache.org/jira/browse/YARN-1237) | Description for yarn.nodemanager.aux-services in yarn-default.xml is misleading |  Minor | (documentation) | Hitesh Shah | Brahma Reddy Battula |
| [YARN-933](https://issues.apache.org/jira/browse/YARN-933) | Potential InvalidStateTransitonException: Invalid event: LAUNCHED at FINAL_SAVING |  Major | (resourcemanager) | J.Andreina | Rohith |
| [YARN-570](https://issues.apache.org/jira/browse/YARN-570) | Time strings are formated in different timezone |  Major | (webapp) | Peng Zhang | Akira AJISAKA |


### TESTS:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11432](https://issues.apache.org/jira/browse/HADOOP-11432) | Fix SymlinkBaseTest#testCreateLinkUsingPartQualPath2 |  Major | (fs) | Liang Xie | Liang Xie |
| [HADOOP-11358](https://issues.apache.org/jira/browse/HADOOP-11358) | Tests for encryption/decryption with IV calculation overflow |  Major | (security , test) | Yi Liu | Yi Liu |
| [HADOOP-11165](https://issues.apache.org/jira/browse/HADOOP-11165) | TestUTF8 fails when run against java 8 |  Minor | (test) | Ted Yu | Stephen Chu |
| [HADOOP-11125](https://issues.apache.org/jira/browse/HADOOP-11125) | Remove redundant tests in TestOsSecureRandom |  Major |  | Ted Yu | Masanori Oyama |
| [HADOOP-10668](https://issues.apache.org/jira/browse/HADOOP-10668) | TestZKFailoverControllerStress#testExpireBackAndForth occasionally fails |  Major | (test) | Ted Yu | Ming Ma |
| [HDFS-7585](https://issues.apache.org/jira/browse/HDFS-7585) | Get TestEnhancedByteBufferAccess working on CPU architectures with page sizes other than 4096 |  Major | (test) | sam liu | sam liu |
| [HDFS-7475](https://issues.apache.org/jira/browse/HDFS-7475) | Make TestLazyPersistFiles#testLazyPersistBlocksAreSaved deterministic  |  Major | (test) | Xiaoyu Yao | Xiaoyu Yao |
| [HDFS-7448](https://issues.apache.org/jira/browse/HDFS-7448) | TestBookKeeperHACheckpoints fails in trunk build |  Minor |  | Ted Yu | Akira AJISAKA |
| [YARN-3070](https://issues.apache.org/jira/browse/YARN-3070) | TestRMAdminCLI#testHelp fails for transitionToActive command |  Minor |  | Ted Yu | Junping Du |
| [YARN-2930](https://issues.apache.org/jira/browse/YARN-2930) | TestRMRestart#testRMRestartRecoveringNodeLabelManager sometimes fails against Java 7 &amp; 8 |  Minor |  | Ted Yu | Wangda Tan |
| [YARN-1979](https://issues.apache.org/jira/browse/YARN-1979) | TestDirectoryCollection fails when the umask is unusual |  Major |  | Vinod Kumar Vavilapalli | Vinod Kumar Vavilapalli |
| [YARN-1537](https://issues.apache.org/jira/browse/YARN-1537) | TestLocalResourcesTrackerImpl.testLocalResourceCache often failed |  Major | (nodemanager) | Hong Shen | Xuan Gong |


### OTHER:

| JIRA | Description | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HADOOP-11612](https://issues.apache.org/jira/browse/HADOOP-11612) | Workaround for Curator's ChildReaper requiring Guava 15+ |  Major |  | Robert Kanter | Robert Kanter |
| [HADOOP-11492](https://issues.apache.org/jira/browse/HADOOP-11492) | Bump up curator version to 2.7.1 |  Major |  | Karthik Kambatla | Arun Suresh |
| [HADOOP-11489](https://issues.apache.org/jira/browse/HADOOP-11489) | Dropping dependency on io.netty from hadoop-nfs' pom.xml |  Minor | (nfs) | Ted Yu | Ted Yu |
| [HADOOP-11463](https://issues.apache.org/jira/browse/HADOOP-11463) | Replace method-local TransferManager object with S3AFileSystem#transfers |  Major | (fs/s3) | Ted Yu | Ted Yu |
| [HDFS-2486](https://issues.apache.org/jira/browse/HDFS-2486) | Review issues with UnderReplicatedBlocks |  Minor | (namenode) | Steve Loughran | Uma Maheswara Rao G |
| [MAPREDUCE-6264](https://issues.apache.org/jira/browse/MAPREDUCE-6264) | Remove httpclient dependency from hadoop-mapreduce-client |  Major |  | Akira AJISAKA | Brahma Reddy Battula |
| [MAPREDUCE-5420](https://issues.apache.org/jira/browse/MAPREDUCE-5420) | Remove mapreduce.task.tmp.dir from mapred-default.xml |  Major |  | Sandy Ryza | James Carman |
| [YARN-3217](https://issues.apache.org/jira/browse/YARN-3217) | Remove httpclient dependency from hadoop-yarn-server-web-proxy |  Major |  | Akira AJISAKA | Brahma Reddy Battula |
| [YARN-2949](https://issues.apache.org/jira/browse/YARN-2949) | Add documentation for CGroups |  Major | (documentation , nodemanager) | Varun Vasudev | Varun Vasudev |

