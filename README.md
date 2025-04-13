
<p align="center"> 
  
  ![image](https://github.com/user-attachments/assets/f3acbec5-6ea9-4300-9547-b9b2e692a18c)
</P>

<h2>Azure Virtual Machine and VPN Lab</h2>
This tutorial oversees setting up a virtual machine in Microsoft Azure, testing VPN connections, and the changes in IP addresses<br />

<h2>Create a Virtual Machine in Azure</h2>

<h3>1.) Access Your Public IP Address</h3>

.On your actual computer, browse to [WhatIsMyIPAddress](https://whatismyipaddress.com)<br>
.Take note of your public IP address and save it in a text file for reference.<br>

<h3>2.) Create a Resource Group</h3>

Log into your [Azure Portal](https://azure.microsoft.com/en-us/)<br>
Navigate to **Resource Groups** and click **Create**.<br>
Provide the following:<br>
**Resource Group Name**: VPN-TEST<br>
**Region**: Select a region near you.<br>
Click **Review + Create**, then **Create**.<br>

<h3>3.) Create a Virtual Machine</h3>

Navigate to **Virtual Machines** in the Azure Portal and click **Create**.<br>
.Select **Azure Virtual Machine**.<br>
.Fill out the following:<br>
 -Name: MyWindowsVM
 -Region: Choose a region close to your geographic location or country from your current location.
 -Image: Windows 10 22H2.
 -Size: Select a size that has at least 2vcpus, and 8GiB memory.
 -Administrator Username and Password: Set your credentials.
.Acknowledge the licensing agreement & ensure Inbound Port Rules to allow RDP (Remote Desktop Protocol).
.Click Review + Create, then Create.

![image](https://github.com/user-attachments/assets/d89cd053-c425-4247-aca9-8e2d320068a0)
