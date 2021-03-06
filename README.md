# Create Encrypted VM's on Azure

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FazureDeployPrereqs.json" target="_blank">
Run this pre-requisite template if you are setting up storage account, vnet and subnet for the first time!
<img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<br />

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FazureDeployEncryptedWindowsVM.json" target="_blank">
Scenario 1: This template creates and deploys an Encrypted Windows or Linux VM on Azure! 
<br>
Bitlocker key is encrypted with Kek.
<br>
<img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<br />

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FazureDeployEncryptedWindowsVMNoKek.json" target="_blank">
Scenario 2: This template creates and deploys an Encrypted Windows or Linux VM on Azure! 
<br>
Bitlocker key in clear (no Kek).
<br>
<img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningLinuxVM-AADClientSecret.json" target="_blank">
Scenario 3: This template enables encryption on a running Linux vm using AAD client secret
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningLinuxVM-AADClientSecret-WithKek.json" target="_blank">
Scenario 4: This template enables encryption on a running Linux vm using AAD client secret and KeyEncryptionKey
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>
<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningLinuxVM-Format-AADClientSecret.json" target="_blank">
Scenario 5: This template enables encryption on a running Linux vm using AAD client secret, this will format the disk directly instead of encrypting the existed data. Parameter of the diskFormatQuery should be like this: [{"scsi":"6:0:0:1","name":"azuredisk"},{"scsi":"6:0:0:1","name":"azuredisk2"}] or [{"dev_path":"/dev/sdx","name":"azuredisk"}], the scsi means the disk scsi number, the name means the mount point name.And you can specify the file system used for the device like this: [{"dev_path":"/dev/sdx","name":"azuredisk","file_system":"ext4"}]
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningLinuxVM-Format-AADClientSecret-WithKek.json" target="_blank">
Scenario 6: This template enables encryption on a running Linux vm using AAD client secret and KeyEncryptionKey, this will format the disk directly instead of encrypting the existed data. Parameter of the diskFormatQuery should be like this: [{"scsi":"6:0:0:1","name":"azuredisk"},{"scsi":"6:0:0:1","name":"azuredisk2"}] or [{"dev_path":"/dev/sdx","name":"azuredisk"}], the scsi means the disk scsi number, the name means the mount point name. And you can specify the file system used for the device like this: [{"dev_path":"/dev/sdx","name":"azuredisk","file_system":"ext4"}]
<br>
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>
<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningWindowsVM-AADClientSecret.json" target="_blank">
Scenario 7: This template enables encryption on a running windows vm using AAD client secret
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningWindowsVM-AADClientSecret-WithKek.json" target="_blank">
Scenario 8: This template enables encryption on a running windows vm using AAD client secret and KeyEncryptionKey
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>
<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningWindowsVM-AADClientCert.json" target="_blank">
Scenario 9: This template enables encryption on a running windows vm using AAD client cert thumbprint
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FEnableEncryptionOnRunningWindowsVM-AADClientCert-WithKek.json" target="_blank">
Scenario 10: This template enables encryption on a running windows vm using AAD client cert thumbprint and KeyEncryptionKey
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FCreateNewEncryptedWindowsVM-AADClientSecret.json" target="_blank">
Scenario 11: This template creates a new encrypted windows vm using the server 2k12 gallery image! Using AAD client secret
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

<br>
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Faravindthoram%2FDiskEncryption%2Fmaster%2FCreateNewEncryptedWindowsVM-AADClientSecret-WithKek.json" target="_blank">
Scenario 12: This template creates a new encrypted windows vm using the server 2k12 gallery image! Using AAD client secret and KeyEncryptionKey
<br>
    <img src="http://azuredeploy.net/deploybutton.png"/>
<br>
</a>

Microsoft Online Services Privacy statement - http://www.microsoft.com/privacystatement/en-us/OnlineServices/Default.aspx
