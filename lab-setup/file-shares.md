## File Shares and Permissions

## Objective
Configure a shared folder in an Active Directory environment and control access using domain security groups, Share permissions, and NTFS permissions. Validate access from a domain-joined client machine.

## Security Groups
1. Created domain security groups:
   - File_RW (Read/Write access)
   - File_RO (Read Only access)
<img width="1024" height="768" alt="file_permissions" src="https://github.com/user-attachments/assets/940744fd-f138-48bd-b54d-3d4754a4f625" />

## Users Added
2. Added domain test users to the appropriate security groups.
<img width="1024" height="768" alt="added_jdoe_to_group" src="https://github.com/user-attachments/assets/bb057387-c3ea-49a6-ba22-ea23b0ff426e" />

## Shared Folder Creation
3. Created shared folder on server:
   - Path: C:\Shares\CompanyData

## Shared Permissions
4. Configured Share Permissions:
   - Removed Everyone
   - File_RW → Change + Read
   - File_RO → Read
<img width="1024" height="768" alt="file_permissions" src="https://github.com/user-attachments/assets/6510fc27-f09c-4270-9ca4-493c4d044f6f" />

## NTFS Permissions
5. Configured NTFS Permissions:
   - File_RW → Modify
   - File_RO → Read & Execute
<img width="1024" height="768" alt="ntfs_permissions" src="https://github.com/user-attachments/assets/42450977-365c-48ee-95a7-d414aa163f99" />

# Test Shared Access Behavior
6. Tested access from domain-joined Windows 11 client:
   - Accessed share using \\DC01\CompanyData
   - Verified Read/Write and Read Only access behavior.
<img width="1024" height="768" alt="rw_user_edit_text" src="https://github.com/user-attachments/assets/e633c431-d48d-41e7-b7d6-a92a8353b36d" />
<img width="1024" height="768" alt="ro_user_denied_file_creation" src="https://github.com/user-attachments/assets/6b7c6342-796a-456f-9bde-0c556f3bf36f" />

## 🧠 What I Learned
- How to implement role-based access control using Active Directory security groups
- The difference between Share permissions and NTFS permissions
- How effective permissions are determined between Share and NTFS
- How enterprise environments securely manage shared file access
- How to validate file access from a domain-joined client system
