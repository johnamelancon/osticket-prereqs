<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable IIS with necessary features
- Install/Set up PHP manager and MySQL
- Configure IIS and PHP
- Install and configure osTicket
- Finalize setup and cleanup

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/UKYhc6F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 First I created a RG in Azure, next I created a VM using windows 10 OS. I then copied the public IP address and pasted it in my virtualized platform. In addition I Opened the VM and installed IIS with Required Features: Guide the user through the process of installing IIS on Windows and enabling CGI and Common HTTP Features, along with the IIS Management Console.
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set Up PHP and MySQL:Create the directory C:\PHP, download and unzip PHP 7.3.8 into this directory, and install MySQL 5.5.62 with the Standard Configuration and the password set to "Password1".
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure IIS and PHP:** Detail the steps to register PHP within IIS, enabling required PHP extensions like php_imap.dll, php_intl.dll, and php_opcache.dll, and then reloading IIS to apply the changes.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
*Install osTicket:** Guide the user through the process of downloading osTicket, extracting the "upload" folder to c:\inetpub\wwwroot, renaming it to "osTicket", and ensuring proper permissions are set.

</p>
<br />
</p>
<br />

<p>
<img src="https://i.imgur.com/uHb1XMh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set Up MySQL Database with HeidiSQL:** Explain how to download and install HeidiSQL, create a new session with root/Password1, and create a database called "osTicket".

</p>
<br />

<p>
<img src="https://imgur.com/ljDlOLH" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finalize Installation and Cleanup:** Describe the final steps, including completing the osTicket setup in the browser with MySQL Database, MySQL Username, and MySQL Password, browsing to the help desk login page (http://localhost/osTicket/scp/login.php), and performing cleanup tasks such as deleting the setup folder in C:\inetpub\wwwroot\osTicket and setting permissions for ost-config.php.

</p>
<br />
