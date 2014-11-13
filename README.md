BigDataWK
=========
What's wrong with this?How could I solve this problem.
=========================================================================================
14/11/13 14:42:19 WARN mapred.JobClient: No job jar file set.  User classes may not be found. See JobConf(Class) or JobConf#setJar(String).
14/11/13 14:42:19 INFO mapred.JobClient: Cleaning up the staging area file:/tmp/hadoop-Administrator/mapred/staging/Administrator1811149864/.staging/job_local_0001
Exception in thread "main" java.lang.RuntimeException: java.lang.InstantiationException
	at org.apache.hadoop.util.ReflectionUtils.newInstance(ReflectionUtils.java:115)
	at org.apache.hadoop.mapred.JobClient$2.run(JobClient.java:946)
	at org.apache.hadoop.mapred.JobClient$2.run(JobClient.java:912)
	at java.security.AccessController.doPrivileged(Native Method)
	at javax.security.auth.Subject.doAs(Unknown Source)
	at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1149)
	at org.apache.hadoop.mapred.JobClient.submitJobInternal(JobClient.java:912)
	at org.apache.hadoop.mapreduce.Job.submit(Job.java:500)
	at org.apache.hadoop.mapreduce.Job.waitForCompletion(Job.java:530)
	at cn.edu.cqu.hadoop.sampling.Sampling.main(Sampling.java:52)
Caused by: java.lang.InstantiationException
	at sun.reflect.InstantiationExceptionConstructorAccessorImpl.newInstance(Unknown Source)
	at java.lang.reflect.Constructor.newInstance(Unknown Source)
	at org.apache.hadoop.util.ReflectionUtils.newInstance(ReflectionUtils.java:113)
	... 9 more
