###### INPUT TERASORT

sudo -u hdfs hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples-2.6.0-mr1-cdh5.11.1.jar terasort /tmp/teraInput3 /tmp/teraOutput


###### INPUT TERAGEN

sudo -u hdfs time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples-2.6.0-mr1-cdh5.11.1.jar teragen 10000000 /tmp/teraInput3