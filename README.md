# Linux-

## File Permissions

1.  r - read
2.  w - write
3.  x - execute = running a program
4.  u - user = yourself
5.  g - group = can be people in the same project
6.  o - other= everyone on the syystem

## change permission
1.  chmod

## Permission using Numeric Mode

1) 0 - No permission --
2) 1 - Execute -x
3) 2 - Write -w-
4) 3 - Execute+Write x+w
5) 4 - Read r-
6) 5 - Read+Execute r+x
7) 6 - Read+write r+w
8) 7 - Read+write+execute rwx


## File OwnerShip

1) chown command is change the ownership of a file
2) chgrp command is change the group ownership of  a file


## Access Control List

1) user : setfacl -m u:user:rwx /path/to/file
2) group : setfacl -m g:group:rw /path/to/file
3) all : setfacl -dm "entry" /path/to/file
4) setfacl -x u:user /path/to/file
