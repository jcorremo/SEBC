##### Cloud Provider

AWS

##### Instances 

1. 172.31.0.2 ip-172-31-18-41
2. 172.31.0.2 ip-172-31-31-18
3. 172.31.0.2 ip-172-31-20-230
4. 172.31.0.2 ip-172-31-16-219

##### Linux release

CentOS Linux release 7.3.1611 (Core)

##### File system capacity for the first node

Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       80G  1.4G   79G   2% /
devtmpfs         16G     0   16G   0% /dev
tmpfs            16G     0   16G   0% /dev/shm
tmpfs            16G  292K   16G   1% /run
tmpfs            16G     0   16G   0% /sys/fs/cgroup
/dev/xvde        50G   33M   50G   1% /var/lib/mesos
/dev/xvdf       100G   33M  100G   1% /var/lib/docker
/dev/xvdg        50G   33M   50G   1% /dcos/volume0
/dev/xvdh        20G   49M   20G   1% /var/log
tmpfs           3.2G     0  3.2G   0% /run/user/1000


##### Comand

Loaded plugins: fastestmirror
base                                                     | 3.6 kB     00:00
extras                                                   | 3.4 kB     00:00
updates                                                  | 3.4 kB     00:00
(1/4): base/7/x86_64/group_gz                              | 155 kB   00:00
(2/4): base/7/x86_64/primary_db                            | 5.6 MB   00:00
(3/4): extras/7/x86_64/primary_db                          | 191 kB   00:00
(4/4): updates/7/x86_64/primary_db                         | 7.8 MB   00:00
Determining fastest mirrors
 * base: mirror.umd.edu
 * extras: www.gtlib.gatech.edu
 * updates: bay.uchicago.edu
repo id                             repo name                             status
base/7/x86_64                       CentOS-7 - Base                       9,363
extras/7/x86_64                     CentOS-7 - Extras                       449
updates/7/x86_64                    CentOS-7 - Updates                    2,130
repolist: 11,942


##### List the /etc/passwd 

saturn:x:2800:1002::/home/saturn:/bin/bash
haley:x:2900:2801::/home/haley:/bin/bash

##### List the /etc/group

comets:x:2802:haley
planets:x:2803:saturn


