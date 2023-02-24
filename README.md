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

- PHP Manager for IIS 
- Rewrite Module
- PHP 7.3.8
- VC_redist.x86.exe
- MySQL 5.5.62

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/Lw8Wm3K.png"/>
</p>
<p>
Create Virtual Machine in Azure
</p>
<br />

<p>
<img src="https://i.imgur.com/WuigqHb.png"/>
</p>
<p>
Enable IIS in Windows WITH CGI.

</p>
<br />

<p>
<img src="https://i.imgur.com/VJGAKyl.png"/>
</p>
<p>
Open IIS as an Admin.

</p>
<br />

<p>
<img src="https://i.imgur.com/6iEWI8E.png"/>
</p>
<p>
Register PHP from within IIS.

</p>
<br />


<p>
<img src="https://i.imgur.com/J61cGoX.png"/>
</p>
<p>
Download osTicket, extract and copy “upload” folder to c:\inetpub\wwwroot. Within c:\inetpub\wwwroot, Rename “upload” to “osTicket.

</p>
<br />


<p>
<img src="https://i.imgur.com/2Dq9Mgr.png"/>
</p>
<p>
Go back to IIS, sites -> Default -> osTicket. Double-click PHP Manager, click “enable or disable an extension”, and enable: php_imap.dll, php_intl.dll, and php_opcache.dll.

</p>
<br />

<p>
<img src="https://i.imgur.com/16DwOaB.png"/>
</p>
<p>
Rename C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to C:\inetpub\wwwroot\osTicket\include\ost-config.php

</p>
<br />

<p>
<img src="https://i.imgur.com/9FH6xA5.png"/>
</p>
<p>
Assign Permissions: ost-config.php
</p>
<br />


<p>
<img src="https://i.imgur.com/tSHVnI1.png"/>
</p>
<p>
Open Heidi SQL: create a new session, connect to the session, and create a database called “osTicket”

</p>
<br />

<p>
<img src="https://i.imgur.com/wSknfdZ.png"/>
</p>
<p>
Set up osticket in the IIS browser

</p>
<br />


<p>
<img src="https://i.imgur.com/MBynvti.png"/>
</p>
<p>
Delete: C:\inetpub\wwwroot\osTicket\setup

</p>
<br />


<p>
<img src="https://i.imgur.com/jDyYZbL.png"/>
</p>
<p>
Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php

</p>
<br />



