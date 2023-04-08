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

- Step 1 - Create Resource Group in Azure portal with a Windows 10 Virutal Machine (VM)

- Step 2 - Enable Internet Information Services (IIS) with CGI

- Step 3 - Install PHP, Rewrite Module, PHP 7.3.8, and VC Redistributal

- Step 4 - Install MySQL (Setup User name and Password)

- Step 5 - Configure permissions and Install osTicket

- Step 7- Install HeidiSQL

- Step 8- Finish osTicket Install

<h2>Installation Steps</h2>

1 - Create Resource Group in Azure portal with a Windows 10 Virutal Machine (VM)
<p>
<img src="https://i.imgur.com/YWUi4XM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
First, create a new resource group and VM in Azure. I created a resource group named "osTicket".  Go to the home page in portal.azure.come, click on Resource Group, and click on create.  Name the Resource Group: osTicket, select the region near your location.  For example: Region: (US) West US 3, then click Review + create, and click create. 

<img src="https://i.imgur.com/oY6Yx6Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
Inside that resource group I created a Windows 10 VM and named it "VM-osTicket".  Go to the home page in portal.azure.com, click on Virtual Machines, click create, and click Azure virtual machine.  Select the recently created "osTicket" for the Resource Group.  Name the virtual machine and select the region.  For example: virtual machine name: VM-osTicket and Region: (US) West US 3.  Now, select the image, for example: Windows 10 Pro, version 21H2 - x64 Gen2. Next, select the size, for example: Standard_E2s_v3 2vcpus, 16 Gib memory.  Then enter a username and password.  Afterwards, check the box at the bottom, click Disks, click Networking, click Review + create, and then click create.
</p>
<br />

2 - Enable Internet Information Services (IIS) with CGI
<p>
<img src="https://i.imgur.com/h2ESx4C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
Next, login to Remote Desktop and enable IIS with CGI performing the following steps.  First, open the Control Panel, select run, click Programs, click "turn windows features on or off"; then find "Internet Information Services", select it and expand it, expand "World Wide Web Services", expand "Application Development Features", find CGI and enable it, then click "OK".
</p>
<br />

3 - Install PHP, Rewrite Module, PHP 7.3.8, and VC Redistributal
<img src="https://i.imgur.com/5m28HN6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

First, download the PHP Manager, go to File Folder, and click on Downloads under Quick access; this is where the PHP Manager file will appear.  Then double click the file to open it and begin installation.  Once open, click next, select agree and click next, click next again, and then click close.

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

5 - 5 - Configure permissions and Install osTicket
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
Then, open osTicket in your web browser and begin the basic installation process.  Fill out the informaiton on the page.

System Settings: Helpdesk Name: First Name (Yours) followed by Help Desk, enter a default email; Admin User: enter first and last name, email address, enter any name for the username and then enter your password.  Before finishing the installation process for osTicket, the last step is to setup the database in HeidiSQL.
</p>
<br />

7- Install HeidiSQL
<p>
<img src="https://i.imgur.com/fpOivnO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, download and Install HeidiSQL.  Make sure the Launch HeidiSQL is check marked and click Finish.  Create a new database for connection and fill in the username and password; User: root and Password: Password1.
</p>
<br />

<img src="https://i.imgur.com/AiBuuKV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To create a database, you will need the username and password that was used to install MySQL.  Create a new database by right-clicking on SSS-->New-->Database-->> name your database osTicket and click Ok.

8- Finish osTicket Install
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
