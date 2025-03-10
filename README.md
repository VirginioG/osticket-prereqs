<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

 ### [YouTube Demonstration](https://www.youtube.com)
osTicket video


<h2>Description</h2>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />
<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Environments Used </h2>
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

@@ -27,11 +32,24 @@ This tutorial outlines the prerequisites and installation of the open-source hel

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
1. Create an Azure VM
VM Name: osticket-vm
Username: labuser
Password: osTicketPassword1!
Choose Windows 10 with 4 vCPUs.
2. Log into the VM
Use Remote Desktop to log in to the VM.
3. Download and Extract osTicket Installation Files
Download osTicket-Installation-Files.zip and unzip it on the desktop. The folder should be named osTicket-Installation-Files.
4. Install IIS with CGI Support
In Control Panel, enable IIS and the CGI feature under Application Development Features.
5. Install Dependencies
PHP Manager for IIS: Install from the osTicket-Installation-Files folder.
Rewrite Module: Install from the osTicket-Installation-Files folder.
PHP 7.3.8: Create a C:\PHP directory and unzip the PHP files there.
Visual C++ Redistributable: Install VC_redist.x86.exe from the osTicket-Installation-Files folder.
These steps will set up the necessary software on your VM to proceed with osTicket installation.




</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
