## Linux
### Part 3.1

3.1.1 Four states: Running,  Sleep(Uninterruptible/Interruptable), Stopped, Zombie  

3.1.2
`pstree` - tool to view a list of child processes for a specific process. `pstree $$` - to see current process tree (`$$` is the process ID of the script itself)  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m5/task5.3/2.png)  
3.1.3
`procfs` - a file system to retrieve information from the kernel. The /proc contains the files and directories that provide information about the system.  
3.1.4
`cat /proc/cpuinfo`
3.1.5
`ps -f`  
3.1.6
Define kernel processes - 1st define kthread PID, then `ps --ppid kthread` ; user processes - `ps -u username`  
3.1.7

3.1.8
3.1.9
3.1.10
3.1.11
3.1.12
3.1.13
3.1.14
3.1.15
3.1.16
3.1.17

### Part 3.2

3.2.1
3.2.2
3.2.3
3.2.4
3.2.5
