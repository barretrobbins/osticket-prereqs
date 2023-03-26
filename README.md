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

- Create Resource Group in Azure portal with a Windows 10 Virutal Machine (VM)
- Enable Internet Information Services (IIS) with CGI
- Install PHP, Rewrite Module, PHP 7.3.8, and VC Redistributal
- Install MySQL (Setup User name and Password)
- Install C++ Reader Redisputable
- Configure permissions and Install osTicket

<h2>Installation Steps</h2>

<p>
The first step was to create a new resource group and VM in Azure. I created a resource group named "osTicket"
<img src="https://i.imgur.com/PypD19T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Inside that resource group I created a Windows 10 VM and named it "VM-osTicket".
<img src="https://i.imgur.com/oY6Yx6Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Next, enabled IIS with CGI performing the following steps: open the Control Panel, select run, click Programs, click "turn windows features on or off"; then find "Internet Information Services", select it and expand it, expand "World Wide Web Services", expand "Application Development Features", find CGI and enable it, then click "OK".
<img src="https://i.imgur.com/h2ESx4C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
Install PHP Manager for IIS.
<img src="https://i.imgur.com/2YLUyK1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Next, install Rewrite Module
<img src="https://i.imgur.com/sMQryjQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
  
Then, install PHP 7.3.8
  
<img src="https://i.imgur.com/umYHJxg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
Finally, install VC Redistributal
<img src="https://i.imgur.com/NkKU8fA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
