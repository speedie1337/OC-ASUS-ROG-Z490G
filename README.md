![img](/img/screenshot.png)

# OC-ASUS-ROG-Z490G

**For Catalina, see the *catalina* branch.**

**For Sonoma, see the *sonoma* branch.**

**For the latest version supported, see the *main* branch.**

OpenCore configuration for the ASUS ROG Strix Z490-G Gaming (Wifi) motherboard.

## Note

This config was made for macOS 14.5 and later updated for 15.0 Sequoia. Whether it works on 14.5
still is uncertain.

**This config is provided as-is, I am not going to provide any support for it.**

## Specifications

The specifications of my system. This config will very likely work with similar configurations.

- Motherboard: ASUS ROG Strix Z490-G Gaming (Wifi)
- CPU: Intel Core i9 10900 (10c/20t) @ 5.20Ghz
- GPU: AMD Radeon RX 570 (8GB)
- RAM: 2x16GB Corsair Vengeance @ 3666Mhz
- Storage: Any NVMe SSD, really. Avoid PM981 though ;)

## Functionality

- GPU acceleration (natively)
- Ethernet (using AppleIGC)
- Audio (using AppleALC with layout 7)*
- Bluetooth (built in, using IntelBluetoothFirmware)
- USB 2/3/3.1/3.2 (mapped ports from macOS with USBMap)
  - If you wish to reuse my config, it's very likely that you will have to map the ports yourself, since they won't necessarily be the same for you.
- Full XMP RAM speeds (3600mhz)
- Most likely anything else I did not specify.

*Line out is not functional. My workaround is to simply use the Headphone jack on the front. If you have any idea why this is, please let me know.

## Not working

- Wifi
  - Can be fixed by adding AirportItlwm or itlwm.kext. itlwm.kext has been tested and works, but requires Heliport to work. Because I use Ethernet on my desktop I've opted not to include it until AirportItlwm has been updated for the latest macOS version.
