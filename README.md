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
<img src="https://i.imgur.com/HPMYaAI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
    1. Setting up VM/Installing IIS with Required Features:
     First create a RG in Azure as the home for VM, next create a VM using windows 10 OS. Then copy the public IP address and paste in your virtualized platform. In addition to that, open the VM and install IIS with Required Features: - Go to your Windows settings and select "Apps" or "Programs."
   - Click on "Turn Windows features on or off."
   - Find "Internet Information Services" and check the box.
   - Expand it and check "CGI" and "Common HTTP Features."
   - Also, check "IIS Management Console."
   - Click "OK" to install these features.
<p>
<img src="https://i.imgur.com/zF9DkWs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
     2. Setting Up PHP and MySQL:
   - Open File Explorer and navigate to the C drive.
   - Create a new folder called "PHP" in the C drive.
   - Download PHP 7.3.8 from the internet and unzip its contents into the "PHP" folder.
   - Now, download and install MySQL 5.5.62 from the internet.
   - During installation, choose the "Standard Configuration" and set the password to something easy to remember 
</p>
<br />

<p>
<img src="https://i.imgur.com/Ojcl2CJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
    3. Configuring IIS and PHP:
   - Open Internet Information Services (IIS) Manager.
   - Find "PHP Manager" and install it.
   - After installation, click on "PHP Manager" and then "Enable or disable an extension."
   - Enable extensions like php_imap.dll, php_intl.dll, and php_opcache.dll.
   - Once done, restart IIS to apply the changes.
<br />

<p>
<img src="https://i.imgur.com/GL8cQvb.png="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
    4. Installing osTicket:
   - Download osTicket from the internet and extract the downloaded file.
   - Move the extracted "upload" folder to C:\inetpub\wwwroot.
   - Rename the "upload" folder to "osTicket."
   - Make sure to set the correct permissions for the "osTicket" folder.
</p>
<br />
</p>
<br />

<p>
<img src="https://i.imgur.com/hu0u4Lc.png"80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
     5. Setting Up MySQL Database with HeidiSQL:
   - Download and install HeidiSQL from the internet.
   - Open HeidiSQL and create a new session.
   - Use "root" as the username and set a password.
   - Create a new database called "osTicket" within HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/aP18sBR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  6. Finalizing Installation and Cleanup: 
  Complete the setup of osTicket in your web browser using the MySQL Database, Username, and Password. 
  Once installation is complete, browse to the help desk login page at http://localhost/osTicket/scp/login.php. Delete the setup folder located in C:\inetpub\wwwroot\osTicket to clean up. Set permissions for ost-config.php file to "Read" only for security purposes.
</p>
<br />
