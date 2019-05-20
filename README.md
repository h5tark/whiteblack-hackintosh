# whiteblack-hackintosh
MSI B360m Mortar | i5-8400 | 16GB RAM | Sapphire Pulse RX 580 8GB | **macOS Mojave 10.14.5** Vanilla Install



# But first..

You should generate new SmUUID, SerialNumber and BoardSerialNumber with uuidgen & [macserial](https://github.com/acidanthera/MacInfoPkg/releases). Then update in` EFI/CLOVER/config.plist` file, under section `SMBIOS`, line 313 is BoardSerialNumber, line 317 is SerialNumber. 

Command

```bash
macserial -a | grep -i iMac19,1
```

Will output like this

```bash
iMac19,1 | SerialNumber | BoardSerialNumber
```



Open Terminal, run `uuidgen` then paste the output to line 319 (SmUUID).



# Sleep issue

Download [Hackintool](http://headsoft.com.au/download/mac/Hackintool.zip), open tab Power -> Fix sleepimage.



# Mainboard BIOS

- 1.60 - 2019-04-01 - ([7B23v16](https://www.msi.com/Motherboard/support/B360M-MORTAR#down-bios)) - WORKING WITH DSDT PATCH

- 1.30 - 2018-08-02 - ([7B23v13](https://www.msi.com/Motherboard/support/B360M-MORTAR#down-bios)) - WORKING WITHOUT DSDT PATCH (config.plist line 108-117)

  

# Mainboard BIOS Setting
- Multi-monitor: Enabled

- ErP Ready: Enabled

- Wake with USB: on (optional)

  

# Clover v2.4k_r4929
Download: <https://github.com/Dids/clover-builder/releases>

**Important:** When install new Clover to EFI, on the Installation Type step, click `Customize` then **uncheck** `AptioMemoryFix-64` in `UEFI Drivers` (MSI board won't boot without doing this).



# Kexts
| Tables             | Version            | URL                                                          |
| ------------------ | ------------------ | ------------------------------------------------------------ |
| VirtualSMC         | 1.0.3              | <https://github.com/acidanthera/VirtualSMC/releases>         |
| IntelMausiEthernet | 2.5.0d0            | <https://github.com/Mieze/IntelMausiEthernet>                |
| USBInjectAll       | 0.7.1 (2018-1108)  | <https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/> |
| Lilu               | 1.3.5              | <https://github.com/acidanthera/Lilu/releases>               |
| AppleALC           | 1.3.7              | <https://github.com/acidanthera/AppleALC/releases>           |
| WhateverGreen      | 1.2.8              | <https://github.com/acidanthera/WhateverGreen/releases>      |
| XHCI-unsupported   | 0.9.2 (2018‑10‑20) | <https://bitbucket.org/RehabMan/os-x-usb-inject-all/src>     |



# Hardware Acceleration

Have to enable Multi-Monitor in BIOS

![Hardware Acceleration Screenshot](https://i.imgur.com/GrFYbrl.jpg)

# Tools
- IORegistryExplorer_v2.1: https://github.com/toleda/audio_ALCInjection/blob/master/IORegistryExplorer_v2.1.zip
- VideoProc: https://www.macxdvd.com/mac-video-converter-pro/
https://www.macxdvd.com/download/macx-video-converter-pro.dmg
- FBpatcher: http://headsoft.com.au/download/mac/FBPatcher.zip
- Hackintool: http://headsoft.com.au/download/mac/Hackintool.zip



# Tips

Turn off GateKeeper (Open app from Anywhere), run `sudo spctl --master-disable` and `sudo spctl --master-enable` to turn it on.
