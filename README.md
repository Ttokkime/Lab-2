# Lab 2: Performing a Vulnerability Assesment

<p align = "center">
<img src = "https://github.com/Ttokkime/Lab-2/blob/439648fd216411c651c7f8b93319827016534dc8/Lab%202%20topology.png">
</p>

## Identifying risks, threats, and vulnerabilities in IP network structures using Zenmap
```
 nmap -sn 172.30.0.0/24
```

* By using this command in Zenmap, I was able to conduct a SYN scan on the subnet and thus do a TCP scan on the target host. 
* This way is an overall less intrusive in comparison to other methods of scanning because of how Zenmap does not need to complete the TCP handshake in order to identify open ports. 
* The scan was able to identify services, but it was not able to identify the specifics such as what the versions of these services were. 


## Performing vulnerability scans on target IP subnetworks using Nessus Scans
## Assessing vulnerability assessment scans in order to identify vulnerabilities
