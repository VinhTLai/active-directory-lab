# Domain Controller Setup (DC01)

## Objective
Set up a Windows Server virtual machine as a Domain Controller for an Active Directory home lab.

## Steps Performed

### 1. Windows Server Installation
- Installed Windows Server 2022 (Standard, Desktop Experience) using ISO.
- Logged in successfully and confirmed Server Manager loaded.
<img width="1024" height="768" alt="server_install_success" src="https://github.com/user-attachments/assets/6496db21-1357-4b9f-ae21-88b79dfb28f0" />

### 2. Server Configuration
- Renamed the server to DC01.
- Restarted the server to apply name change.
- Configured a static IPv4 address.
- Set the preferred DNS server to the server’s own IP address.
<img width="1024" height="768" alt="local_server_rename" src="https://github.com/user-attachments/assets/7ff9d110-a248-4929-9758-f3bd50bb4d83" />

### 3. Active Directory Domain Services Installation
- Installed the Active Directory Domain Services role via Server Manager.
- Included DNS Server role as required.
<img width="1024" height="768" alt="roles_installed" src="https://github.com/user-attachments/assets/c3ebb9a7-9c15-47cf-9f87-f660360fec37" />

### 4. Domain Controller Promotion
- Promoted the server to a Domain Controller.
- Created a new forest with the domain name `lab.local`.
- Configured Directory Services Restore Mode (DSRM) password.
- Verified successful reboot and domain login.

## Verification
- Successfully logged in using domain credentials.
- Confirmed Active Directory Users and Computers opened without errors.
- Verified DNS Manager functionality.
<img width="1024" height="768" alt="ADUC" src="https://github.com/user-attachments/assets/4eb964dd-c9d4-400a-8c94-e71621546e43" />
<img width="1024" height="768" alt="DNS_Manager" src="https://github.com/user-attachments/assets/3d3e7f78-1d6a-4905-bc23-628f2b586a5b" />

## What I Learned
- The importance of setting a static IP before promoting a Domain Controller.
- How Active Directory relies on DNS for authentication and domain services.
- The correct order of steps required to safely promote a server to a Domain Controller.
