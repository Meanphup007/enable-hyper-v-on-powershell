### 1. Restart computer
### 2. Key boot = ' ESC, F1, F2, F10, F11, F12, DELETE ' key 
### 1-2. Automatically Restart Windows Into BIOS Setup (CMD) 
``` Command
shutdown /r /fw /t 0
```
### 3. Enable virtualization on bios
### 4. Disable fast boot
### 5. Disable security boot   
### 6. Use this command with powershell (Administrator)
    
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
    dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
