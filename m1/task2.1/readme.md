### PART 1. HYPERVISORS
1.1 Vmware vSphere, Hyper-V, Xen, KVM, RHEV

1.2 Types: 	  
- "bare-metal hypersvisor" deploys on host maschiche, should not have basic operation system	  
-  Install on existing operation system (e.g Windows, macOS)	  
- Number of guest operating systems, Reduce disk size, Change the number of resources without Downtime, USB Redirection	  

1.4 Created VM1   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.4_create_VM1.png)
- ubuntu version:  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.4_create_VM1_ubuntu_version.png)

1.7 Groups for VMs   

vs@MacBook-Pro ~ % VBoxManage modifyvm "ubuntu_shevtsov" --groups "/Ubuntu"    
vs@MacBook-Pro ~ % VBoxManage modifyvm "ubuntu_shevtsov_2" --groups "/Ubuntu"   

![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.7_groups_for_VMs.png)

1.8 Snapshots functionality  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.8_snapshots.png)

1.9 Export/Import VMs   
- Exported *.ova file:   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.9_%20export_ova.png)

- Import from *.ova file:   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/1.9_import_ova.png)

 ---
   
### PART 2. Configuration of virtual machines
2.2 USB configuration  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/2.2_USB_configuration.png)

2.3 Shared folder  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/2.3_shared_folder.png)

2.4 Network modes table  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/2.4_network_modes.png)

---

### PART 3. WORK WITH VAGRANT

3.4 "vagrant up" logs  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/3.4_vagrant_up_logs.png)

3.5 Connect to VM using Termius  
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/3.5_connect_via_termius.png)

3.6 "date" inside Vagrant VM   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/3.6_date_command.png)

3.8 Own Vagrant box   
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m1/task2.1/3.8_vagrant_box.png)

