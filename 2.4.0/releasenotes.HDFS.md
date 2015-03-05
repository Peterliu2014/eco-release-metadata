# Hadoop HDFS 2.4.0 Release Notes

These release notes include new developer and user-facing incompatibilities, features, and major improvements.

## Changes since Hadoop 2.3.0

* [HDFS-6102](https://issues.apache.org/jira/browse/HDFS-6102) | Blocker | Lower the default maximum items per directory to fix PB fsimage loading

No release note provided for this incompatible change.

* [HDFS-6055](https://issues.apache.org/jira/browse/HDFS-6055) | Major | Change default configuration to limit file name length in HDFS

The default configuration of HDFS now sets dfs.namenode.fs-limits.max-component-length to 255 for improved interoperability with other file system implementations.  This limits each component of a file system path to a maximum of 255 bytes in UTF-8 encoding.  Attempts to create new files that violate this rule will fail with an error.  Existing files that violate the rule are not effected.  Previously, dfs.namenode.fs-limits.max-component-length was set to 0 (ignored).  If necessary, it is possible to set the value back to 0 in the cluster's configuration to restore the old behavior.

* [HDFS-5804](https://issues.apache.org/jira/browse/HDFS-5804) | Major | HDFS NFS Gateway fails to mount and proxy when using Kerberos

Fixes NFS on Kerberized cluster.

* [HDFS-5790](https://issues.apache.org/jira/browse/HDFS-5790) | Major | LeaseManager.findPath is very slow when many leases need recovery

Committed to branch-2 and trunk.

* [HDFS-5776](https://issues.apache.org/jira/browse/HDFS-5776) | Major | Support 'hedged' reads in DFSClient

If a read from a block is slow, start up another parallel, 'hedged' read against a different block replica.  We then take the result of which ever read returns first (the outstanding read is cancelled).  This 'hedged' read feature will help rein in the outliers, the odd read that takes a long time because it hit a bad patch on the disc, etc.

This feature is off by default.  To enable this feature, set &lt;code&gt;dfs.client.hedged.read.threadpool.size&lt;/code&gt; to a positive number.  The threadpool size is how many threads to dedicate to the running of these 'hedged', concurrent reads in your client.

Then set &lt;code&gt;dfs.client.hedged.read.threshold.millis&lt;/code&gt; to the number of milliseconds to wait before starting up a 'hedged' read.  For example, if you set this property to 10, then if a read has not returned within 10 milliseconds, we will start up a new read against a different block replica.

This feature emits new metrics:

+ hedgedReadOps
+ hedgeReadOpsWin -- how many times the hedged read 'beat' the original read
+ hedgedReadOpsInCurThread -- how many times we went to do a hedged read but we had to run it in the current thread because dfs.client.hedged.read.threadpool.size was at a maximum.

* [HDFS-5698](https://issues.apache.org/jira/browse/HDFS-5698) | Major | Use protobuf to serialize / deserialize FSImage

Use protobuf to serialize/deserialize the FSImage.

* [HDFS-5321](https://issues.apache.org/jira/browse/HDFS-5321) | Major | Clean up the HTTP-related configuration in HDFS

dfs.http.port and dfs.https.port are removed. Filesystem clients, such as WebHdfsFileSystem, now have fixed instead of configurable default ports (i.e., 50070 for http and 50470 for https).

Users can explicitly specify the port in the URI to access the file system which runs on non-default ports.

* [HDFS-5138](https://issues.apache.org/jira/browse/HDFS-5138) | Blocker | Support HDFS upgrade in HA

No release note provided for this incompatible change.

* [HDFS-4685](https://issues.apache.org/jira/browse/HDFS-4685) | Major | Implementation of ACLs in HDFS

HDFS now supports ACLs (Access Control Lists).  ACLs can specify fine-grained file permissions for specific named users or named groups.

* [HDFS-4370](https://issues.apache.org/jira/browse/HDFS-4370) | Major | Fix typo Blanacer in DataNode

I just committed this. Thank you Chu.


