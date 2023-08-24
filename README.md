# DO NOT USE | NOT READY FOR USE

# Dell Latitude-7400-Hackintosh Files

## Compatible MacOS Versions
- Ventura

## My System
- Intel Core i7-8650U
- 16GB DDR4 RAM
- Intel UHD 620 Graphics
- Toshiba KIOXIA 512GB SSD
- Intel Wireless-AC 9560

## Completly Working
1) Loudspeaker
2) 3.5mm headphone jack
4) Battery Management
5) Backlight Control (Keys and Software)
7) Touchpad with Gestures
8) WiFi and LAN (per Adapter) (AirportItlwm)
10) USB-C with Power Delivery for Charging
11) Barrel Plug for Charging
13) CPU 
14) iGPU Acceleration
15) Fn Keys

## Not working

## Potential issues

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

## Credits
- toschief
- dortina
- OpenIntelWireless
- All other file creators
