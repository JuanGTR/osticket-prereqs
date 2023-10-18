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

- Enabling IIS 
- Getting/setting up PHP
- Downloading and setting up MySQL
- Setting up IIS and downloading Osticket
- Setting up osTicket and its database

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/S2vJUWw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First we are going to run the control panel and go to “programs and features” and click "turn windows features on and off" to get ISS features.
</p>
<br />

<p>
<img src="https://i.imgur.com/tU3lee9.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
CGI and Common HTTP Features
Start turning on the following features:
World Wide Web Services -> Application Development Features ->
- CGI
- Common HTTP Features
AND IIS Management Console
Internet Information Services -> Web Management Tools -> IIS Management Console
- IIS Management Console
</p>
<br />

<p>
<img src="https://i.imgur.com/IX9Zw0E.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
  After Enabling ISS you can test it by going to your browser and typing 127.0.0.1. Next download PHP manager for IIS And Download rewrite module.
</p>
<br />

<p>
<img src="https://i.imgur.com/ZNkbvKT.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p> 
 
- Create a folder on (C:) Drive for PHP
- Download and extract PHP onto the PHP folder in C: drive
- Download Microsoft C++ Redistributable

<p>
<img src="https://i.imgur.com/yNSQuLK.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

- Download MySQL and set up
- Typical Setup
- Launch Configuration Wizard (after install), Standard Configuration, Set Password

<p>
<img src="https://i.imgur.com/CSHpu7q.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

<p>Next, go to start and run ISS as an administrator.</p>

<p>
<img src="https://i.imgur.com/QCIJs9g.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

- Register PHP from within IIS
- Reload IIS (Open IIS, Stop and Start the server)

<p>
<img src="https://i.imgur.com/J5Uql9o.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

- Download and Install osTicket
- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
- Reload IIS (Open IIS, Stop and Start the server)
- Go to sites -> Default -> osTicket
- On the right, click “Browse *:80”

You should be taken to osTicket setup page if done successfully.

<p>
<img src="https://i.imgur.com/q0qD1fv.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

Note that some extensions are not enabled

- Go back to IIS, sites -> Default -> osTicket
- Double-click PHP Manager
- Click “Enable or disable an extension”
- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll
  
Refresh the osTicket site in your browse, observe the changes

<p>
<img src="https://i.imgur.com/PkMIPVP.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

<p>Continue setting up on osTicket, it will ask you to fill in some information from previous steps and create some accounts.</p> 

<p>
<img src="https://i.imgur.com/mkzwN2f.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

download and install HeidiSQL.
- Open Heidi SQL
- Create a new session, root/Password1
- Connect to the session
- Create a database called “osTicket”

<p>
<img src="https://i.imgur.com/daMLU2s.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

<p>Once you finish making changing some more settings in Osticket, you will be presented with a screen like the one above if every step was completed properly.</p>


  




























