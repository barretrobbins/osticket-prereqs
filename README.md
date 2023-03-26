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
- Install MySQL (Setup User name and Password)
- Install C++ Reader Redisputable
- Configure permissions and Install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/PypD19T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oY6Yx6Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The first step was to create a new resource group and VM in Azure. I created a resource group named "osTicket" and inside that group I created a Windows 10 VM and named it "VM-osTicket".
</p>
<br />

<p>
<img src="https://i.imgur.com/h2ESx4C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, I opened VM-osTicket and enabled IIS with CGI using the following steps: open the Control Panel -> click Programs -> click "turn windows features on or off", next find "Internet Information Services", enable it and expand it, -> expand "World Wide Web Services" -> expand "Application Development Features", find CGI and enable it, then click o
</p>
<br />

<p>
<img src="https://i.imgur.com/2YLUyK1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, install PHP Manager for IIS.
</p>
<br />
