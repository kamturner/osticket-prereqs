# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Create an Azure Virtual Machine Windows 10, 4 vCPUs. After that, log into the Virtual Machine with remote desktop
- Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop. 
- Install / Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI and then install PHP manager for IIS From the “osTicket-Installation-Files” folder. From the same folder you will then install the rewrite module,  Create the directory C:\PHP, unzip PHP 7.3.8 into the “C:\PHP” folder, nstall VC_redist.x86.exe., install MySQL 5.5.62
- Open IIS as an Admin, Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe), Reload IIS (Open IIS, Stop and Start the server)
- Install osTicket v1.15.8
From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”, Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”
- Install osTicket v1.15.8
From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”
-Assign Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
