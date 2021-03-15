# Linux-

## command

* wc command is count ther letter in file ex:- wc -c filename

## File Permissions

*   r - read
*   w - write
*   x - execute = running a program
*   u - user = yourself
*   g - group = can be people in the same project
*   o - other= everyone on the syystem

## change permission
*  chmod

## Permission using Numeric Mode

*  0 - No permission --
*  1 - Execute -x
*  2 - Write -w-
*  3 - Execute+Write x+w
*  4 - Read r-
*  5 - Read+Execute r+x
*  6 - Read+write r+w
*  7 - Read+write+execute rwx


## File OwnerShip

*  chown command is change the ownership of a file
*  chgrp command is change the group ownership of  a file

## File Maintenance commands 

* cp
* rm
* mv
* mkdir
* rmdir or rm -r
* chgrp
* chown

## FIle Display Commands

* cat
* more
* less
* head
* tail

## Truncate file size

* Truncate command is used to reduce the size of the files to the specifized size (Truncate -s 10 filename)

## FIlters/ Test Processors commands

* cut command is use to cut the part the files (cut -c1 filename)
* awk command is utility designed for data extraction (awk '{print $1}' fileName)
* grep and egrep command is used to search the given commands in the file
* sort command is sort in alphabatic order
* uniq command is used to filder the duplicate the character
* wc coomand is used to count the word of  the file

## Access Control List

*  user : setfacl -m u:user:rwx /path/to/file
*  group : setfacl -m g:group:rw /path/to/file
*  all : setfacl -dm "entry" /path/to/file
*  setfacl -x u:user /path/to/file
*  setfacl -b path/to/file

## Compare Files

* diff
* cmp

## compress and un-compress files 

tar command is used to compress the file and store in one container file (tar cvf filename dir) (tar xvf tarfilename )
gzip
gzip -d OR gunzip

## standard output to a file

* tee commands is used to store and view

## Talking to users

* users command is use to check the avaiable user in system admin / example "users"
* wall command is use share message to one account to another account / example "wall message"
* write command is use share message to one acount to another account / example "write message"

## System utility commands

* date command is use to tell the current date
* uptime command is use to tell how many users login and time 
* hostname command is use to show currrent user name
* uname command is use to show the name of kernel machine / ex: uname -a
* which 
* cal command is use to show the  calander 

## Processes and Jobs

* Application = service
* script
* Process (systemctl or service, ps, top = system montoring , kill = ex: kill process id, crontab = ex: min:hou:day:mon:year)
* Daemon
* Threads
* Job

## Process Management

* Background= ctrl-z, jobs and bg
* Foreground = fg
* Run process even after exit = nohup process & /dev/null 2>$1 &
* Kill a process by name- pKill
* Process Priority = nice (eg nice -n 5 process)
* process Monitoring = top
* List Process = ps

## System monitoring

* top command is used to show monitoring process
* df command is used to show the size of directorys
* dmesg command is used to show the error messageses
* iostat l command is used to show the input and output of monitoring processes
* netstat command is used to show the network protocols (eg: netstat -rnv)
* free 
* cat /proc/cpuinfo
* cat /proc/meminfo

## Log Monitoring

* Log Directory = /var/log
* boot
* chrondy = NTP
* cron
* maillog
* secure
* messages
* httpd

## System Mantenance commands

* shutdown 
* init 0-6
* reboot
* halt 

## Changing System Hostname

* hostnamectl set-hostname newhostname
* version 7 = Edit /etc/hostname
* version 6 = Edit /etc/sysconfig/network

## Finding System information

* cat /etc/redhat-release
* uname -a
* dmidecode

## system Architecure 

* Arch

## Terminal control Key

* CTRL-U - erase everthing you've tyyped on the command line
* CTRL-o - stop/kill
* CTRL-z - suspend a command
* CTRL-d -exit from an interactive program (signals end of data)

## Terminal commands

* clear - clear our screen
* exit - Exit out of the sheel, terminal or a user session
* script - THe script command stores terminal activities in a log file that can be named by user

## Recover Root Paaswd

* Restart your computer 
* Edit grup
* change pasword
* reboot
* rw init=/sysroot/bin/sh
* ctrl x
* chroot /sysroot
* passwd root
* exit

## SOS report 

* collect and package diagnostic and support data
* sos-version -version 
* sosreport - command

## Type of Linux Shells

* Gnome
* KDE
* Sh
* bash
* csh and tcsh
* ksh

* cat /etc/shells

## shell scripting

