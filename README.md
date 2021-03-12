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

## FIlters/ Test Processors commands

* cut command is use to cut the part the files (cut -c1 filename)
* awk command is utility designed for data extraction
* grep and egrep
* sort
* uniq
* wc

## Access Control List

*  user : setfacl -m u:user:rwx /path/to/file
*  group : setfacl -m g:group:rw /path/to/file
*  all : setfacl -dm "entry" /path/to/file
*  setfacl -x u:user /path/to/file
*  setfacl -b path/to/file

## standard output to a file

* tee commands is used to store and view
