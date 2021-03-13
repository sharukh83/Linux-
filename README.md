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
