## Rebuild Ubuntu Environment
### Download Ubuntu

* Pre-setting
    * window + s -> windows terminal 설치
    * window + s ->  window기능 켜기/끄기 
    * check 'VirtualMachinePlatform'
    * check 'Windows-Subsystem-for-Linux'
    * reboot 

* download vmware
    * window + r -> winver : check the version of window
    * window + s -> powershell(admin) 
    * ```dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart```
    * ```dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart```
    * reboot -> powershell



* download linux 

    * https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi 
    * ```wsl --set-default-version 2``` -> set WSL2 as default version
    * ```wsl -l -v``` or ```wsl --list --verbose``` : check the distributed version of linux
    * if, the version is "1" -> change the version to "2"
    * ex) change the version : ```wsl --set -version Ubuntu 2```