# ONLY USE WITH THIS SYSTEM OR EDIT FOR YOUR SYSTEM

# Dell Latitude-7400-Hackintosh Files

## Compatible MacOS Versions
- Ventura

## My System
- Intel Core i7-8665U
- 16GB DDR4 RAM
- Intel UHD 620 Graphics
- Toshiba KIOXIA 512GB SSD
- Intel Wireless-AC 9560

## Completly Working
Not tested

## Not working
Not tested

## Confirmed issues
Open issue for it to be listed

## Unknown (not tested)
Everything not listet above

# Install Guide

## Creating the USB
- Create the USB like here: https://dortania.github.io/OpenCore-Install-Guide/installer-guide/#creating-the-usb
- Download the EFI for your version
- Copy the EFI on the USB

## BIOS Setup
- Boot into BIOS using f2 key
- Reset to default BIOS
- Reboot into BIOS
-------------------------------------------------------------------
- Advanced Boot Options - all unchecked
- UEFI Boot Path Security - Always, Except internal HDD
 
- SATA Operations - AHCI

- Secure Boot Enable - Disabled
- Expert Key Management - unchecked
  
- Intel SGX Enable - Enabled
- Enclave Memory Size - 64MB
  
- Fastboot - Thorough
  
- Virtualization - unchecked
- VT for Direct I/O - unchecked

## Boot
- Boot into Boot-Menu using f12 key
- Select USB
- If it reboots try again
- When in Opencore menu press space
- Select the orange dmg

## Install
- Connect to WIFI or LAN
-------------------------------------------------------------------
- Open Disk Utility
- Select "Show all devices" under view
- Select your disk
- Click erase then select "APFS" and type a name
- Exit Disk Utility
-------------------------------------------------------------------
- Open Reinstall macOS
- Go throught
-  Wait
-------------------------------------------------------------------
- If succesful it will reboot sometimes
- Select macOS Installer if reboot to Opencore menu

## Post-Install
- Configure macOS as you like
- Do this: https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html#grabbing-opencore-off-the-usb
- Have fun!

# Extras

## Editing the EFI
- Use this: https://dortania.github.io/OpenCore-Install-Guide/ or other sites

## Credits
- toschief
- dortina 
- OpenIntelWireless
- All other file creators
