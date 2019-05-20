**OsxAptioFixDrv** and OsxAptioFix2Drv reverted to rev before 4368 so without NVRAM support. Let them stay here for history. And sometimes OsxAptioFixDrv is only working version for high warped memory map.

**OsxAptioFix2Drv** is a reduced version without relocation blocks and may not works on some hardware or with older OS version. But this version supported Hibernation while first one no.

**OsxAptioFix3Drv** is a OsxAptioFix2Drv rev 4369 renamed to be different. This version supported NVRAM. More runtime fixes in 4379. This version can be improved by clover crew in future.

**AptioMemoryFix** included in the package is third-party memory fix driver used as is. It is probably better then OsxAptioFix*. Choose it for a first attempt.

**OsxLowMemFixDrv** is also memory fix driver, not improved since rev608.

SIC! These 5 drivers should not be used simultaneously! Choose one of them!

Clover will be updated for mutually exclusion.

 

**AptioInputFix** is included in the package now. It is keyboard driver to support FileVault2 for those who have AMI UEFI BIOS.