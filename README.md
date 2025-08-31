<h1>Staying Anonymous with ProxyChains</h1>


<h2>Description</h2>
This lab demonstrates how to enhance anonymity and security while performing network reconnaissance by leveraging ProxyChains with a SOCKS5 Tor proxy. The setup routes all traffic through the Tor network, ensuring that scans and connections are obfuscated from the target system. Using tools like Nmap in combination with ProxyChains highlights how penetration testers and ethical hackers can conduct stealthier assessments while maintaining privacy. The project covers configuration of ProxyChains, integration with Tor, and practical use cases such as anonymized port scanning and service enumeration.
<br />


<h2>Languages and Utilities Used</h2>

- <b>ProxyChains</b> 
- <b>Tor (SOCKS5 proxy)</b>
- <b>Nmap</b> 
- <b>Netcat</b>
- <b>Linux networking utilities (ping, curl, etc.)</b>

<h2>Environments Used </h2>

- <b>Fedora Linux</b> 
- <b>Tor Network</b> 
- <b>Virtualized Lab Environment (VMware/VirtualBox)</b> 

<h2>Workflow:</h2>

<p align="center">
Lab network created with spare router + Raspberry Pi 4 Password: test123!: <br/>
<img src="https://i.imgur.com/iKyEhx8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Monitordn.sh create to enable monitor mode:  <br/>
<img src="https://i.imgur.com/pry0CVu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Monitorup.sh create to enable managed mode: <br/>
<img src="https://i.imgur.com/4adI6dW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Discover nearby Wi-Fi networks using airodump-ng:  <br/>
<img src="https://i.imgur.com/kcFgVPw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Deauthentication to Forces client reconnection Confirm handshake in Wireshark:  <br/>
<img src="https://i.imgur.com/YNtAQoF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Locate file and send to VM with ssh:  <br/>
<img src="https://i.imgur.com/PprrkzP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Use aircrack-ng with dictionary wordlist successfully cracked - “test123!”:  <br/>
<img src="https://i.imgur.com/6pENfVx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
