## Linux
### Part 2.

2.1

`etc/passwd` fields - `login : password : UID : GID : GECOS : home : shell`  
`etc/group` fields - `group_name:password:GID:user_list`  

2.2
`UID` - user's ID. From 1000 to 60000 for regular users, root - 0  

2.3
`GID` - user's group ID. Example: `id root`  
2.4
`id username`  
2.5
`sudo useradd username -m` create home directory, `useradd -D` check all default parametrs when creating  
2.6
`sudo usermod -l new_name old_name`  
2.7
`/skell_dir` - directory contains the data that will be copied to the home directory when a new user is created  
2.8
`userdel` with `--remove-all-files`  parameter  
2.9
lock: `passwd -l user_name`, unlock: `passwd -u user_name`  
2.10
`passwd -d username`  
2.11
`ls -l` information with owner,group,created date, size etc.  
2.12
file owner, group owner of the file or other users. r=Readable, w=Writeable, x = Executable, - = Denied  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.2.12.png)  

2.13
this can be checked with the command `ls -l`, to see the owner of the file and group access. then you can check the users which are in the group  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.2.13.png)  

2.14
`chown` - change owner of the file, `chmod` - change mod access (ugo - user,group,others. rwx - the same as 1.12). Examples:  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.2.14_chown.png)   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.3.14_chmod.png)    


2.15
Octal representation is the matching of permissions to values:  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/octal.png)  

`umask` is the preset permissions for new files to be created  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.2.15.png)

2.16
sticky bits - the last special permission bit. if this bit is set for file or directory, the files in the directory can only be deleted by owner.  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.2/5.2.16.pnng.png)  

2.17
immutable – “i” append only – “a” compressed – “c” no dump – “d” secure deletition – “s” no atime updates – “A”
