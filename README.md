<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>🔧 Major Prerequisites</h2>

1. **Azure Subscription and Resource Group Access**  
   Required to provision and manage the virtual machine infrastructure.

2. **Basic Understanding of Windows Server and IIS**  
   Needed for enabling roles/features like CGI and managing the web server stack.

3. **PHP and MySQL Installation Files and Tools**  
   Must have all installation assets (PHP, MySQL, PHP Manager, URL Rewrite, VC Redistributable, osTicket) on-hand.

4. **Remote Desktop Access and Admin Privileges**  
   Full admin access to the VM is essential for installing software and modifying system settings.

5. **Network Configuration and Port Accessibility**  
   Ensure that HTTP/port 80 is open and accessible for web access to osTicket.


<h2>Installation Steps</h2>

<p>
![image](https://github.com/user-attachments/assets/3b90f622-590b-4e63-a011-606ae348b63b)
</p>
✅ Step 1: Provision and Configure the Virtual Environment

- Deployed a **Windows 10 VM** on **Microsoft Azure** with **4 vCPUs**.
- Connected via **Remote Desktop Protocol (RDP)** to access the virtual machine.
- Prepared the environment for software installation and configuration.


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
✅ Step 2: Install Required Services and Software Stack

- Installed and configured **Internet Information Services (IIS)** with **CGI support**.
- Set up **PHP**, **MySQL 5.5**, and required IIS modules:
  - **PHP Manager**
  - **URL Rewrite Module**
  - **VC Redistributable**
- Deployed **osTicket files** into the web server root directory.
- Registered the PHP executable in IIS using **PHP Manager**.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 ✅ Step 3: Configure osTicket and Finalize Web Interface

- Enabled necessary **PHP extensions** and configured **file/folder permissions**.
- Created the **MySQL database** and completed the osTicket installation via the web browser.
- Finalized help desk settings:
  - Defined support email address
  - Connected osTicket to the configured MySQL database
