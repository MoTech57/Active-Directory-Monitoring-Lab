<h1>Staying Anonymous with ProxyChains</h1>


<h2>Description</h2>
This lab demonstrates how to enhance anonymity and security while performing network reconnaissance by leveraging ProxyChains with a SOCKS5 Tor proxy. The setup routes all traffic through the Tor network, ensuring that scans and connections are obfuscated from the target system. Using tools like Nmap in combination with ProxyChains highlights how penetration testers and ethical hackers can conduct stealthier assessments while maintaining privacy. The project covers configuration of ProxyChains, integration with Tor, and practical use cases such as anonymized port scanning and service enumeration.
<br />


<h2>Languages and Utilities Used</h2>

- <b>ProxyChains</b> 
- <b>Tor (SOCKS5 proxy)</b>
- <b>Nmap</b>
- <b>SSH (remote access)</b>
- <b>Remote Desktop Client</b>
- <b>Netcat</b>
- <b>Linux networking utilities (ping, curl, etc.)</b>

<h2>Environments Used </h2>

- <b>Fedora Linux</b> 
- <b>Tor Network</b> 
- <b>Virtualized Lab Environment (VMware/VirtualBox)</b> 

<h2>Workflow:</h2>

<p align="center">
A Diagram layout for the lab so we can create a Playbook: <br/>
<img src="https://i.imgur.com/t0cOZeZ.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Three diffrenet servers need to be created two for Windows one for Ubuntu:  <br/>
<img src="https://i.imgur.com/NtiKzxm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />Test Machine Will use Windows and 55GB: <br/>
<img src="https://i.imgur.com/ZZDNoGm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />Active Directory Will use Windows 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />Splunk Will use Ubuntu 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Create Firewall Group and give name:  <br/>
<img src="https://i.imgur.com/oO1qXt8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Edit Firewall Rules:  <br/>
<https://i.imgur.com/xEYVGXc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />Splunk Will use Ubuntu 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Use RDP or SSH to access Machines:  <br/>
<img src="https://i.imgur.com/oO1qXt8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oO1qXt8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
<br/>Edit Firewall Rules:  <br/>
<https://i.imgur.com/xEYVGXc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>







</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
