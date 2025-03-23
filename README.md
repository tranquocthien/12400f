### GIGABYTE H610 - 12400F: sonoma

## BIOS

### Disable
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- VT-d
- Compatibility Support Module (CSM)
- Thunderbolt
- Intel SGX
- Intel Platform Trust
- CFG Lock (MSR 0xE2 write protection)

### Enable
VT-x
- Above 4G Decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: Other OS
- DVMT Pre-Allocated(iGPU Memory): 64MB hoặc cao hơn
- SATA Mode: AHCI

bt403: Dùng IntelBluetoothFirmware.kext và BlueToolFixup.kext (BrcmPatchRAM)


doge:DMYYzcma9eefrB8Ys1RU3CU8KR4wsn2oDL


### MSI H610 - 12400F: sonoma

1. Hardware Compatibility Check:

Before starting, ensure that all your hardware components are compatible with macOS. Check online resources and compatibility lists to verify compatibility with the specific macOS version you intend to install.
2. BIOS Settings:

Access your motherboard's BIOS settings and configure them appropriately for Hackintosh compatibility. Key settings may include:
Disable Secure Boot.
Set SATA mode to AHCI.
Disable CFG Lock.
Enable XHCI Handoff.
Disable VT-d (if applicable).
Disable CSM.
3. Create macOS Installer:

Use a real Mac or a macOS virtual machine to create a bootable macOS installer USB drive. You can use tools like Disk Utility or createinstallmedia command in Terminal.
4.  Configuration:

Download the latest version of  bootloader.
Configure your config.plist file according to your hardware specifications. Pay attention to ACPI, Kernel, and DeviceProperties sections.
Include necessary ACPI patches and SSDTs for your specific motherboard and CPU.
5. Graphics Card Setup:

For your RX 6700 XT Pulse GPU , ensure that you have the necessary framebuffer patches in your config.plist to enable full graphics acceleration.
Use WhateverGreen.kext and Lilu.kext for proper GPU functionality.
6. Installation Process:

Boot from your macOS installer USB drive.
Install macOS on your target drive.
After installation, boot from the  bootloader on your target drive.
7. Post-Installation Setup:

Install essential kexts using a kext installer or manually into your EFI partition.
Configure network, audio, and other drivers as needed for full functionality.
Test various features and functionalities to ensure everything works as expected.
8. Troubleshooting:

If you encounter any issues or errors during installation or post-installation, refer to online resources, forums, and Hackintosh communities for assistance.
Check logs, Kernel Panic s, and error messages for clues on how to resolve any issues.
9. Optional: DRM Content Testing:

If you use Safari for streaming DRM-protected content, test DRM playback to ensure compatibility.
By following these steps and ensuring proper configuration, you can achieve a Success ful macOS Hackintosh setup with the MSI H610M-E motherboard, Intel Core i5-12400F CPU, and RX 6700 XT Pulse GPU . Enjoy your Hackintosh experience!
