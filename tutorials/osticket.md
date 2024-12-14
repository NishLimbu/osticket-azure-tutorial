# osTicket Installation on Azure Virtual Machine

This repository provides a step-by-step tutorial for deploying osTicket, a support ticketing system, on a virtual machine in Microsoft Azure.

### Step 1: Connect to the VM  
Use Remote Desktop to connect to your Azure Virtual Machine.  

---

### Step 2: Enable IIS on Windows  
1. Open the Control Panel and navigate to **Programs > Turn Windows Features On or Off**.  
2. Check **Internet Information Services (IIS)** and click OK.  

---

### Step 3: Install Web Platform Installer and Configure PHP/MySQL  
1. Download and install the [Web Platform Installer](https://www.microsoft.com/web/downloads/platform.aspx).  
2. In the installer, search for:  
   - **MySQL 5.5** > Click "Add".  
   - **PHP (x86)** up to version **7.3** > Add all simple versions.  
3. Click **Install** and follow the prompts. Use:  
   - Username: `root`  
   - Password: `Password1`  
4. Ignore installation errors if any, and finish.  
5. Download and install:  
   - PHP Version 7.3.8  
   - PHP Manager 1.5.0 for IIS  
   - Microsoft Visual C++ 2009 Redistributable Package  

---

### Step 4: Install osTicket  
1. Download osTicket and extract the files.  
2. Move the **Upload** folder to `C:\inetpub\wwwroot` and rename it to `osTicket`.  

---

### Step 5: Restart IIS and Launch osTicket  
1. Open IIS and restart the server.  
2. Navigate to **Sites > Default Website > osTicket** and click **Browse *:80** to open osTicket in your browser.  

---

### Step 6: Enable PHP Extensions  
1. In IIS, go to **Sites > Default Website > osTicket > PHP Manager**.  
2. Enable these extensions:  
   - `php_imap.dll`  
   - `php_intl.dll`  
   - `php_opcache.dll`  

---

### Step 7: Configure osTicket  
1. Rename `ost-SAMPLEconfig.php` to `ost-config.php` in `C:\inetpub\wwwroot\osTicket\include`.  
2. Set file permissions:  
   - Right-click `ost-config.php`, select **Properties > Security > Advanced > Disable Inheritance**.  
   - Remove inherited permissions, add **everyone**, and grant full control.  

---

### Step 8: Continue Setup in Browser  
1. In your browser, set up osTicket:  
   - Name: xxxx  
   - Email: Use your email.  
   - Admin Username: `xxxx`  
   - Password: `xxxx`  

---

### Step 9: Install HeidiSQL and Create Database  
1. Download and install [HeidiSQL](https://www.heidisql.com/).  
2. Open HeidiSQL and connect:  
   - Username: `xxxx`  
   - Password: `xxxx`.  
3. Right-click and create a new database named `osTicket`.  

---

### Step 10: Finalize osTicket Installation  
1. Return to your browser and complete the fields:  
   - Database Name: `osTicket`  
   - Username: `root`  
   - Password: `Password1`  
2. Click **Install Now**.  

---

