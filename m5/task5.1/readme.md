## Linux
### Part 1.

1.1 Log in to the system as root  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.1.png)

1.2 Linux passwords are stored in the /etc/shadow file   
1.3 Users registred in system: */etc/passwd*. Users command history: *cat /home/home_directory/.bash_history*  
1.4  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.4.png)   
1.5  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.5.png)   
- root@vs-VirtualBox:/home/vs# man -f ls (short description)
- root@vs-VirtualBox:/home/vs# man -k ls (brief descriptions of reference pages)

1.6  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.6_less.png)  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.6_more.png)  
- more /home/vs/.bash_history, less /home/vs/.bash_history   


1.7   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.7.png)   
1.8   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/1.8.png)   



### Part 2.
2.1   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.1.png)  
2.2   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.2.png)  
2.3   *"cd" or "cd ~"*   

2.4  
- "ls -l" listening with additional information (owner, group, date of creation)  
-  "ls -a" also shows hidden files   


2.5   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.5.png)   
2.6   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.6.png)   
2.7  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.7.png)   
2.8  "mount -l"  
2.9  
- "mount -l | wc -l" number of line  
- "mount -l | wc -m" number of characters   


2.10  'find /etc/ -type f -name "host*"'   
2.11   
- 'find /etc/ -name "ss*"' 
- 'grep -r "ss*" /etc'  


2.12  vs@vs-VirtualBox:~$ ls /etc/ | less
2.13  ls -l /dev/,   type can be checked by *file* comman
- c - character
- b - block
- p - pipe
- s - socket


2.14  *file* command, e.g:  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.1/2.14.png)    
2.15  ls -1lt | head -6
