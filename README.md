# Lenovo Ideapad 330-151KB Hackintosh OpenCore

## Hardware Specifications
Processor:	Intel(R) Core(TM) i3-8130U CPU @ 2.20GHz

Graphics:	Intel(R) UHD Graphics 620 

## Test
tested and works on macOS Tahoe 26.2 (25C56)

## Installing/Upgrading macOS
**Coming from Windows/Linux**: If you are on Windows or Linux, follow the guide provided by [**Dortania**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/#making-the-installer). I provide no support for issues with UBS Installers created in Windows or Linux or when installing macOS into a VM!

**Coming from macOS**: If you already have access to macOS, you can either download macOS from the App Store, via the [**OpenCore Legacy Patcher**](https://github.com/dortania/OpenCore-Legacy-Patcher) App or use [**ANYmacOS**](https://www.sl-soft.de/en/anymacos/). Botch can download macOS High Sierra to Ventura and create a USB Installer as well.

## Disable startup messages (Verbose Logs)
 1: Go to config.plist in OC folder 

 2: Search about **boot-args** and remove **-v**

## Notes

`AppleHDA` has been removed from beta 2 so no on-board Audio since AppleALC requires AppleHDA [**Guide**](https://github.com/perez987/AppleHDA-back-on-macOS-26-Tahoe)

To fix wifi you need install heliport
[**Download**](https://github.com/OpenIntelWireless/HeliPort/releases)

Ethernet DOES NOT WORK (Android USB Tethering Works)

Intel UHD Graphics are Spoofed, GPU Acceleration Works

DO NOT BOOT WINDOWS FROM OPENCORE BOOTPICKER, It is not recommended and gives BSOD.

 **Everything works except ethernet**