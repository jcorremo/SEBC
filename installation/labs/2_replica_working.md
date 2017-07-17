
#########   REPLICACION

#######(Master)
mysql -u user -p password

GRANT REPLICATION SLAVE ON *.* TO 'root'@'ip-172-31-23-55' IDENTIFIED BY 'jaimito12';

SET GLOBAL binlog_format = 'ROW'; 

FLUSH TABLES WITH READ LOCK;

SHOW MASTER STATUS;

UNLOCK TABLES;

#######(Maquina dos)


CHANGE MASTER TO MASTER_HOST='HostMaster', MASTER_USER='userReplica', MASTER_PASSWORD='passwordReplica', MASTER_LOG_FILE='', MASTER_LOG_POS=master file offset;

START SLAVE;

SHOW SLAVE STATUS \G

