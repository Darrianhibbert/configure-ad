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

<h2>High-Level Deployment and Configuration Steps</h2>

- Domain Admin user created within the domain
- Setup Remote Desktop for non-administrative users on Client-1 virtual machine
- Created additional users and attempt to log into client-1 virtual machine



<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/HXz0uqO.png"/>
</p>
<p>Created a Domain Admin user within the domain and structured Active Directory Users and Computers by adding an _EMPLOYEES Organizational Unit and a _ADMINS Organizational Unit. Additionally, added a new employee called Jane Doe, as the Domain Users Admin to manage user accounts and permissions.
</p>
<br />

<p>
<img src="https://i.imgur.com/NOEnc6u.png"/>
</p>
<p>Configured Remote Desktop access for non-administrative users on Client-1, ensuring proper permissions and security settings are applied to allow seamless remote connectivity.
</p>
<br />

<p>
<img src="https://i.imgur.com/Qwf1dly.png"/>
<img src="https://i.imgur.com/mQwBaNR.png"/>
</p>
<p>Created multiple user accounts and verified them in ADUC under the _EMPLOYEES OU. Logged into DC-1 as jane_admin, ran a PowerShell script to automate account creation, and successfully logged into Client-1 virtual machine with one of the new accounts.
</p>
<br />
