[hrj@HRJ ~]$ uname -r
7.0.10-arch1-1
[hrj@HRJ ~]$ cat /etc/pacman.conf | grep -v '^#' | grep -v '^$'
[options]
HoldPkg     = pacman glibc
Architecture = auto
Color
CheckSpace
ParallelDownloads = 5
DownloadUser = alpm
SigLevel    = Required DatabaseOptional
LocalFileSigLevel = Optional
[core]
Include = /etc/pacman.d/mirrorlist
[extra]
Include = /etc/pacman.d/mirrorlist
[hrj@HRJ ~]$ sudo pacman -Sy
:: Synchronizing package databases...
 core is up to date
 extra                                                                                                8.2 MiB  3.53 MiB/s 00:02 [#############################################################################] 100%
[hrj@HRJ ~]$ pacman -Ss nvidia | head -20
core/linux-firmware-nvidia 20260519-1 [installed]
    Firmware files for Linux - Firmware for NVIDIA GPUs and SoCs
extra/bumblebee 3.2.1-21
    NVIDIA Optimus support for Linux through VirtualGL
extra/cuda 13.2.1-3
    NVIDIA's GPU programming toolkit
extra/cudnn 9.23.0.39-1
    NVIDIA CUDA Deep Neural Network library
extra/egl-gbm 1.1.3-1
    The GBM EGL external platform library
extra/egl-wayland 4:1.1.21-1 [installed]
    EGLStream-based Wayland external platform
extra/egl-wayland2 1.0.1-1
    EGLStream-based Wayland external platform (2)
extra/egl-x11 1.0.5-1
    NVIDIA XLib and XCB EGL Platform Library
extra/ffnvcodec-headers 13.0.19.0-1
    FFmpeg version of headers required to interface with Nvidias codec APIs
extra/hip-runtime-nvidia 7.2.3-1
    Heterogeneous Interface for Portability (Nvidia runtime)
[hrj@HRJ ~]$ sudo pacman -Syu
:: Synchronizing package databases...
 core is up to date
 extra is up to date
:: Starting full system upgrade...
 there is nothing to do
[hrj@HRJ ~]$ pacman -Qi archlinux-keyring
Name            : archlinux-keyring
Version         : 20260420-1
Description     : Arch Linux PGP keyring
Architecture    : any
URL             : https://gitlab.archlinux.org/archlinux/archlinux-keyring/
Licenses        : GPL-3.0-or-later
Groups          : None
Provides        : None
Depends On      : pacman
Optional Deps   : None
Required By     : base  base-devel
Optional For    : None
Conflicts With  : None
Replaces        : None
Installed Size  : 1763.69 KiB
Packager        : Christian Hesse <eworm@archlinux.org>
Build Date      : Mon 20 Apr 2026 03:13:28 PM IST
Install Date    : Sat 30 May 2026 11:16:27 PM IST
Install Reason  : Installed as a dependency for another package
Install Script  : Yes
Validated By    : Signature

[hrj@HRJ ~]$ pacman -Ss "^nvidia$"
[hrj@HRJ ~]$ pacman -Ss nvidia-utils
extra/nvidia-utils 610.43.02-2
    NVIDIA drivers utilities
[hrj@HRJ ~]$ 
