## **[Dell Optiplex 7010 USFF](https://github.com/hackintosh-club/DELL-7010-USFF-OpenCore)  Hackintosh OpenCore EFI**

![image](ScreenShot/dell7010usff.jpg)

### [简体中文](https://github.com/hackintosh-efi/MAG-B660M-MORTAR-WIFI-DDR4-OpenCore)

[OpenCore 10.4](https://github.com/acidanthera/OpenCorePkg)

### OS Version Tested

- macOS Big Sur 11.x
- macOS Monterey 12.x  ( Need to install KDK and use OCLP to patch )

### Hardware

- Motherboard: DELL Q77 Express
- bios Version:  A29（06/28/2018）
- CPU: Intel 3th  i7-3770  @ 3.40GHz Quad-core
- RAM: Crucial DDR3L 1600MHz 8GB×2
- iGPU: Intel HD Graphics 4000
- SSD: XSJ-X100-512GB SATA SSD macOS 12.7.5
- Audio: Realtek ALC265
- Ethernet: Intel  82579LM
- Wireless: Dell Wireless 1705 （Cannot be used in Hackintosh）

### BIOS Setup

```
General
     |-- Boot Sequence：boot List Option -- UEFI
     |-- Advanced Boot Options：Enable Legacy Option ROMs - unCheck  ❎  

System Configuration
	   |-- SATA Operation: AHCI
Video
	   |-- Primary Display: Intel HD Graphics
Security
	   |-- TPM Security - uncheck  ❎  
Secure Boot
	   |-- Secure Boot Enable: Disabled
PowerManagement
	   |-- USB Wake Support: Disabled
	   |-- Block Sleep (S3 State): Check ✅
```

### Notes

- Use [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools/releases) build your SMBIOS
- The original built-in wireless network card Dell Wireless 1705 is Qualcomm QCA9565, which cannot be used in Hackintosh
- Must install the KDK compatible with macOS Monterey in order to use OCLP to apply the integrated graphics patch and enable the HD Graphics 4000
- This EFI does not support macOS 13 Ventura and Higher OS

### Contact Us

- QQ Group: 23304408

![image](ScreenShot/QRCode.png)
