Provider: AWS

Instances

CASALS_1 52.210.133.119	(172.31.47.175)		i-001da571dd63a9a9e: ec2-52-210-133-119.eu-west-1.compute.amazonaws.com
CASALS_2 54.72.197.46	(172.31.38.205)		i-03c509baafc6e521b: ec2-54-72-197-46.eu-west-1.compute.amazonaws.com
CASALS_3 52.215.3.80	(172.31.33.235)		i-065645d249a65f22c: ec2-52-215-3-80.eu-west-1.compute.amazonaws.com
CASALS_4 52.212.150.250	(172.31.38.247)		i-0a53f8f8cb82934c2: ec2-52-212-150-250.eu-west-1.compute.amazonaws.com
CASALS_5 54.76.154.127	(172.31.34.131)		i-0d9216306788dad67: ec2-54-76-154-127.eu-west-1.compute.amazonaws.com

cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.0 (Maipo)

uname -a
Linux ip-172-31-47-175.eu-west-1.compute.internal 3.10.0-123.8.1.el7.x86_64 #1 SMP Mon Aug 11 13:37:49 EDT 2014 x86_64 x86_64 x86_64 GNU/Linux

df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2      6.0G  1.6G  4.4G  27% /
devtmpfs         32G     0   32G   0% /dev
tmpfs            32G     0   32G   0% /dev/shm
tmpfs            32G   17M   32G   1% /run
tmpfs            32G     0   32G   0% /sys/fs/cgroup

yum repolist enabled
Loaded plugins: amazon-id, rhui-lb
cloudera-manager                                                                                                                                  |  951 B  00:00:00
rhui-REGION-client-config-server-7                                                                                                                | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                                                                                  | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                                                                                 | 3.8 kB  00:00:00
cloudera-manager/primary                                                                                                                          | 4.3 kB  00:00:00
cloudera-manager                                                                                                                                                     7/7
repo id                                                                   repo name                                                                                status
cloudera-manager                                                          Cloudera Manager                                                                              7
rhui-REGION-client-config-server-7/x86_64                                 Red Hat Update Infrastructure 2.0 Client Configuration Server 7                               6
rhui-REGION-rhel-server-releases/7Server/x86_64                           Red Hat Enterprise Linux Server 7 (RPMs)                                                 14,282
rhui-REGION-rhel-server-rh-common/7Server/x86_64                          Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                          228


adduser zhou;adduser chen
vi /etc/passwd

groupadd shangai
groupadd beijing
usermod -a -G shangai zhou
usermod -a -G shangai chen
usermod -a -G beijing zhou
usermod -a -G beijing chen

zhou:x:2800:1001::/home/zhou:/bin/bash
chen:x:2900:1002::/home/chen:/bin/bash

shangai:x:1003:zhou,chen
beijing:x:1004:zhou,chen