* shell (#!/bin/bash)
* comments (# comments)
* commands (echo, cp, grep etc)
* Statements (if, while, for etc)
* shell script should have executable permissions (e.g -rwx r-x r-x)

* output to screen using "echo"
* creating tasks

## Input/Output

* read
* echo


##  network commands

* ping commands is used to communicate the other server (ping servername)
* ip stands for internaet protocol 
* subnet mask associate with attach ip address and divide the ip network 
* Gateway tells yyour computer which routes you have to pick to send your traffic out and recieve in
* static means if you give your ip addr to our company and you to assign ip in your machine and rebbot the system it doesn't change if dhcp is set the ip addr will change
* interface means that you have ethernet port on laptop
* interface Mac associate with network card and it will never change

## network files and commands

* Interface Domain
* Assigning an Ip address
* Interface configuration files
* - /etc/nswitch.conf with tells the host of your ip address
* - /etc/hostname 
* - /etc/sysconfig/network
* - /etc/sysconfig/network-scripts/ifcfg-nic
* - /etc/resolv.con

## Network commands

* ping
* ifconfig
* ifup and ifdown
* netstat (eg: netstat -rnv)
* tcpdump 

## NIC information

* NIC= network interface card that is attach to your laptop
* ethtool =  query or control network driver and hardware settings

## Download files or Apps

* wget url

## Curl and ping commands

* curl commands show the web page code like html code (eg:- curl -o url)
* ping commands u can see the ip addr of web site

## FTP

* client
* - yum install ftp
* - put filename

* server
* - root access
* - rpm -qa | grep ftp
* - yum install vsftpd
* -  cd /etc/vsftpd/
* - cp vsftpd.conf vsftpd.conf.orig

## scp (secure copy protocol help to transfer computer files securely from a remote host. like ftp, but it add sec and auth)
* - protocol - set of rules used by computer communicate
* - Default SCP Port = 22 
* scp command : scp filename server@ipaddr:/dirname

## rsync- Remote Synchronization ( rsync is used transfer and synchronizing files with in the same computer or remote computer by comparing the modification times and size of files)
* - basic sysntax of rsync command
* rsync options source destination
* - install rsync in your linux machine
* yum install rsync
* - rsync a file on local machine
* tar cvf backup.tar
* mkdir /tmp/backups
* rsync -zvh backup.tar /tmp/backups/
* - rsync a directoryy on a local machine
* rsync -azvh /home/centos /tmp/backups
* - rsync a file to remote machine
* mkdir /tmp/backups
* rsync -avz backup.tar centos@ipaddr:/tmp/backups
* - rsync a file from a remote machine
* touch filename
* rsync -avzh centos@ipaddr:/home/centos/filename /tmp/backups

## System Updates and Repos

* yum (Centos), apt-get(linux), rpm (redhat linux)
* yum update -y
* upgrade = delete package
* update = preserve
* yyum remove packagename

## Advance Package Management

* iNstalling Packages
* upgrading
* Deleting
* view package details information
* Identifyy source or location infornmation
* Packages configuration files

* installed rpm package command - rpm -hiv tar-packagename.gz
* package information command - rpm -qi package-name 
* delete package name - rpm -e package-name
* package configuration - rpm -qc package-name

## RollBack Updates and patches

* yum install package
* yum upgrade package
* yum history undo package_id

## SSH and Telnet
* Telnet = un-secured connection between computer
* ssh = secured

* Two type of packages for most of the services
* - client packages
* - server packages

## Hostname/ ip lookup

* nslookup command show the server ipaddr (eg nslokup domainname)
* dig command show the server information (eg dig domain name)

## NTP 

* Purpose?
  -- Time synchronization
* File
  --  /etc/ntp.conf
* Service
  --  systemctl restart httpd
* command
  --  ntpq
  
## chronyd

* Purpose? = Time Synchronization
* package name = chronyd
* configurtion file =/etc/chronyyd.conf
* Log file = /var/log/chrony
* service file = systemctl start/restart  chronyd
* program command = chronyc.

## sendmail

* purpose? = send and recive mail
* files = /etc/mail/sendmail.mc && /etc/mail/sendmail.cf && /etc/mail
* service = systemctl restart sendmail
* command = mail -s "subject line" srk868567@gmail.com

## web server (httpd)

* Purpose = werve webpages
* service or package name = httpd
* files =/etc/http/conf/httpd.conf && /var/www/html/index.html
* service = systemctl restart httpd && systemctl enable httpd
* Log files= /var/log/httpd
        

## central logger(RSYSLog)

* purpose = generate logs or collect logs from other servers
* service or package name = rsyslog
* configuration file= /etc/rsyslog.conf
* service= systemctl restart rsyslog && systemctl enable rsyslog

## OpenLDap Installation(basically open source implementation of like active directory of protocols)

* openldap service = slapd
* start or stop the service = systemctl start enable, systemctl enable slapd
* configuration files = /etc/openldap/slapd.d

## TraceRoute

* traceroute means basically trace from source to destination
* traceroute (traceroute www.ggogle.com)

## how to open an image file

* command = imageMagick 
* command for output = display filename

## Access Remote server without password(ssh-keys)

* Two reasons to access a remote machine / Repitive logins / Automation through scripts
* key are generated at user level

* client
*  -  Generate the key && ssh-keygen
*  - copy the key to the server && ssh-copy-id root@ipaddr
*  - login from client to server

## System Run Level

* Main Run level
* 0  Shut down the system
* 1 Single-user mode usually aliased as s or S
* 6 Reboot the system

##### Other Run Level

* 2 Multiuser mode withour networking
* 3 Multiuser mode with networking
* 5 Multiuser mode with networking and GUi









