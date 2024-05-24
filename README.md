<h1>SCCM/MECM Application Deployment</h1>

 <img src="https://i.imgur.com/Wl8C0vj.png" alt="Microsoft Endpoint Configuration Manager" class="header-image">

<h2>Description</h2>
Project showcases how System Center Configuration Manager (SCCM), also known as Microsoft Endpoint Configuration Manager (MECM), is utilized to deploy applications to client work computers in a simulated work environment. The applications deployed in this demonstration are Microsoft Teams, Google Chrome, and 7-Zip. The target devices for this deployment are three workstations: WS01, WS02, and TS01, representing typical client devices in a professional setting.
<br />
<br />

<h2>Environment Used</h2>
<p>
The lab environment is comprised of three virtual machines: DC01 (Domain Controller 1), GW01 (Gateway 1), and CM01 (Configuration Manager 1). DC01, equipped with 1 processor (2 cores), 2GB of memory, and 100GB of storage, operates within the LAN segment "CM Lab" and functions as the domain controller. GW01, featuring similar specifications to DC01, serves as the gateway, facilitating Wi-Fi connections to DC01 via Routing and Remote Access. DC01, in turn, employs DHCP to allocate IP addresses, enabling CM01's internet connectivity. CM01, with 1 processor (8 cores), 16GB of memory, and varying storage capacities, operates within the same LAN segment and relies on DC01 for internet access. This setup is designed to demonstrate network infrastructure configurations and management using virtualization technology.
 <br />
</p>

<p> 
   CM01 is the focal point, boasting a robust configuration that includes WSUS (Windows Server Update Services), SQL Server 2022, SQL Server Management Studio, and Configuration Management version 2403. WSUS enables centralized management of Windows updates across the network, ensuring timely deployment and compliance with security patches and feature upgrades. With SQL Server 2022 and SQL Server Management Studio in place, CM01 serves as a powerful database management platform, facilitating data storage, retrieval, and manipulation with advanced SQL functionalities. Additionally, Configuration Management version 2403 enhances the system's capability to streamline configuration tasks, automate software deployment, and enforce compliance standards.
<br />
<br />
</p>


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
