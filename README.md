<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=WRr7XhbUlJg)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Server Environment
- Operating Systems
- Web Server
- Remote Access
- Database

<h2>Installation Steps</h2>

<p>
  
![Alt Text](https://github.com/chawk10/osticket-prereqs/blob/main/step%201.png?raw=true)

</p>
<p>
Step 1: Install IIS (Internet Information Services)

Open Control Panel > Programs > Turn Windows features on or off.

Enable Internet Information Services (IIS).

Expand IIS components and ensure CGI and ISAPI Extensions are selected.

Click OK and restart if necessary.
</p>
<br />

<p>
  
![Image alt](https://github.com/chawk10/osticket-prereqs/blob/main/Step%202.png?raw=true)

</p>
<p>


Step 2: Install PHP

Download PHP (recommended version 7.4) from the official PHP website.

Extract PHP files to C:\PHP.

Add C:\PHP to the system environment variable PATH.

Configure php.ini:

Enable required extensions such as mysqli, gd, mbstring.
</p>
<br />

<p>
  
![image alt](https://github.com/chawk10/osticket-prereqs/blob/main/Step%203.png?raw=true)
  
</p>
<p>
Step 3: Install MySQL Database

Download and install MySQL Server or MariaDB.

Create a database named osticket.

Create a database user with full privileges on osticket
</p>
<br />

<p>

![image alt](https://github.com/chawk10/osticket-prereqs/blob/main/Step%204.png?raw=true)

</p>
<p>
Step 4: Download and Extract osTicket

Download osTicket from osTicket’s official website.

Extract the contents to C:\inetpub\wwwroot\osticket.
</p>
<br />

<p>
  
![image alt](https://github.com/chawk10/osticket-prereqs/blob/main/Step%205.png?raw=true)
  
</p>
<p>
Step 5: Configure IIS for osTicket

Open IIS Manager.

Add a new site with the following details:

Site name: osTicket

Physical path: C:\inetpub\wwwroot\osticket



Configure PHP handler mapping in IIS.
</p>
<br />

<p>
  
![image alt](https://github.com/user-attachments/assets/53fc349f-8548-4700-b916-326223acc35f)

<p>


Step 6: Run osTicket Installation Script

Open a web browser and navigate to https://osticket.com/download/

Follow the on-screen installation steps:

Provide database credentials.

Set up the administrator account.

Complete installation.
</p>
<br />

<p>
  
![image alt](https://github.com/chawk10/osticket-prereqs/blob/main/Step%207.png?raw=true)

</p>
<p>
Step 7: Final Configuration

Delete the setup directory from C:\inetpub\wwwroot\osticket.

Set file permissions correctly.

Log in to the osTicket admin panel and configure settings as needed.
</p>
<br />
