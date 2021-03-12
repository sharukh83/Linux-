# Linux-

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


## Access Control List

*  user : setfacl -m u:user:rwx /path/to/file
*  group : setfacl -m g:group:rw /path/to/file
*  all : setfacl -dm "entry" /path/to/file
*  setfacl -x u:user /path/to/file
*  setfacl -b path/to/file
