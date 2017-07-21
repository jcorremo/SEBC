##### Full Comand

sudo -u saturn time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples-2.6.0-mr1-cdh5.12.0.jar  teragen  -Dmapreduce.map.memory.mb=32  -Dmapreduce.job.maps=12 -Dmapreduce.map.java.opts.max.heap=512 655360000 /user/saturn/tgen



##### Result

teragen <num rows> <output dir>
1.55user 0.11system 0:00.94elapsed 177%CPU (0avgtext+0avgdata 112348maxresident)k
0inputs+968outputs (0major+41432minor)pagefaults 0swaps
