<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install Web Platform Installer
- Enable Internet Information Services (IIS)
- Setup Username and Password
- Install C++
- Configure Permissions and install OsTicket

<h2>Installation Steps</h2>

<p>
![Osticket](https://github.com/user-attachments/assets/f81ad1d3-bb23-4634-8df0-007895175629)



</p>
<p>
You will need to log into the osTicket VM in azure and download the installation files and unzip them. After this you need to enable ISS and then make a PHP manager for ISS. Then from the folder open the rewrite module and create a directory C:/PHP. In the files unzip PHP 7.3.8 into the C:/PHP folder. From the installation folder install VC_redist.X86.exe and MySQL 5.5.62 once this is open to a typical setup and launch the wizard configuration and then make the username:root and password:root 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an admin, in IIS register PHP, then reload. from the osTicket folder unzip the osTicket-v1.15.8zip and then copy the upload folder into c:\inetpub\wwwroot and then within that file rename the upload folder to osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
go back to IIS and then reload go to sites-default-osTicket then click browse :80. Then go to PHP manager and enable extensions php_imap.dll,php_intl.dll and php_opcache.dll then click refresh. Rename ost-config-php in there assign permissions to everyone and disable inheritance continue setting up osTicket in the browser and install HeidiSQL. open Heidi create a session and create a database called osTicket. In Heidi the database should be osTicket, the username and password: root. Then click install then it should be installed!
<br />
