🖥️ <h1>Active Directory monitoring lab</h1> 🖥️ 


<h2>Description</h2>
This project demonstrates an Active Directory security monitoring lab hosted on Vultr virtual machines. A Windows Server domain controller and a test Windows machine were configured under the domain MyDFIR.local, with telemetry forwarded to a Splunk server running on Ubuntu. Using Remote Desktop and SSH, I managed the lab and generated authentication events for analysis. Splunk ingested the logs and triggered alerts on unauthorized logins, which then activated an automated playbook in Shuffle. The playbook sent notifications to a SOC analyst through Slack and email, giving them the option to disable the compromised domain account. This lab showcased how Active Directory, Splunk, and SOAR automation can work together to detect and respond to account compromises in a realistic enterprise setting..
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Splunk</b>
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
<img src="https://i.imgur.com/t0cOZeZ.jpeg" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
Three different servers need to be created: two for Windows, one for Ubuntu:  <br/>
<img src="https://i.imgur.com/NtiKzxm.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />Test Machine Will use Windows and 55GB: <br/>
<img src="https://i.imgur.com/ZZDNoGm.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />Active Directory will use Windows 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />Splunk Will use Ubuntu 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Create Firewall Group and give name:  <br/>
<img src="https://i.imgur.com/oO1qXt8.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Edit Firewall Rules:  <br/>
<https://i.imgur.com/xEYVGXc.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />Splunk Will use Ubuntu 80GB:  <br/>
<img src="https://i.imgur.com/eewx2iC.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>Use RDP or SSH to access Machines:  <br/>
<img src="https://i.imgur.com/bc14zKk.png" height="70%" width="70%%" alt="Disk Sanitization Steps"/>
 <br/>
 <br/>
<img src="https://i.imgur.com/UVIlZBA.png" height="70%" width="70%%" alt="Disk Sanitization Steps"/>

<br />
<br />
<br/>Verify IP in terminal with ip a or ipconfig <br/>
<img src="https://i.imgur.com/O4kUfQB.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/gAefKCd.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ycDLNpH.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br/>Install and configure Active Directory, promote to Domain Controller <br/>
<img src="https://i.imgur.com/gfhrgWh.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/OWBlaxS.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9Ee5cVJ.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

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
