# Windows 11 Domain Join

## Objective
Join a Windows 11 client machine to the Active Directory domain and verify domain authentication.

## Configuration Steps
- Configured Windows 11 DNS settings to point to the Domain Controller.
- Verified connectivity using ping and nslookup.
<img width="1024" height="768" alt="ping_and_nslookup" src="https://github.com/user-attachments/assets/94361714-cacf-469b-81ec-0b0740a60d77" />

- Joined the Windows 11 VM to the lab.local domain.
- Restarted the system to complete the domain join.
<img width="1024" height="768" alt="joining_domain" src="https://github.com/user-attachments/assets/4f86be78-5c5a-4b3f-ad86-0ccf283e7ca1" />

## Verification
- Successfully logged in using a domain user account.
<img width="1024" height="768" alt="user_logged_in" src="https://github.com/user-attachments/assets/8bb7ab0a-eb25-4f87-88c3-34d272713529" />

- Confirmed client computer object appeared in Active Directory.
- Moved the client computer into the Workstations OU.
<img width="1024" height="768" alt="client_in_AD" src="https://github.com/user-attachments/assets/d616cb41-5c35-4cde-8979-be2e1d02e1cf" />

## What I Learned
- Active Directory domain joins rely heavily on DNS configuration.
- Proper network configuration is critical for authentication.
- How client machines integrate into an AD environment.
