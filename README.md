# PLEASE READ THE DETAILS SECTION BEFORE ATTEMPTING TO USE MY EFI

# EFI for Hackintosh-Thinkpad-T470s
Hackintosh Lenovo Thinkpad T470's created with Dortania's open core guide, running macOS Monterey 12.7.6.

![Monterey Screenshot](https://9to5mac.com/wp-content/uploads/sites/6/2022/01/install-macos-monterey-beta.jpg?quality=82&strip=all)

Personally, I will recommend you to make your own EFI as that way you will actually learn how to fix issues that come up, this is a shortcut and teaches you nothing and might leave you confused if you encounter issues. You can download it as a ZIP file or go through the repo to pick specific files.

## DETAILS (IMPORTANT)
:warning: USE PROPERTREE TO EDIT **CONFIG.PLIST** AND USE **GENSMBIOS** TO PUT YOUR OWN **PLATFORM ID INFORMATION**, without it **YOU CANNOT SIGN IN TO APPLE SERVICES**
:warning: This is not a complete EFI, donot use as is, just replace the folders in your own efi with mine when using (USE UR BRAIN)
:warning: Please do read the hardware info before attempting to use EFI, good chance of not working if it doesnt match (except ram and storage etc)
:warning: I am not responsible for responsible for any broken laptops if you mess it up while using it 😛

## Hardware Info
|Hardware|Specifications|
|----|----|
|MacOS|macOS Monterey 12|
|CPU|Intel Core i7-6600u @ 2.6Ghz|
|Graphics|Intel HD Graphics 520|
|RAM|20GB DDR4 2133MHZ|
|Hard-drive|128GB Toshiba M.2 NVME SSD|
|WLAN|Intel Wireless-AC 8620|
|Audio|Realtek ALC298|
|SMBIOS|MacbookPro 13,1| 

## What's working?

- iServices (iCloud, iMessage, Facetime, Photos, etc)
- Laptop keyboard (with backlight0 & touchpad (with gestures)
- Sleep/wake (sometimes touchpad doesnt work after long sleep, just restart)
- GPU acceleration
- Mic and Audio (Issue and temporary fix listed below)
- Volume and brightness keys
- Wifi and bluetooth
- Apple continuity features (pick up call on iPhone from Mac etc)
- All USB ports including type-c (data transfer on c port not tested yet)
- Integrated webcam

## Current issues

- Dual Batteries are not working, I have the right kexts to my knowledge but still haven't been able to get it to work.
- Touch screen is not working, although that should be an easy fix.
- Audio is working, but is very low through the speakers, have to use eqMac to boost it. The BT and 3.5mm audio is working fine though.
- Wifi disconnects randomly/hard to connect, have to go to Network preferences > Advanced > TCP/IP and renew DCHP license for it to work.
- Airdrop is not working but that is due to the card being incompatible with AWDL.

  
NOTE: Rarely it won't shutdown due to some glitch, it keeps restarting instead, just reset the NVRAM and it'll be fixed.

## Acknowledgements
 - [Dortania's open-core guide](https://dortania.github.io/OpenCore-Install-Guide/)

 My thinkpad running Monterey :DDD
 
 ![Laptop picture](https://i.ibb.co/pp648RY/thinkpad.jpg)
