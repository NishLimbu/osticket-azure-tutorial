# osTicket Installation on Azure Virtual Machine

This repository provides a step-by-step tutorial for deploying osTicket, a support ticketing system, on a virtual machine in Microsoft Azure.

## Prerequisites
1. An Azure account (create one at [Azure Portal](https://portal.azure.com)).
2. Basic understanding of Azure and virtual machines.
3. Remote Desktop Protocol (RDP) client installed.

## Steps

### Step 1: Create a Virtual Machine
1. Log in to the [Azure Portal](https://portal.azure.com).
2. Navigate to **Virtual Machines** and click **+ Create**.
3. Fill out the required fields:
   - **Resource Group**: Create or use an existing one.
   - **VM Name**: `osticket-vm`.
   - **Region**: Choose your preferred location.
   - **Image**: Select `Windows Server 2022 Datacenter`.
   - **Size**: Use `Standard_B1ls` or equivalent.
   - **Administrator Account**: Set username and password.
4. Click **Review + Create**, then **Create**.

![Virtual Machine Creation](./images/vm-creation.png)

### Step 2: Connect to the Virtual Machine
1. Once the VM is deployed, go to the **Virtual Machines** section in Azure.
2. Select your VM and click **Connect > RDP**.
3. Download the RDP file and log in using the credentials created earlier.

### Step 3: Install Prerequisites on the VM
1. Open PowerShell as Administrator.
2. Install IIS (Internet Information Services):
   ```powershell
   Install-WindowsFeature -name Web-Server -IncludeManagementTools