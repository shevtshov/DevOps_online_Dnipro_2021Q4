## Linux
### Part 3.1

3.1.1 
Four states: Running,  Sleep(Uninterruptible/Interruptable), Stopped, Zombie   
3.1.2
`pstree` - tool to view a list of child processes for a specific process. `pstree $$` - to see current process tree (`$$` is the process ID of the script itself)  
3.1.3
`procfs` - a file system to retrieve information from the kernel. The /proc contains the files and directories that provide information about the system.   
3.1.4
`cat /proc/cpuinfo`  
3.1.5
`ps -f`  
3.1.6
Define kernel processes - 1st define kthread PID, then `ps --ppid kthread` ; user processes - `ps -u username`    
3.1.7
top or `ps -F` (-e for printing all processes); the status of process could be output: `ps -q PID -o state`  
3.1.8
`ps -u username`  
3.1.9
htop - with this utility you can see the same information as in ps, you can also filter or kill processes   
3.1.10
top - shows dynamic information about the system: list of processes, resources used   
3.1.11
when top is output - click on u and enter the username  
3.1.12
`l` - hide/show avarage system load; `d` - change delay board updating (seconds)  
3.1.13
`top -O` (check allowed fields for sorting), `top -o %CPU`  
3.1.14
Priority means how much more/less processor time the process will have. e.g change prio for process by PID `renice -n 15 -p 1262`  
3.1.15
yes, click on `r` in the intaractive mode, then enter prio value e.g "15"  
3.1.16
find require process PID e.g `ps a | grep ping`, then kill by PID number e.g `kill 123`. SIGKILL(9) - kill process; SIGSTOP(23) - stop process  
3.1.17
`jobs` - list of current background tasks; `bg` - move task in background mode; `fg` - move task in foreground mode; `nohup` - running command with signals ignoring

### Part 3.2

3.2.1
`ssh user@host` - to connect to the server; `scp -p *.txt` `user@host` - copy files. (I have no Windows to demonstrate these commands)  
3.2.2
change port in /etc/ssh/ssh_config file; disable root logins in /etc/ssh/sshd_config `PermitRootLogin no`  
3.2.3

3.2.4

3.2.5


![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.3/2.png)  
