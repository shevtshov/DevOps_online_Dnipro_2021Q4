## Configuring DHCP, DNS servers and dynamic routing using OSPF protocol

1. Settings for three VMs:

![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.2/images/6.2.1.png)

2. Steps for install and settings dnsmasq:
```
VM1:
apt install dnsmasq
configuring DHCP /etc/dnsmasq.conf
  port=5530
  interface=enp0s8
  dhcp-range=192.168.1.10,192.168.1.150,24h
  dhccp-option=option:router,192.168.1.1
 
enadling DNS
  nameserver 127.0.0.1 in /etc/resolv.conf
  prepend domain-name-servers 127.0.0.1 in /etc/dhcp/dhclient.conf
  
VM2,VM3:
  /etc/netplan/*.yaml:
    enp0s3:
      dhcp4: true
      dhcp6: no

```

`systemctl status dnsmasq.service`
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.2/images/6.2.2.png)

check `iptables -S` for existence rules from previos task
