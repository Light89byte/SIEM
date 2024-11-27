<h1>Brute Force RDP to IP Geo Data</h1>


 


<h2>Description</h2>
<b>The Powershell script is in charge with going through Windows Event Log data for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
This script utilizes Azure Sentinel, which is a SIEM, and connects to a live virtual machine, working as a honey pot to capture data from all over the world.
We will observe mostly live RDP Brute Force attacks attempting to break-in to my machine through intrusion. I have used a custom PowerShell script to
look up the attackers Geolocation information and mark it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
  
![image_alt](https://i.imgur.com/s3yUNo7.png)
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extracting RDP failed logons from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from Ukraine coming in; logs being output with geodata</h2>

<p align="center">
 
![image_alt](https://i.imgur.com/z4PXrqQ.png)
</p>

<h2>World map of attacks after 24 hours (logs including geodata)</h2>

<p align="center">
 
![image_alt](https://i.imgur.com/PAouWLp.png)
</p>

<br />
Interesting how this only seems to be coming from only part of the world, that mainly being Ukraine. 
I wonder what this implies....
<br />
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
