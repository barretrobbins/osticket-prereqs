# osticket-prereqs<p align="center">
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

1 - Create Resource Group in Azure portal with a Windows 10 Virutal Machine (VM)

2 - Enable Internet Information Services (IIS) with CGI

3 - Install PHP, Rewrite Module, PHP 7.3.8, and VC Redistributal

4 - Install MySQL (Setup User name and Password)

6 - Configure permissions and Install osTicket

<h2>Installation Steps</h2>

1 - Create Resource Group in Azure portal with a Windows 10 Virutal Machine (VM)
<p>
<img src="https://i.imgur.com/YWUi4XM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
The first step was to create a new resource group and VM in Azure. I created a resource group named "osTicket".

<img src="https://i.imgur.com/oY6Yx6Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
Inside that resource group I created a Windows 10 VM and named it "VM-osTicket".
</p>
<br />

2 - Enable Internet Information Services (IIS) with CGI
<p>
<img src="https://i.imgur.com/h2ESx4C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
Next, enabled IIS with CGI performing the following steps: open the Control Panel, select run, click Programs, click "turn windows features on or off"; then find "Internet Information Services", select it and expand it, expand "World Wide Web Services", expand "Application Development Features", find CGI and enable it, then click "OK".
</p>
<br />

3 - Install PHP, Rewrite Module, PHP 7.3.8, and VC Redistributal
<img src="https://i.imgur.com/5m28HN6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

First, install PHP Manager

<img src="https://i.imgur.com/yklMBP4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

Next, install Rewrite Module  
 
 
<img src="https://i.imgur.com/umYHJxg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Then, install PHP 7.3.8 

<img src="https://i.imgur.com/NkKU8fA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Finally, install C++ Reader Redisputable
</p>
<br />

4 - Install MySQL (Setup User name and Password)
<p>
<img src="https://i.imgur.com/Y3HJ5AM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/XxOjNbC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Next, install MySQL.  Once downloaded, click next, select standard configuration, click next, create a password then click next, and finally click execute. A database is now installed on the VM, which is used for osTicket.
</p>
<br />

5 - Install osTicket
<p>
<img src="https://i.imgur.com/5W0uyAV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install osticket v1.15.8
</p>
<br />

<p>
<img src="https://i.imgur.com/Apj16hR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy upload folder and paste it in the Windows C: drive.  Go to inetpub -> wwwroot, and then restart Internet Information Services Manager. IIS Manager can be found in the start menu.
</p>
<br />

<p>
<img src="https://i.imgur.com/OCkMydh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Windows C: drive -> inetpub -> wwwroot -> osTicket -> include, and then rename "ost-sampleconfig.php" to "ost-config.php".
</p>
<br />

<p>
<img src="https://i.imgur.com/NXjOkjz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Then, open osTicket in your web browser and begin the basic installation process.
</p>
<br />

<p>
<img src="https://i.imgur.com/fpOivnO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, download and Install HeidiSQL.  Make sure the Launch HeidiSQL is checkmarked and click Finish.  Create a new database for connection and fill in the username and password; User: root and Password: Password1.
</p>
<br />

<p>
<img src="https://i.imgur.com/1M3rVcT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finish the installation process.
</p>
<br />

<p>
<img src="https://i.imgur.com/Z4rIlOb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, delete: C:\inetpub\wwwroot\osTicket\setup
Set Permissions to “Read” only, C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/5trEXyf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login to the osTicket Admin Panel
</p>
<br />
