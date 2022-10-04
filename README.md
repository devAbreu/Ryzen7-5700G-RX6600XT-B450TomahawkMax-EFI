# Ryzen 7 5700G + RX 6600 XT + B450 Tomahawk Max

![Screenshot](screenshot.png?raw=true)

Builded following this [dortania guide](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#starting-point)

# OpenCore EFI for AMD Ryzen Hackintosh (Ryzentosh)

## Verified Specification

| **Component**    | **Model**                                   |
| ---------------- | ------------------------------------------  |
| CPU              | AMD Ryzen 7 5700G @ 3.8GHz                  |
| Motherboard      | Tomahawk Max B450                           |
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

I haven't done much testing on this build. The basics work fine.

- Wifi, Ethernet, Audio (AppleALC) front and rear. If you want the mic to work, you must use the VoodooHDA kext method. I have tested it and it works fine. The mic and front/rear audio.

- I had trouble registering an AppleID (iService issues) Just applied [this part](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#fixing-en0) of the dortania guide, and it worked perfectly.

- Bluetooth works fine for me, I've paired with audio devices and it sounds great. Sending files via bluetooth from mac to other devices also works fine for me. I haven't tried it the other way around.

**Note: I will be updating this information over time.**