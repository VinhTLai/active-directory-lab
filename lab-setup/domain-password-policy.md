# Domain Password and Lockout Policy

## Objective
Implement domain-wide password security and account lockout protections.

## Password Policy Configuration
- Minimum length: 8 characters
- Complexity: Enabled
- History: 5 passwords remembered
- Max age: 60 days
<img width="1024" height="768" alt="configured_password_policy" src="https://github.com/user-attachments/assets/4cab5e63-e0ef-41fa-9d25-f5cdff41f5b9" />

## Account Lockout Policy
- Lockout threshold: 5 failed attempts
- Lockout duration: 15 minutes
- Reset counter: 15 minutes
<img width="1024" height="768" alt="configured_account_lockout_policy" src="https://github.com/user-attachments/assets/00d00923-f8a6-4daa-9e5a-b018332fb9ac" />

## Testing
- Simulated failed login attempts.
- Confirmed account lockout occurred.
- Unlocked user via Active Directory Users and Computers.
<img width="1024" height="768" alt="account_locked_out" src="https://github.com/user-attachments/assets/73336685-b7e0-4ad2-94f3-0e23ad744c21" />
<img width="1024" height="768" alt="unlock_account" src="https://github.com/user-attachments/assets/cae14bff-c2b8-4096-ad2c-4ce03940bef7" />

## What I Learned
- How domain password policies are applied globally.
- How account lockouts protect against brute force attacks.
- How helpdesk unlocks user accounts.
