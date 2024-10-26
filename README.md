**Add RDP Users to AzureAD-joined Devices**<br />

This article covers how to add RDP users to AzureAD-joined devices<br />
**Step1**: Login to Intune admin portal at https://intune.microsoft.com/#home<br />
Select > **Endpoint security** > **Account Protection** > **Create policy**<br />
Select the platform and select "**Local user group membership**" and create<br />

![image](https://github.com/user-attachments/assets/4d49ea1b-e969-4524-aa83-275677c66712)

**Note: Add users/User group in the Configuration settings under selection type and not the device to RDP'ed to. The device to be rdp to is added in the Assignement**<br />

![image](https://github.com/user-attachments/assets/2992a835-4db2-4bb5-b7f1-d4374ba9d0d9)

Login to remote device and check the remote dektop users list, you should see all the users.
