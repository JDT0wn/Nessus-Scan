# Nessus-Scan

<p>
  Vulnerability Assessment with Kali Linux and Nessus
Platform: VMware | Tools Used: Kali Linux, Tenable Nessus

Project Overview:
In this lab, I configured a virtual machine to run Kali Linux and installed Tenable Nessus to perform a vulnerability assessment on my host machine. This project demonstrated my ability to identify, analyze, and recommend solutions for security vulnerabilities in a controlled environment.

Key Tasks and Skills Demonstrated:

Configured a Kali Linux virtual machine 

Installed and set up Tenable Nessus to scan the host system for vulnerabilities.

Performed a basic vulnerability scan, reviewing system configurations, missing patches, and potential exploit risks.

Documented the scan results, including risk levels, CVE references, and affected services.

Provided recommended remediation steps based on best practices .

<br>
</p>


</br>

<p>
<h1>Nessus installation and basic scan<h1>  
   <h2>https://youtu.be/1VlOsJKgGdo?si=VtkDJVsmGpyVZp-R </h2>
   
   <br>
   </br>
 In this lab, I conducted a vulnerability assessment using Tenable Nessus on a Kali Linux virtual machine hosted in a VMware environment. The objective was to identify potential security weaknesses on the local system and become familiar with the core functionalities of Nessus. The installation process began by using the dpkg -i command to install the Nessus 10.9 package. After installation, the Nessus service was initiated with systemctl start nessusd, and then i accessed the interface via  localhost:8834 for further configuration.
 <br>  
 </br>

Using the ifconfig command, I retrieved the IP address of the host machine to define the scan target. I then configured a basic network scan, exploring various customization options such as scan scheduling (e.g., daily or weekly), port selection (common, custom, or all), and vulnerability detection levels (quick, complex, or comprehensive). Before executing the scan, I reviewed the reporting preferences for the output such as choosing to display hostnames instead of IP addresses and deciding whether to show unreachable hosts or only those that respond to pings.

Overall, this lab provided hands-on experience with one of the industry’s most widely used vulnerability scanning tools in network assessment and threat detection.

 
  <br>
  </br>

  <h1>Scan results and remediations</h1>
</p>
  
<p>
</p>

![image](https://github.com/user-attachments/assets/228d5767-7718-4242-8257-82b79029c3b8)


<p> Description of vulnerability group: The version of Node.js installed on the remote host is prior to 18.20.6, 20.18.2, 22.13.1, 23.6.1. It is, therefore, affected by multiple vulnerabilities. 

<br>


</br>
              Vulnerabilities
  
1 critical vulnerability with a CVSS score of 9.8 <br>
3 high vulnerabilities ranging from 7.7, 8.1, 8.2 <br>
1 medium vulnerability CVSS score 6.2


<br>



</br>

  


Recommended remediation for these vulnerabilites would be: Upgrade to Node.js version 18.20.6 / 20.18.2 / 22.13.1 / 23.6.1 or later as soon as possible. 

<br>


</br>

![image](https://github.com/user-attachments/assets/41524964-39b9-4672-81ba-26bcdb6a29b7)
![image](https://github.com/user-attachments/assets/cf38c47b-6ba6-48d6-9172-1129796820ea)

<br>



</br>


Description of vulnerability: Detected version of tornado python package pre-dates 6.4.2, possible dos vulnerability. CVSS score 7.5

<br>



</br>


Recommmended remediation: Upgrade to Tornado version 6.5.0 or later 

<br>



</br>



![image](https://github.com/user-attachments/assets/8c2dcdf3-2441-4b18-98e8-efbed7e895f7)
![image](https://github.com/user-attachments/assets/53168825-8b92-4650-9c95-7294f7f9d758)


<br>



</br>


Description of vulnerability: The server's X.509 certificate cannot be trusted,possible server authenticity/identity issues.  CVSS score 6.5

<br>

</br>

Recommmended remediation: Purchase or generate a proper SSL certificate for this service.





















