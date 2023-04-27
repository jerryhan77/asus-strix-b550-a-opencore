# AMD Ryzen Hackintosh - Opencore EFI for ASUS ROG STRIX B550-A GAMING

## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 7 5800X @ 3.8GHz |
| Motherboard | ASUS ROG STRIX B550-A GAMING |
| RAM | 32GB (4 x 8GB) T-Force Delta White DDR4-3200 |
| GPU | Power Color Red Devil RX 6800 XT 16G |
| Ethernet | Intel® I225-V 2.5Gb |
| Wi-Fi & Bluetooth | BCM94360CS2 (Wi-Fi) + BRCM20702 (05AC:821f, Bluetooth 4.0) + MHF4 Connector |
| OS Disk (NVME) | ADATA SX8200Pro 512GB |

**macOS version**: 13.3.1

**OpenCore version**: 0.9.1

**SMBIOS**:  MacPro7,1

## Working
- Everything !
- Fixed Ethernet (Intel® I225-V 2.5Gb) issue on MacOS Ventura
- Wi-Fi & Bluetooth
- Airdrop & Handoff (Continuity)
- ResizeableBar is On

## Not working
 - None

## Known Issues
 - None

## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **MacPro7,1**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. Boot it!  

## Credits

 * [jerryhan77](https://github.com/jerryhan77/asus-strix-b550-a-opencore)
 * [RadeonSensor - Kext and Gadget to show Radeon GPU temperature on macOS](https://github.com/aluveitie/RadeonSensor)
 * [AMD Vanilla OpenCore](https://github.com/AMD-OSX/AMD_Vanilla)

## Disclaimer

This documentation is published for the sole purpose of learning and tech enthusiasm and with no guarantees of any kind, I’m not responsible of any harm of any kind or loss of data that may occur.
