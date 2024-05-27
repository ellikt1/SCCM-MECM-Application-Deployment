<h1>SCCM/MECM Application Deployment</h1>

 <img src="https://i.imgur.com/Wl8C0vj.png" alt="Microsoft Endpoint Configuration Manager" class="header-image">

<h2>Description</h2>
Project showcases how System Center Configuration Manager (SCCM), also known as Microsoft Endpoint Configuration Manager (MECM), is utilized to deploy applications to client work computers in a simulated work environment. The applications deployed in this demonstration are Microsoft Teams, Google Chrome, and 7-Zip. The target devices for this deployment are three workstations: WS01, WS02, and TS01, representing typical client devices in a professional setting.
<br />
<br />

<h2>Environment Used</h2>
<p>
The lab environment consists of three virtual machines: DC01 (Domain Controller), GW01 (Gateway), and CM01 (Configuration Manager).
 <br />
</p>

<b>DC01:</b>
- 1 processor (2 cores)
- 2GB of memory
- 100GB of storage
- Operates within the "CM Lab" LAN segment as the domain controller.

<b>GW01:</b>
- Similar specifications to DC01
- Serves as the gateway, enabling Wi-Fi connections to DC01 via Routing and Remote Access
- Has 2 network adapters: one configured for NAT and the other operating in the "CM Lab" LAN segment.

<b>CM01:</b>
- 1 processor (8 cores) 
- 16GB of memory
- Varying storage capacities totaling to 700GB of storage
- Operates within the "CM Lab" LAN segment and relies on DC01 for internet access.
- DC01 uses DHCP to allocate IP addresses, allowing CM01 to connect to the internet. This setup demonstrates network infrastructure configurations and management using virtualization technology.
<br />

<p> 
CM01 is the focal point of the lab environment, featuring a robust configuration that includes WSUS (Windows Server Update Services), SQL Server 2022, SQL Server Management Studio, and Configuration Manager version 2403.
<br />
</p>

- <b>WSUS:</b> Manages Windows updates across the network, ensuring timely deployment and compliance with security patches and feature upgrades.
- <b>SQL Server 2022 and SQL Server Management Studio:</b> Provide a powerful database management platform, facilitating advanced data storage, retrieval, and manipulation 
- <b>Configuration Manager version 2403:</b> Enhances system capabilities by streamlining configuration tasks, automating software deployment, and enforcing compliance standards.
<br />


<h2>Environment Topology</h2>

<img src="https://i.imgur.com/GGKYoDS.png" height="80%" width="80%" alt="Disk Sanitization Steps2"/>



<h2>Applications Deployed</h2>

- <b>Microsoft Teams: A collaboration platform developed by Microsoft, combining chat, video meetings, file storage, and application integration to enhance teamwork and communication.</b>


- <b>Google Chrome: A widely-used web browser developed by Google.</b>


- <b>7-Zip: A free and open-source file archiver utility.</b>


<h2>Utilities Used</h2>

- <b>SCCM</b>
- <b>Draw.io</b> 

<h2>Program walk-through:</h2>
The program walk-through below demonstrates the successful deployment process of Microsoft Teams to TS01. The same steps were followed, with the necessary modifications, to deploy Google Chrome and 7-Zip to the client work computers.
<br/>
<br/>
<br/>
<br/>

<p align="center">
Creating the Application: <br/>

<img src="https://i.imgur.com/l6cQuEs.png" height="80%" width="80%" alt="Disk Sanitization Steps2"/>
 
<img src="https://i.imgur.com/tvyWmP4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/zWNGEda.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
<br />
<br />
Populating the properties with the correct date published, language, keywords, and icon:  <br/>
<img src="https://i.imgur.com/skQ8xuQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/OZybQ00.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
Deploying Microsoft Teams: <br/>
<img src="https://i.imgur.com/V8uMPgz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/InDuD4i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/lzAX0MQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/X2bjZvg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/FcxKhAX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/QFJTfVw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/PpVbZpE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/zjHMqCF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
Client view in Software Center (TS01):  <br/>
<img src="https://i.imgur.com/vt7PyJ4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Added the shortcuts to the desktop:  <br/>
<img src="https://i.imgur.com/U7sC3bO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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
