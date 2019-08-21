#  ASUS-X299-TUF Mark 1 and All of X299 series

Support CPU:
- i7-7xxx, 9xxx CPU

SMBIOS Used:
- iMacPro1,1

Kext Used:
- Lilu
- AppleALC
- WhateverGreen
- CPUFriend
- VirtualSMC
- SMCProcessor
- SMCSuperIO
- IntelMausiEthernet
- SmallTree-Intel-211-AT-PCIe-GBE
- TSCAdjustReset
* For USB need create a usb map using hackintool *

Drivers Used:
- ApfsDriverLoader
- AppleUISupport
- AptioInputFix
- APtioMemoryFix
- VirtualSMC
- HfsPlus

**Notes:**
- PC00 to PCI0 : Since the PC00 device has many PCI devices, recommend using Patch methods than rename using SSDT.
- LPC0 to LPCB : Same as changing method in PC00 to PCI0
- CPxx to PRxx : No need to rename CPU name. (does not affect sleep and wake up)
- EC0 to EC : No need to rename. To refer to this document 
[SSDT-EC-USBX](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/AcpiSamples/SSDT-EC-USBX.dsl)
