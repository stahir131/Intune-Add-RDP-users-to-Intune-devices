**Add RDP Users to AzureAD-joined Devices**<br />

This article covers how to add RDP users to AzureAD-joined devices from the Intune admin portal<br />
**Step1**: Login to Intune admin portal at https://intune.microsoft.com/#home<br />
Select > **Endpoint security** > **Account Protection** > **Create policy**<br />
Select the platform and select "**Local user group membership**" and create<br />

![image](https://github.com/user-attachments/assets/4d49ea1b-e969-4524-aa83-275677c66712)

**Note: Add users/User group in the Configuration settings under selection type and not the device to RDP'ed to. The device to be rdp to is added in the Assignement**<br />

![image](https://github.com/user-attachments/assets/2992a835-4db2-4bb5-b7f1-d4374ba9d0d9)

Login to remote device and check the remote dektop users list, you should see all the users.

This settings can also be implemented in the remote device using cmd command as administrator.<br />
**net localgroup "Remote Desktop Users" /add "AzureAD\<userUPN>"**<br />

Replace <userUPN> with the user's email address
