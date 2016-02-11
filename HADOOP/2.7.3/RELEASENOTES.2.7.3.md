# Apache Hadoop  2.7.3 Release Notes

These release notes cover new developer and user-facing incompatibilities, important issues, features, and major improvements.


---

* [MAPREDUCE-5485](https://issues.apache.org/jira/browse/MAPREDUCE-5485) | *Critical* | **Allow repeating job commit by extending OutputCommitter API**

Previously, the MR job will get failed if AM get restarted for some reason (like node failure, etc.) during its doing commit job no matter if AM attempts reach to the maximum attempts. 
In this improvement, we add a new API isCommitJobRepeatable() to OutputCommitter interface which to indicate if job's committer can do commitJob again if previous commit work is interrupted by NM/AM failures, etc. The instance of OutputCommitter, which support repeatable job commit (like FileOutputCommitter in algorithm 2), can allow AM to continue the commitJob() after AM restart as a new attempt.



