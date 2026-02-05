# Group Policy Configuration

## Objective
Implement basic Group Policy Objects to control user desktop settings and restrict system access.

## GPOs Created
<img width="1024" height="768" alt="wallpaper_GPO" src="https://github.com/user-attachments/assets/4e11b42a-4fcc-49fe-b168-3d090fb5f3c0" />
<img width="1024" height="768" alt="disable_control_panel_GPO" src="https://github.com/user-attachments/assets/84681ecd-a4d6-40db-adea-6498315b1b2b" />

### Corporate Wallpaper Policy
Configured a standard desktop wallpaper for domain users.

### Disable Control Panel Policy
Restricted user access to Control Panel and PC Settings.

## Implementation
- Created GPOs in Group Policy Management.
- Linked policies to the Users Organizational Unit.
- Forced policy update using gpupdate /force.
<img width="1024" height="717" alt="forced_policy_update" src="https://github.com/user-attachments/assets/700102c0-25b9-4802-be8a-a8d6c775c172" />

## Verification
- Confirmed wallpaper applied to domain user login.
- Confirmed Control Panel access was blocked.
<img width="1024" height="768" alt="confirmed_policies_success" src="https://github.com/user-attachments/assets/360ef6bb-6e1d-4eb5-a9aa-eea5c9db45e3" />

## What I Learned
- How Group Policy centralizes management of user settings.
- The difference between User and Computer configuration policies.
- How OU linking controls policy scope.
