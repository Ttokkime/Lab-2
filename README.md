# Lab 2: Performing a Vulnerability Assesment

<p align = "center">
<img src = "https://github.com/Ttokkime/Lab-2/blob/439648fd216411c651c7f8b93319827016534dc8/Lab%202%20topology.png">
</p>

## Identifying risks, threats, and vulnerabilities in IP network structures using Zenmap
```
 nmap -sS 172.30.0.0/24
```

* By using this command in Zenmap, I was able to conduct a SYN scan on the subnet and thus do a TCP scan on the target host. 
* This way is an overall less intrusive in comparison to other methods of scanning because of how Zenmap does not need to complete the TCP handshake in order to identify open ports. 
* The scan was able to identify services, but it was not able to identify the specifics such as what the versions of these services were. 

<p align = "center">
<img src = "https://github.com/Ttokkime/Lab-2/blob/8d18e915961a7d513b555896f4e695182c26990f/172.30.0.10%20Nmap%20Ports%20and%20Hosts.png" width="700" height="550">
</p>
 
This is a picture of the Ports/Hosts tab from the SYN scan for 172.30.0.10 on Zenmap

## Performing vulnerability scans on target IP subnetworks using Nessus Scans
## Assessing vulnerability assessment scans in order to identify vulnerabilities
