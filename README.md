# Asus Z370-I Hackintosh

![Asus Z370-I Hackintosh](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/nzxt-h200-asus-z370-i.jpg)

## Components

| Component         | Manufacturer | Model
| ----------------- | -------------| ---
| CPU               | Intel        | [Core i5-9600K](https://ark.intel.com/content/www/us/en/ark/products/134896/intel-core-i5-9600k-processor-9m-cache-up-to-4-60-ghz.html)
| CPU Cooler        | Corsair      | [Hydro Series H60 (2018) 120mm AIO](https://www.corsair.com/us/en/Categories/Products/Liquid-Cooling/Single-Radiator-Liquid-Coolers/Hydro-Series™-H60-%282018%29-120mm-Liquid-CPU-Cooler/p/CW-9060036-WW)
| Motherboard       | Asus         | [ROG Strix Z370-I Gaming](https://www.asus.com/us/Motherboards/ROG-STRIX-Z370-I-GAMING/)
| Memory            | Corsair      | [Vengeance LPX 16GB (2x8GB) DDR4 DRAM 3000MHz C15](https://www.corsair.com/us/en/Categories/Products/Memory/vengeance-lpx-black/p/CMK16GX4M2B3000C15)
| Storage           | Samsung      | [970 EVO 1TB - NVMe PCIe M.2 2280 SSD](https://www.samsung.com/us/computing/memory-storage/solid-state-drives/ssd-970-evo-nvme-m-2-1tb-mz-v7e1t0bw/)
| Video Card        | MSI          | [Radeon RX Vega 64](https://www.msi.com/Graphics-card/Radeon-RX-Vega-64-8G)
| Video Card Cooler | AlphaCool    | [Eiswolf 240 GPX Pro AMD RX Vega M01](https://www.alphacool.com/shop/neue-produkte/22291/alphacool-eiswolf-120-gpx-pro-amd-rx-vega-m01-black)
| Case              | NZXT         | [H200](https://www.nzxt.com/products/h200-matte-white)
| Power Supply      | Corsair      | [SF750 SFX 80+ Platinum](https://www.corsair.com/us/en/Categories/Products/Power-Supply-Units/Power-Supply-Units-Advanced/SF-Series/p/CP-9020186-NA)
| Fan Controller    | Corsair      | [iCUE Commander PRO](https://www.corsair.com/us/en/Categories/Products/CORSAIR-LINK/iCUE-Commander-PRO-Smart-RGB-Lighting-and-Fan-Speed-Controller/p/CL-9011110-WW)
| Top Case Fan      | Noctua       | [NF-S12A PWM](https://noctua.at/en/nf-s12a-pwm)
| CPU/GPU Rad Fans  | Noctua       | [NF-A12x25 PWM](https://noctua.at/en/nf-a12x25-pwm)
| Wi-Fi/Bluetooth   | Dell         | [DW1560 M.2 NGFF (Broadcom BCM94352Z)](https://wikidevi.com/wiki/Dell_Wireless_1560_(DW1560))

## EFI

### ACPI

These files go in /EFI/CLOVER/ACPI/patched:
* [SSDT-UIAC.aml](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/SSDT-UIAC.aml?raw=true) - USB port mappings
* [SSDT-USBX.aml](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/SSDT-USBX.aml?raw=true) - USB power properties

### drivers64UEFI

| Driver                          | Purpose
| ------------------------------- | ---
| ApfsDriverLoader-64.efi         | Apple File System support.
| AptioMemoryFix-64.efi           | Allows macOS to boot with UEFI.
| HFSPlus.efi                     | HFS+ support.

### kexts

| Kext                                 | Purpose
| ------------------------------------ | ---
| AirportBrcmFixup.kext                | Wi-Fi
| AppleALC.kext                        | Audio
| BrcmFirmwareData, BrcmPatchRAM2.kext | Bluetooth
| IntelMausiEthernet.kext              | Ethernet
| Lilu.kext                            | Kext/process patching
| NoVPAJpeg.kext                       | Fixes preview/quicklook when integrated graphics are disabled
| USBInjectAll.kext                    | Injects all ports for each USB controller
| VirtualSMC.kext                      | SMC emulator
| WhateverGreen.kext                   | Patches for GPUs

## Screenshots

| ![Boralus](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/Screen%20Shot%202019-02-25%20at%204.46.13%20PM.jpg) | 
|:--:| 
| *Boralus* |

| ![Atal'Dazar](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/Screen%20Shot%202019-03-11%20at%2010.00.58%20PM.png) | 
|:--:| 
| *Atal'Dazar* |

| ![Pandaria](https://github.com/phine-eredar/asus-z370-i-hackintosh/blob/master/Screen%20Shot%202019-03-20%20at%2012.00.18%20AM.png) | 
|:--:| 
| *Pandaria* |
