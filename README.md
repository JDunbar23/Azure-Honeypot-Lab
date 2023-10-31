<h1>Azure Failed RDP to IP Geolocation Honeypot Project</h1>

<h2>Description</h2>
The PowerShell script contained within this repository is designed to extract data from Windows Event Logs regarding unsuccessful RDP intrusion attempts. It then employs a third-party API to gather geographical data related to the origin of the attackers.
<br />
<br />
This script is utilized in the context of my Azure Sentinel configuration, where it is connected to a live virtual machine serving as a decoy for potential cyberattacks. I have personally witnessed live attacks, particularly RDP brute force attacks, originating from various locations worldwide. To visualize this information, I utilized a custom PowerShell script to retrieve the geographic information of the attackers and visualize it on an Azure Sentinel map.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Virtual Machine</b> 
- <b>Windows 10</b>
- <b>Azure Sentinel</b> 
- <b>PowerShell: Extract RDP failed logon logs from Windows Event Viewerl</b> 
- <b>ipgeolocation.io: IP Address to Geolocation API</b>


<h2>Walkthrough</h2>

Virtual Machine under attack from multiple locations <br/>
<img src="https://i.imgur.com/MOYc8Pq.png" height="80%" width="80%" alt="Powershell ISE"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>World Map of incoming attacks</h2>
<img src="https://i.imgur.com/vbx7950.png" height="80%" width="80%" alt="Azure Attack Map"/>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
