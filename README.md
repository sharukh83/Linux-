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
