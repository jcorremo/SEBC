##### Repo

ls /etc/yum.repos.d

CentOS-Base.repo  CentOS-Debuginfo.repo  CentOS-Media.repo    CentOS-Vault.repo          cloudera-manager.repo
CentOS-CR.repo    CentOS-fasttrack.repo  CentOS-Sources.repo  cloudera_init_mariadb.sql

##### Cloudera Server to DataBase

sudo /usr/share/cmf/schema/scm_prepare_database.sh mysql -uroot -p scm scm scm

sudo service cloudera-scm-server start

