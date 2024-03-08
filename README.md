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
 First create a RG in Azure as the home for VM, next create a VM using windows 10 OS. Then copy the public IP address and paste in your virtualized platform. In addition to that, open the VM and install IIS with Required Features: - Go to your Windows settings and select "Apps" or "Programs."
   - Click on "Turn Windows features on or off."
   - Find "Internet Information Services" and check the box.
   - Expand it and check "CGI" and "Common HTTP Features."
   - Also, check "IIS Management Console."
   - Click "OK" to install these features.
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   - Open File Explorer and navigate to the C drive.
   - Create a new folder called "PHP" in the C drive.
   - Download PHP 7.3.8 from the internet and unzip its contents into the "PHP" folder.
   - Now, download and install MySQL 5.5.62 from the internet.
   - During installation, choose the "Standard Configuration" and set the password to "Password1."
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
