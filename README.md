# whiteblack-hackintosh
MSI B360m Mortar | i5-8400 | 16GB RAM | Sapphire Pulse RX 580 8GB | macOS Mojave 10.14.2 Vanilla Install

# Kexts
| Tables                   | Version            | URL                                           |
| ------------------------ |------------------- | --------------------------------------------- |
| FakeSMC                  | 2018-0915          | <https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/> |
| IntelMausiEthernet       | 2.5.0d0            | <https://github.com/Mieze/IntelMausiEthernet> |
| USBInjectAll             | 0.7.1 (2018-1108)  | <https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/> |
| Lilu                     | 1.2.8              | <https://github.com/acidanthera/Lilu/releases> |
| AppleALC                 | 1.3.3              | <https://github.com/acidanthera/AppleALC/releases> |
| WhateverGreen            | 1.2.4              | <https://github.com/acidanthera/WhateverGreen/releases> |
| XHCI-unsupported         | 0.9.2 (2018‑10‑20) | <https://bitbucket.org/RehabMan/os-x-usb-inject-all/src> |

# Hardware Acceleration

Have to enable Multi-Monitor in BIOS

![Hardware Acceleration Screenshot](https://i.imgur.com/oUJzwrj.png?1)

# Tools
- IORegistryExplorer_v2.1: https://github.com/toleda/audio_ALCInjection/blob/master/IORegistryExplorer_v2.1.zip
- VideoProc: https://www.macxdvd.com/mac-video-converter-pro/
https://www.macxdvd.com/download/macx-video-converter-pro.dmg
- FBpatcher: http://headsoft.com.au/download/mac/FBPatcher.zip

# Tips

Turn off GateKeeper (Open app from Anywhere), run `sudo spctl --master-disable` and `sudo spctl --master-enable` to turn it on.
