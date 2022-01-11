## Linux administration with bash

### Part A. 
Script:

![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m7/task7.1/images/script.png)

Outputs: 

1. When starting without parameters, it will display a list of possible keys and their description.
2. The --all key displays the IP addresses and symbolic names of all hosts in the current subnet
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m7/task7.1/images/output1.png)

3. The --target key displays a list of open system TCP ports.
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m7/task7.1/images/output2.png)

### Part B. 

Script:

```
#!/bin/bash

echo Most reuested IP:
cat apache_logs.txt | awk '{print $1}' | sort | uniq -c | sort -nr | head -n 1




echo Most requested page:
cat apache_logs.txt | awk '{print $11}' | sort | uniq -c | sort -nr | head -n 2 | awk 'NR!=1 {print}'


echo Number of requests from each IP:
cat apache_logs.txt | awk '{print $1}' | sort | uniq -c | sort -nr | head 


echo Non-existent pages:
cat apache_logs.txt | grep /error404

echo "Most requests time:"
cat apache_logs.txt | awk '{print $4}' | sort | uniq -c | sort -nr | head -n 1


echo List of search bots:
cat apache_logs.txt | awk '{print $14}' | sort | uniq -c | sort -nr | awk '/[Bb]ot/{print}'

```
to process another file - use $1 variable instead of apache_logs.txt 

Script output:
![alt text](https://github.com/shevtshov/DevOps_online_Dnipro_2021Q4/blob/main/m7/task7.1/images/script_output.png)
