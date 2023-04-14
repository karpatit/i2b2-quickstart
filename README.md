installs i2b2 hive and webclient on centos vm, amazon webservice and Docker  (see wiki for details)

###Quickstart

1) ssh to the aws instance

2) sudo yum -y install git wget unzip patch bzip2 screen

3)  sudo su -
 
4) cd /opt

5) mkdir git && cd git

6) git clone https://github.com/karpatit/i2b2-quickstart.git

7) cd i2b2-quickstart

8) sudo sh scripts/install/centos_first_install.sh 2>&1|tee first.log

9) Remember to use the **public/external IP_ADDRESS** of the instance in the cmd above.

10) To verify installation see: http://[ipaddress]/webclient/

Paper: https://escholarship.org/content/qt24j4f80p/qt24j4f80p_noSplash_d2dc96ea753c6a798364b61dd88ddcef.pdf

"we tested the performance of the quickstart package on a virtual machine in the Amazon Cloud environment using CentOS 7 as the operating system.
We carried out our experiment using Amazon EC2 instance of type t2.medium, having 2 cores, 4 GB memory, and 20 GB disk space"
