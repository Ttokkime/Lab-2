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
 
 
<p align = "center"> 
This is a picture of the Ports/Hosts tab from the SYN scan for 172.30.0.10 on Zenmap
</p>


```
 nmap -O 172.30.0.0/24
```

* This command runs an OS fingerprinting scan and can see which OS or operating systems are being run on the network hosts in the subnetwork.
* This scan not only can see which TCP ports are open, but can also guess which operating systems each host had. 
* The different operating systems can be seen as the icons that are next to each host. For instance, the windows icon represents a Windows machine while the penguins represent a Linux machine. 

<p align = "center">
<img src = "https://github.com/Ttokkime/Lab-2/blob/8809509c9c8970988714982913987e5bf5ba56f2/OS%20scan%20172.30.0.2.png" width="650" height="500">
</p>
 
 
<p align = "center"> 
This is a picture of the Host Details tab from the OS scan for 172.30.0.2 on Zenmap
</p>


```
 nmap -sV 172.30.0.0/24
```

* This command unlike the previous SYN scan can identify the software versions of the TCP ports that are open and can make a guess as to which operating system each host has based on the services of each. 
* -sV  is better than the OS fingerprinting scan in that it is able to detect OS types better than -O, but the downside of this scan is that it takes a longer time to complete scans in comparison to other scanning options. 

<p align = "center">
<img src = "https://github.com/Ttokkime/Lab-2/blob/8809509c9c8970988714982913987e5bf5ba56f2/172.30.0.10%20Ports%20and%20Hosts%20Service%20scan.png" width="650" height="500">
</p>
 
 
<p align = "center"> 
This is a picture of the Ports/Hosts tab from the Service scan for 172.30.0.10 on Zenmap
</p>

## Performing vulnerability scans on target IP subnetworks using Nessus Scans
## Assessing vulnerability assessment scans in order to identify vulnerabilities
