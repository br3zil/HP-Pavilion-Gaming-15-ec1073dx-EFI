# HP-Pavilion-Gaming-15-ec1073dx-EFI
OpenCore EFI for HP Pavilion Gaming 15 Laptop ec1073dx

Specs:
AMD Ryzen 5 4600H
8GB of RAM (DDR4 3200MHz)
Renoir Integrated APU/GPU (NootedRed)
NVIDIA GTX 1650 (disabled)
WD SN500 256GB NVME SSD
Realtek RTL8822CE (Wi-Fi and Bluetooth, not supported)
Realtek Gaming GbE Family Controller (RTL8111, Ethernet)

Currently working:
Graphics accel (with NootedRed, don't forget to disable GPU accel on apps like discord and browsers!)
Ethernet
Apple ID
Audio + Mic + AUX Port (layout ID 11)
Keyboard
Trackpad (+ native macOS gestures)
USB
Battery status (only for MacBookPro16,2/16,3 SMBIOSes, running MacPro6,1 because its funny)
Webcam
AirPlay (can detect TVs and etc, not actually tested)

Not working:
Shutdown/Reboot (kernel panic)
Any version above Catalina (HP BIOS is screwy with NVRAM on OC and Apple updated the NVRAM installation process in Big Sur and above)
Sleep
OpenVariableRuntimeDxe.efi (needed for fake NVRAM and makes the computer restart instantly when loading into boot picker)



