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
The first step is to set up your virtual machine in Azure. Create a new virtual machine and make sure to click "create new" for the resource group and you can name it "osTicket". Afterwards you should name your virtual machine "osticket-vm" and set the region to whatever region works for you, just make sure that your resource group is set to the same region. For the purpose of this lab, we will be setting the region to Canada Central. Once that is done, you need to set the virtual machine's image to "Windows 10 Pro, version 22H2-x64 Gen2" and set the size to 2 vcpus and 8 Gib memory. Finally for the username, set it as "labuser" and the password will be set as "osTicketPassword1!". After that, you're done and you can create the virtual machine and log in using remote desktop.
</p>
<br /><p>
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
Once you are logged into your virtual machine, go ahead and download and unzip the osTicket file from above. After that you have to enable IIS and CGI, you can do this by opening the control panel and then click on "programs" turn "windows features on or off". From there you'll see Internet Information Services and you'll want to check this one. For CGI, you'll have to expand Internet Information Services and then expand World Wide Web Services and then expand Application Development Features and from there you'll see CGI and be able to check it. From the osTicket folder download PHP Manager and the Rewrite Module. 
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
The next step is to go into your files and clicking into your C:// drive and creating a PHP folder inside your C:// drive and extract the PHP folder you downloaded eariler into the C:// PHP folder. From the osTicket folder, download the VC_redist and install and open the MySQL file. Once it's opened click on "typical setup", "Launch configuration Wizard", "Standard Configuration" and set the username and password to "root" for both of them. The next step is to open IIS as an admin and Registering PHP within IIS by clicking on "PHP manager" and clicking on "register a new PHP version" and then browsing to select the PHP file you extracted into your C:// drive. After that reload IIS by starting and stopping IIS.
</p> 
<br />
<p>
<img src="https://i.imgur.com/1z5sR7V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/eLnurqg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/OndmR5o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/ub5ulk7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/8jvnveH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/57gwrZn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/DvmF7zU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/tTNLGZB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you're done reloading IIS, you should unzip the osTicket.zip file and take the "upload" file within it and copy the file and go into your C:// drive, open inetpub, then open wwwroot and then paste the file inside here and rename it to "osTicket". Once you're done with that, go ahead and open IIS and reload once again. Within IIS, you should also click on "sites", then "default web site", and then "osTicket" and then on the right click on "Browse 0.80" and this should open up osTicket.
</p> 
<br />
<p>
<img src="https://i.imgur.com/KjRkaQ7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/9Sr2lSG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/iYPUvJN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/3Yj1JNV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/dwjInnE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/cyF2RCx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <p>
<img src="https://i.imgur.com/tL4etE1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
Some extensions will not be enabled, but we will need these to be enabled. Open up IIS and osTicket once again and double click on PHP manager and click “Enable or disable an extension” and from there enable "php_imap.dll", "php_intl.dll", "php_opcache.dll". Refresh your osTicket browser and observe the extensions that are now enabled. After that is done, we need to open up your C:// drive and click on "inetpub", "wwwroot", "osTicket" and then "include". Within the include folder should be a file named "ost-sampleconfig.php" and you should rename this file to "ost-config.php". Once that is done, right click on "ost-config.php" and click on "properties" and then click on "advanced". After that remove all inherited permissions and then click on "add". Then click on "select a principle" and set it as "everybody". Once that is done click "full control" for the permissions and click on "ok". Once that is done continue setting up your osTicket browser up until "database settings".
<img src="https://i.imgur.com/EvXjZqp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/J11pOES.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/R9R4OrS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/AL2a3y4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/8famZKp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/A4EvNSv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/rTbyrv6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/xAIlb4x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/UJbbwkN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/kE0Tq3H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/PTucIZO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/ylrOV5l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/AD65H7z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/U7rZp80.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/2bTyAvI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  Finally you should install Heidi SQL and open it once downloaded. Once opened, click "add" and type in "root" for both the username and password and click on "open". After that click on "create new" and then "database" and name this database "osTicket". Once the database is created, go back to the osTicket browser and continue filling out the "database settings" section. The MySQL database should be "osTicket" and the username and password should be "root". After that click "install now", and after that, your osTicket system should be installed fully and should be running smoothly!
  <img src="https://i.imgur.com/seDmBup.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/uULer8E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/REb6X5v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/rYsUNdQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/bmCaSL6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/3sx4B2w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/fZM6p8s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
  <img src="https://i.imgur.com/Gx4LC7u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
