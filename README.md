OpenCore Bootloader EFI
======================

| Support |  |
| :--- | :--- |
| Boot Mode | UEFI |
| macOS Support | macOS Sierra 10.12.x, macOS High Sierra 10.13.x, macOS Mojave 10.14.x, macOS Catalina 10.15.x, macOS Big Sur 11 Beta |

## Bootloader 
- **EFI** 
  -    config.plist (for Sandy Bridge processor and newer)
  -    config_amd.plist (for all CPUs AMD Ryzen, Threadripper, Athlon 2xxGE)
  -    /config_laptop/   /config_HD510.plist
                         /config_HD515_520_530_540.plist
                         /config_HD550_P530.plist
                         /config_HD615_620_630_640_650.plist
                         /config_HD3000_1600x900.plist
                         /config_HD3000.plist
                         /config_HD4000_1600x900.plist
                         /config_HD4000.plist
                         /config_HD4600_4400_4200.plist
                         /config_HD5000_5100_5200.plist
                         /config_HD5300_5500_6000.plist
                         /config_HD5600.plists
                         /config_IcelakeG4/G7.plist
                         /config_UHD617(ABL)_620(KBL).plist
                         /config_UHD620.plist
                         /config_UHD630.plist    

## ACPI

| Name | Description |
|:-----|:------------|
SSDT-AWAC.aml | Patch STAS for 300 mainboard series or newer
SSDT-CPUR.aml | Fix CPU definitions with only B550 motherboards (Don't both SSDT-PLUG.aml enable)
SSDT-EC-AMD.aml | Add device EC for AMD systems to fix USB ports
SSDT-EC-USBX.aml | Add device EC and USBX to fix USB ports
SSDT-IMEI.aml | Add device IMEI for CPU Ivy Bridge or older
SSDT-PLUG.aml | Enable CPU power management on Haswell and newer
SSDT-PMCR.aml | Add missing patch PCMR to fix NVRAM for 300 series mainboard or newer
SSDT-PNLF.aml | Enable brightness control for laptop
SSDT-RHUB.aml | Fix USB ports (Root-device errors) on ASUS and MSI 400 series mainboards
SSDT-SMBUS.aml | Add missing device DVL0 in SBUS or SMBU
SSDT-XOSI.aml | Trick our hardware into thinking it's booting Windows to fix touchpad I2C, XHCI,etc

## Kext

| Name | Version | Build date |
|:-----|:-------------|:-----|
[OpenCore Bootloader](https://github.com/acidanthera/OpenCorePkg) | 0.6.3 | 16/10/2020
[AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) |  2.1.1 | 19/10/2020
[AppleALC](https://github.com/acidanthera/AppleALC) | 1.5.4 | 06/10/2020
[AppleMCEReporterDisabler](https://github.com/acidanthera/AppleALC) | 1.2.0 | 10/10/2019
[AtherosE2200Ethernet](https://github.com/Mieze/AtherosE2200Ethernet) | 2.2.2 | 18/11/2018
[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) | 1.1.2 | 03/08/2020
[IntelMausi](https://github.com/acidanthera/IntelMausi) | 1.0.5 | 06/10/2020
[itlwm](https://github.com/OpenIntelWireless/itlwm) | 1.2.0 | 16/10/2020
[Lilu](https://github.com/acidanthera/Lilu) | 1.4.9 | 06/10/2020
[LucyRTL8125Ethernet](https://github.com/Mieze/LucyRTL8125Ethernet) | 1.0.0 | 15/08/2020
[NVMeFix](https://github.com/acidanthera/NVMeFix) | 1.0.5 | 06/10/2020
[RealtekRTL8100](https://github.com/Mieze/RealtekRTL8100) | 2.0.1 | 11/05/2018
[RealtekRTL8111](https://bitbucket.org/RehabMan/os-x-realtek-network/downloads/) | 2.3.0 | 22/03/2017
[USBInjectAll](https://github.com/RehabMan/OS-X-USB-Inject-All) | 0.7.1 | 09/11/2018
[VirtualSMC](https://github.com/acidanthera/VirtualSMC) | 1.1.8 | 11/10/2020
[VoodooI2C](https://github.com/VoodooI2C/VoodooI2C) | 2.5.1 | 06/10/2020
[VoodooPS2Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller) | 1.9.2 | 08/10/2018
[WhateverGreen](https://github.com/acidanthera/WhateverGreen) | 1.4.4 | 08/10/2020

## How to use?

    Run script gitBootloaderEFI.bat (Windows) or gitBootloaderEFI.command (macOS)

<img src="https://media.giphy.com/media/LnQjpWaON8nhr21vNW/giphy.gif" width="60"> <b> If you need support, contact me to [my facebook](https://www.facebook.com/lzhoang2601) or join [my discord](https://discord.gg/4cDFWPw) </b>
