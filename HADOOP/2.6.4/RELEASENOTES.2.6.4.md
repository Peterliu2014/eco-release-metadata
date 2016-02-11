# Apache Hadoop  2.6.4 Release Notes

These release notes cover new developer and user-facing incompatibilities, important issues, features, and major improvements.


---

* [YARN-3154](https://issues.apache.org/jira/browse/YARN-3154) | *Blocker* | **Should not upload partial logs for MR jobs or other "short-running' applications**

Applications which made use of the LogAggregationContext in their application will need to revisit this code in order to make sure that their logs continue to get rolled out.



