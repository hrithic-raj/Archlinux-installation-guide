[hrj@HRJ ~]$ nvidia-smi
bash: nvidia-smi: command not found
[hrj@HRJ ~]$ pacman -Qs nvidia
local/egl-wayland 4:1.1.21-1
    EGLStream-based Wayland external platform
local/libvdpau 1.5-4
    Nvidia VDPAU library
local/linux-firmware-nvidia 20260519-1
    Firmware files for Linux - Firmware for NVIDIA GPUs and SoCs
local/vulkan-nouveau 1:26.1.1-2
    Open-source Vulkan driver for Nvidia GPUs
local/xf86-video-nouveau 1.0.18-1 (xorg-drivers)
    Open Source 3D acceleration driver for nVidia cards
[hrj@HRJ ~]$ lspci | grep -E "VGA|3D"
00:02.0 VGA compatible controller: Intel Corporation CometLake-H GT2 [UHD Graphics] (rev 05)
01:00.0 VGA compatible controller: NVIDIA Corporation TU117M [GeForce GTX 1650 Mobile / Max-Q] (rev a1)
[hrj@HRJ ~]$ 







[hrj@HRJ ~]$ sudo pacman -S nvidia nvidia-utils nvidia-settings
[sudo] password for hrj: 
error: target not found: nvidia
[hrj@HRJ ~]$ 
