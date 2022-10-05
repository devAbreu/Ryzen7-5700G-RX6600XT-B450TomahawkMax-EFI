# Ryzen 7 5700G + RX 6600 XT + B450 Tomahawk Max
# OpenCore EFI for AMD Ryzen Hackintosh (Ryzentosh)
## **Remember to change MLB, ROM, Serial Number, UUID** in the config.plist

![Screenshot](screenshot.png?raw=true)

- Builded following this [dortania guide](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#starting-point)

- [Making the installer in windows](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html#downloading-macos)
- [macOS dortania installation process](https://dortania.github.io/OpenCore-Install-Guide/installation/installation-process.html#installation-process)

- <span style="color: red">Clean Install - new volume partition needs to be formatted as</span> <span style="color: #61BD6D">APFS</span>

## Verified Specification

| **Component**    | **Model**                                   |
| ---------------- | ------------------------------------------  |
| CPU              | [AMD Ryzen 7 5700G @ 3.8GHz](https://www.amd.com/en/products/apu/amd-ryzen-7-5700g)                  |
| Motherboard      | [Tomahawk Max B450](https://www.msi.com/Motherboard/B450-TOMAHAWK-MAX/Specification)                           |
| RAM              | 16GB (2x8GB) Corsair Vengeance LPX @ 3200MHz|
| GPU              | MSI RX 6600 XT GAMING X 8G                  |
| Audio Chipset    | Realtek® ALC892 Codec                       |
| Ethernet         | Realtek® RTL8111                            |
| WiFi & Bluetooth | Fenvi HB 1200                               |
| OS Disk          | SAMSUNG 870 EVO SATA 500GB 2.5 SSD          |

**macOS version**: 12.6
**OpenCore version**: 0.8.4

## BIOS Settings

*Don't worry if all of these options don't appear in your BIOS setup, try configuring the ones listed in this table.
| **Option**            | **Status**           |
| --------------------- | -------------------- |
| SATA Mode             | AHCI                 |
| Above 4G Decoding     | Disabled             |
| EHCI/XHCI Hand-off    | Enabled              |
| SVM                   | Enabled              |
| CSM                   | Disabled             |
| Resizable BAR Support | Disabled             |
| Secure Boot           | Disabled             |
| Serial Port           | Disabled             |
| Parallel Port         | Disabled             |




## What is working?

I haven't done much testing on this build. The basics work fine. I've done this build for iOS development purposes.

- Wifi, Ethernet, Audio (AppleALC) front and rear. If you want the mic to work, you must use the VoodooHDA kext method. I have tested it and it works fine. The mic and front/rear audio.

- I had trouble registering an AppleID (iService issues) Just applied [this part](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#fixing-en0) of the dortania guide, and it worked perfectly.

- Bluetooth works fine for me, I've paired with audio devices and it sounds great. Sending files via bluetooth from mac to other devices also works fine for me. I haven't tried it the other way around.

**Note: I will be updating this information over time.**