# 2014 Haswell

- Guide Used: [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)
- Installation Date: Mar 7, 2020

# Current Version

- Open Core: v.0.6.0
- macOS Catalina, v.10.15.6 Supplemental Update
- SMBIOS: iMac14,2

# Hardware

- MB [GA-Z87MX-D3H](Extra/Specification-GA-Z87MX-D3H.md) @ BIOS [F7](https://www.gigabyte.com/Motherboard/GA-Z87MX-D3H-rev-1x/support#support-dl-bios)
- CPU Intel Core i5-4670
- iGPU [Intel HD Graphics 4600](https://downloadcenter.intel.com/product/81496/Intel-HD-Graphics-4600)
- dGPU [Sapphire](https://www.sapphiretech.com/en/consumer/nitro-rx-580-4g-g5) [Radeon RX 580 4 GB](https://www.amd.com/en/products/graphics/radeon-rx-580)
- RAM 32 GB 1333 MHz DDR3
- Audio Codec Realtek ALC892
- Ethernet `00:00:00:00:00:00` **I217-V** from Intel 
- Bluetooth: IOGEAR Bluetooth 4.0 USB Micro Adapter (GBU521)
- Wi-Fi: TP-Link AC1750 Wireless Dual Band PCI-Express Adapter (Archer T8E)

# Kexts

- AppleALC
- IntelMausiEthernet
- Lilu
- SMCProcessor
- SMCSuperIO
- VirtualSMC
- USBInjectAll
- WhateverGreen

---

## SMBIOS Info

```
         Model: iMac14,2
      Board ID: Mac-2700000000000000
    FW Version: 141.0.0.0.0
 Hardware UUID: 00000000-0000-0000-0000-000000000000
 Serial Number: 000000000000
       Country:  D25 - Unknown
          Year:    N - 2014
          Week:    V - 50 (10.12.2014-16.12.2014)
          Line:  000 - 000 (copy 1)
         Model: 0000 - iMac14,2
   SystemModel: iMac (27-inch, Late 2013)
         Valid: Possibly
     System ID: 00000000-0000-0000-0000-000000000000
           ROM: 000000000000
           MLB: 00000000000000000
```

---

# BIOS Settings

## Recommended

**Disable:**

- Fast Boot
- VT-d (can be enabled if you set DisableIoMapper to YES)
- CSM
- Intel SGX
- Intel Platform Trust

**Enable:**

- VT-x
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: Windows 8.1/10 UEFI Mode
- DVMT Pre-Allocated(iGPU Memory): 64MB

## Real

**Disable:**


**Enable:**


## Not present in BIOS

**Disable**

- Thunderbolt
- CFG Lock

**Enable**

- VT-x
- Hyper Threading
- Execute Disable Bit
