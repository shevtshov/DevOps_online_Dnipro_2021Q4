### PART 1. HYPERVISORS
1.1 Vmware vSphere, Hyper-V, Xen, KVM, RHEV	  
1.2 Types: 	  
		1. "bare-metal hypersvisor" deploys on host maschiche, should not have basic operation system	  
		2. Install on existing operation system (e.g Windows, macOS)	  
	Number of guest operating systems, Reduce disk size, Change the number of resources without Downtime, USB Redirection	  
	
	
	
	
	
vs@MacBook-Pro ~ % VBoxManage modifyvm "ubuntu_shevtsov" --groups "/Ubuntu" 
vs@MacBook-Pro ~ % VBoxManage modifyvm "ubuntu_shevtsov_2" --groups "/Ubuntu"
