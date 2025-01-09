<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket and the files needed to install osTicket can be found here: https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- osTicket virtual machine
- osTicket-installation-files-zip


<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/XzQCznY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/pyLXdqu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
    <p>
<img src="https://i.imgur.com/WkWmaQP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The first step is to set up your virtual machine in Azure. Create a new virtual machine and make sure to click "create new" for the resource group and you can name it "osTicket". Afterwards you should name your virtual machine "osticket-vm" and set the region to whatever region works for you, just make sure that your resource group is set to the same region. For the purpose of this lab, we will be setting the region to Canada Central. Once that is done, you need to set the virtual machine's image to "Windows 10 Pro, version 22H2-x64 Gen2" and set the size to 2 vcpus and 8 Gib memory. Finally for the username, set it as "labuser" and the password will be set as "osTicketPassword1!". After that, you're done and you can create the virtual machine and log in using remote desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/nYS6lVf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/ajYO2Am.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/5a2PCQ9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/prmHKqm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you are logged into your virtual machine, go ahead and download and unzip the osTicket file from above. After that you have to enable IIS and CGI, you can do this by opening the control panel and then click on "programs" turn "windows features on or off". From there you'll see Internet Information Services and you'll want to check this one. For CGI, you'll have to expand Internet Information Services and then expand World Wide Web Services and then expand Application Development Features and from there you'll see CGI and be able to check it. From the osTicket folder download PHP Manager and the Rewrite Module. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
