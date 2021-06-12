[![Open Source Love svg3](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
![Hits](https://hitcounter.pythonanywhere.com/count/tag.svg?url=https://github.com/StarTrooper08/DockerInstallation) ![Maintaner](https://img.shields.io/badge/maintainer-StarTrooper08-blue) [![GitHub forks](https://img.shields.io/github/forks/StarTrooper08/DockerInstallation.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/StarTrooper08/DockerInstallation/network/)  



# Docker Installation
Quick Start Guide for Docker Installation process on Windows 10


### **Software Requirements :**
Download the required softwares -

1. [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) - Here you can download Docker Desktop for Windows. <br/> 
2. [WSL update package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) (WSL2 Linux kernel update package for x64 machines) - Here you can download wsl_update package.  <br/>
3. Linux Distro for Windows(Install it from Microsoft Store) - For this follow along the steps dont install it before.

**`Please dont install any of this software before it may give you an error. Follow the below steps for installation carefully`**

### **System Requirements :**

#### For Docker Desktop -
Windows 10 64-bit: Home, Pro, Enterprise, or Education, version 1903 (Build 18362 or higher).
Enable the WSL 2 feature on Windows. For detailed instructions, refer to the Microsoft documentation.

`The following hardware prerequisites are required to successfully run WSL 2 on Windows 10:`

* 64-bit processor with Second Level Address Translation (SLAT)
* 4GB system RAM
* BIOS-level hardware virtualization support must be enabled in the BIOS settings.
* Download and install the Linux kernel update package.


#### For WSL2 -
To update to WSL 2, you must be running Windows 10.
* For x64 systems: Version 1903 or higher, with Build 18362 or higher.
* For ARM64 systems: Version 2004 or higher, with Build 19041 or higher.
* Builds lower than 18362 do not support WSL 2. Use the Windows Update Assistant to update your version of Windows.


##### Easy Steps to Install Docker Desktop on Windows :

**`Step 1:`**

First open command prompt of windows on administrator mode.
Then paste this command (Enable WSL)-

```dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart```

You will get WSL Enabled Successfully msg will be displayed on command prompt.

**`Step 2:`**
Now after successfully enabling WSL ,we need to enable virtualization capabilities on our windows machine.
For that open command prompt in administrator mode.
Then paste this command (Enable Virtualiztion feature)-

```dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart```

**`Step 3:`**
Now install the WSL update package

**`Step 4:`**
open command prompt in administrator mode
Then paste this command (sets WSL2 as default version)-

```wsl --set-default-version 2```


**`Step 5 :`**
Now go to the Microsoft Store -> install the Linux Distro you prefer(I personally Installed Ubuntu) -> Launch the distro on your windows Device.
Do the setup of username and password for your installed Linux distro.


**`Step 6 :`**
Now install the Docker Desktop and Login with your Docker account.
If you dont have Docker account create one - [DockerHub](https://hub.docker.com/)

**`Step 7 :`**
After this your docker desktop will get started and you will see something like this.
<div align="center">
  
![image](https://user-images.githubusercontent.com/72031540/121762654-fd29d280-cb54-11eb-8ef6-353c8da98f87.png)

</div>

##### Try out the Tutorial .



<div align="center">

![20210612_083402_0000](https://user-images.githubusercontent.com/72031540/121763694-bb505a80-cb5b-11eb-9e13-1bc4b84b783d.png)

 🎊 **YAY,You have successfully installed Docker Desktop** 🎊
</div>



 [![ForTheBadge makes-people-smile](http://ForTheBadge.com/images/badges/makes-people-smile.svg)](http://ForTheBadge.com)
### `If you have any Query Regarding the Installation please feel free to open an issue for this repository I will try my best to help you.`


### `If you found this docker installation process repository helpfull ,please dont forget to give it a ⭐ and do follow me on Github itself 🙂 .`







