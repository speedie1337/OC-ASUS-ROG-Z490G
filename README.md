![img](/img/screenshot.png)

# OC-ASUS-ROG-Z490G

**For Catalina, see the *catalina* branch.**

**For Sonoma, see the *sonoma* branch.**

**For the latest version supported, see the *main* branch.**

OpenCore configuration for the ASUS ROG Strix Z490-G Gaming (Wifi) motherboard.

## Note

This config was made for macOS 14.5 Sonoma. It is for sure not going to work with any older version than that. The included version of AirportItlwm itself depends on 14.4 so that should be pretty telling. The config.plist should provide a good baseline, still, even if you want to run another macOS version.

This config is provided as-is, I am not going to provide any support for it. I am however working on Sequoia support right now.

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
- WIFI (built in, using AirportItlwm)
- Bluetooth (built in, using IntelBluetoothFirmware)
- USB 2/3/3.1/3.2 (mapped ports from macOS with USBMap)
  - If you wish to reuse my config, it's very likely that you will have to map the ports yourself, since they won't necessarily be the same for you.
- Full XMP RAM speeds (3600mhz)
- Most likely anything else I did not specify.

*Line out is not functional. My workaround is to simply use the Headphone jack on the front. If you have any idea why this is, please let me know.
