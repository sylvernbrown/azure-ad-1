<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)
  
<h2>High-Level Architecture Setup Steps</h2>

- Architecture Explanation
- Set up a Domain Controller in Microsoft Azure
- Set up Client-1 in Microsoft Azure

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
Navigate to <strong>Microsoft Azure</strong> and create a new resource group named <strong>Active-Directory-Lab</strong> or something else memorable.
<img src="https://i.imgur.com/RjSeT4B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Create a Virtual Machine named <strong><i>dc-1</i></strong>.  Be sure to follow the steps below.
<img src="https://i.imgur.com/MqeHx3w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Ensure the <strong>image</strong> selection reads <strong><i>Windows Server 2022: Azure Edition</i></strong>.
<img src="https://i.imgur.com/MqeHx3w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Next, create a new VM named <strong>Client-1</strong>.
<img src="https://i.imgur.com/MEAUWZF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Ensure <strong>Windows 10 Desktop</strong> is running on client-1.
<img src="https://i.imgur.com/wyP4nX7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Navigate to <strong>Home > Virtual-Machines > dc-1 > Virtual NIC </strong>.
<img src="https://i.imgur.com/62diXV5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Navigate to <strong>Home > Virtual-Machines > dc-1 > Virtual NIC </strong>.
<img src="https://i.imgur.com/62diXV5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Select <strong>IP Config</strong>.
<img src="https://i.imgur.com/sgRgtJ2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Select <strong>Static</strong>.
<img src="https://i.imgur.com/FlcFoBj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Navigate to <strong>Home > Virtual Machines > [select dc-1] > Networking Settings > [copy private i.p address] </strong>.
<img src="https://i.imgur.com/Hjs5ujx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
Next, navigate to <strong>Home > Virtual Machines > client 1 | Network Settings > client-1352_z1 </strong>.  Paste the private i.p addres from <strong>dc-1</strong> in the <strong>"DNS Server"</strong> text box.
<img src="https://i.imgur.com/xzpAYZo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />

<p>
  Finally, login to <strong>client-1</strong> using it's public ip address.  Open <strong>powershell</strong> and ping <strong>dc-1</strong> to ensure the process has worked.
<img src="https://i.imgur.com/OkGW9Un.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <br />
  <strong>Note: This is imperative, ensure dc-1 is running the server version of Windows OS.</strong>
</p>
<br />



