
<p align="center"> 
  
  ![image](https://github.com/user-attachments/assets/f3acbec5-6ea9-4300-9547-b9b2e692a18c)
</P>

<h2>Azure Virtual Machine and VPN Lab</h2>
This tutorial oversees setting up a virtual machine in Microsoft Azure, testing VPN connections, and the changes in IP addresses<br />

<h2>Create a Virtual Machine in Azure</h2>

<h3>1.) Access Your Public IP Address</h3>

.On your actual computer, browse to [WhatIsMyIPAddress](https://whatismyipaddress.com)<br>
.Take note of your public IP address and save it in a text file for reference.<br>

![image](https://github.com/user-attachments/assets/7f7726f7-a8bf-4e70-89f7-55148a9e48b1)

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
 -**Name**: vpn-test-win-10<br>
 -**Region**: Choose a region close to your geographic location or country from your current location.<br>
 -**Image**: Windows 10 22H2.<br>
 -**Size**: Select a size that has at least 2vcpus, and 8GiB memory.<br>
 -**Administrator Username and Password**: Set your credentials.<br>
.Acknowledge the licensing agreement & ensure Inbound Port Rules to allow RDP (Remote Desktop Protocol).<br>
.Click **Review + Create**, then **Create**.<br>

![image](https://github.com/user-attachments/assets/d89cd053-c425-4247-aca9-8e2d320068a0)

<h3>4.) Log into the Virtual Machine</h3>

.After the VM is created, navigate to it in the Azure Portal.<br>
.Copy the Public IP Address of your VM.<br>
.Use Remote Desktop to connect to the VM:<br>
  -**Remote Desktop Address**: Enter the Public IP Address of the VM.<br>
  -**Username and Password**: Use the credentials you created earlier.<br>
.Once connected, open a web browser on the VM.<br>

![image](https://github.com/user-attachments/assets/7d48d1f8-5a20-4457-b39a-af7851a27033)

<h3>5.) Check the VM's Public IP Address</h3>

.In the VM, browse to [WhatIsMyIPAddress](https://whatismyipaddress.com)<br>
.Take note of the VM's public IP address and save it in a text file.<br>

![image](https://github.com/user-attachments/assets/246c650c-aa84-4311-869c-91df360def01)



<h2>Sign Up for ProtonVPN and Test the Connection</h2>

<h3>1.) Sign Up for ProtonVPN</h3>

.On your actual computer, go to [ProtonVPN Sign-Up](https://account.protonvpn.com/signup?plan=free&language=en).<br> 
.Create a free account.<br>

<h3>2.) Download ProtonVPN Client</h3>

.In your VM, go to [ProtonVPN Download](https://protonvpn.com/download).<br>
.Download and install the ProtonVPN client.<br>

![image](https://github.com/user-attachments/assets/8599013c-d594-4c1d-8b3e-a39c2ef61077)
![image](https://github.com/user-attachments/assets/b1d642c5-d559-4dad-ba4e-786813892eb8)


<h3>3.) Log into ProtonVPN</h3>

.Open the ProtonVPN client in the VM.<br>
.Login using your ProtonVPN account credentials: [ProtonVPN Login](https://account.protonvpn.com/login)<br>

<h3>4.) Connect to a VPN Server</h3>

.In the ProtonVPN client, choose a VPN server in an area different from your actual computer's location (Proton VPN requires payment to change countries).<br>
.Connect to the VPN server.<br>

![image](https://github.com/user-attachments/assets/06de1327-d3c0-4911-b0dc-6ca19cedc133)

<h3>5.) Check the VPN's Public IP Address</h3>

.In the VM, browse to [WhatIsMyIPAddress](https://whatismyipaddress.com).<br>
.Take note of the new IP address and save it in a text file.<br>

![image](https://github.com/user-attachments/assets/2f1948ec-9656-41bd-b906-6572ef6306be)


<h2>Notes and Observations</h2>

.Save all IP addresses and observations in a text file for documentation purposes.<br>
.Compare the behavior of websites and the changes in IP addresses to understand the effects of geographic location and VPN usage.<br>
