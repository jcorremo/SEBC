##### INPUT

sudo sysctl vm.swappiness=1

##### OUTPUT

vm.swappiness = 1


##### MOUNT DISK


mkfs -t ext4 /dev/xvdc
mkfs -t ext4 /dev/xvdb
mkdir /data/
mkdir /data/d1
mkdir /data/d2

mount /dev/xvdb /data/d1/
mount /dev/xvdc /data/d2/

cp /etc/fstab /etc/fstab.bak


echo "/dev/xvdb       /data/d1/   ext4    defaults" >> /etc/fstab
echo “/dev/xvdc       /data/d2/   ext4    defaults” >> /etc/fstab


##### LIST SIDK

##### INPUT

sudo lsblk

##### OUTPUT


NAME    MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
xvda    202:0    0  40G  0 disk
+-xvda1 202:1    0  40G  0 part /
xvdb    202:16   0  40G  0 disk /data/d1
xvdc    202:32   0  40G  0 disk /data/d2


##### Disable transparent hugepage support

sudo echo never > /sys/kernel/mm/transparent_hugepage/defrag
sudo echo never > /sys/kernel/mm/transparent_hugepage/enabled

##### List your network interface configuration

##### INPUT

ip link show

##### OUTPUT


1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN mode DEFAULT qlen 1
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP mode DEFAULT qlen 1000
    link/ether 0e:5f:87:12:9a:84 brd ff:ff:ff:ff:ff:ff

##### INPUT

netstat -i

##### OUTPUT

Kernel Interface table
Iface      MTU    RX-OK RX-ERR RX-DRP RX-OVR    TX-OK TX-ERR TX-DRP TX-OVR Flg
eth0      9001 12941444      0      0 0       9383085      0      0      0 BMRU
lo       65536  6829143      0      0 0       6829143      0      0      0 LRU








