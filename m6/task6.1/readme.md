## Networking with Linux

2. VM2 has one interface (internal), VM1 has 2 interfaces (NAT and internal). Configure all network interfaces in order to make VM2 has an access to the Internet (iptables, forward, masquerade).  

![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/1.1.png)
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/1.png)

Steps:
```
- set portforwarding in virtualbox settings for VM1 machine
- interfaces enp03s, enp08s setting 

VM1:
sudo ip addr add 192.168.1.1/255.255.255.0 broadcast 192.168.1.255 dev enp0s8
sudo ip link set enp0s8 up
VM2:
sudo ip addr add 192.168.1.1/255.255.255.0 broadcast 192.168.1.255 dev enp0s8
sudo ip link set enp0s3 up

Set 1 in ip_forward file /proc/sys/net/ipv4/ip_forward
set iptables rules:
  iptables -t nat -A PREROUTING -p tcp -i eth0 --dport 2222 -j DNAT --to-destination 192.168.1.10:22
  iptables -t nat -A POSTROUTING -o enp0s3 -j MASQUERADE
  ```
  
  
  5. `whois 8.8.8.8` or `nslookup 8.8.8.8`  
  ![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/5.png)
  ![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/5.1.png)


  6. `dig epam.com`
  ![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/6.png)

  7. `ping _getaway`
  ![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/7.png)

  8. `traceroute google.com`
  ![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m6/task6.1/images/8.png)
