<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Description</h2>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />
<h2>Video Demonstration</h2>
<a href="https://youtu.be/gzy48ooUdZc?si=hVSqeiG2InnKcpre">osTicket - Prerequisites and Installation</a>






<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)


<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2> Installation Steps </h2>

<p>
<h2> Step 1 </h2>

  ![Image](https://github.com/user-attachments/assets/c8c1298f-eae5-4317-8e14-9065b52db231)

<p>
To set up osTicket on a Windows 10 Azure Virtual Machine, start by creating a VM with 4 vCPUs named "osticket-vm". Set the username as "labuser" and the password as "osTicketPassword1!". Log into the VM using Remote Desktop. Next, download the "osTicket-Installation-Files.zip" and extract it to the desktop, naming the folder "osTicket-Installation-Files".
Install and enable IIS with CGI support by navigating to the "World Wide Web Services" and selecting "Application Development Features" and enabling CGI.



</p>
<br />

<p>
<h2> Step 2 </h2>

![Image](https://github.com/user-attachments/assets/17fa5c22-7594-42cb-aeaf-9866df4e2b0f)

<p>
From the "osTicket-Installation-Files" folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) and the Rewrite Module (rewrite_amd64_en-US.msi). Create a new directory at "C:\PHP", unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into this directory, and install the Visual C++ Redistributable (VC_redist.x86.exe). Then, install MySQL 5.5.62 (mysql-5.5.62-win32.msi), choose the typical setup, and configure MySQL with the username "root" and the password "root".
Open IIS as an administrator, and register PHP by pointing PHP Manager to "C:\PHP\php-cgi.exe". Reload IIS by stopping and starting the server. 
</p>
<br />

<p>
<h2> Step 3 </h2>

![Image](https://github.com/user-attachments/assets/c79c4d64-596e-4490-b0aa-74c3181e13e0)

<p>
Install osTicket v1.15.8 by extracting "osTicket-v1.15.8.zip" and copying the "upload" folder into "C:\inetpub\wwwroot". Rename the folder to "osTicket". Reload IIS again by stopping and starting the server. To access the site, go to "sites" -> "Default" -> "osTicket" and click "Browse *:80".
Some PHP extensions may not be enabled. To enable them, go back to IIS, navigate to "sites" -> "Default" -> "osTicket", and open PHP Manager. Enable the extensions: php_imap.dll, php_intl.dll, and php_opcache.dll. Refresh the site in the browser to see the changes. Rename the file "ost-sampleconfig.php" to "ost-config.php" in "C:\inetpub\wwwroot\osTicket\include", then assign permissions to "ost-config.php" by disabling inheritance, removing all permissions, and granting "Everyone" full control.
</p>
<br />
<h2> Step 4 </h2>

![Image](https://github.com/user-attachments/assets/22a55a06-1a0b-47f2-beb6-128153f8a818)

Continue the osTicket setup in the browser by entering the helpdesk name and default email. Install HeidiSQL from the "osTicket-Installation-Files" folder, open it, create a new session with the credentials "root/root", and connect to the session. Create a database named "osTicket". Finish the osTicket installation in the browser by entering "osTicket" as the MySQL database, "root" as the username, and "root" as the password, then click "Install Now!".

Final Setup: Once installation is successful, browse to the Help Desk Login Page: http://localhost/osTicket/scp/login.php

End Users osTicket URL: http://localhost/osTicket/

This completes the installation and setup of osTicket on your VM.


<p>

</p>
<br />
