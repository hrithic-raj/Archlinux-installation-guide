# Archlinux-installation-guide


[hrj@HRJ ~]$ git clone https://github.com/caelestia-dots/shell.git ~/.local/share/caelestia
Cloning into '/home/hrj/.local/share/caelestia'...
remote: Enumerating objects: 21625, done.
remote: Counting objects: 100% (1353/1353), done.
remote: Compressing objects: 100% (235/235), done.
remote: Total 21625 (delta 1204), reused 1121 (delta 1118), pack-reused 20272 (from 3)
Receiving objects: 100% (21625/21625), 4.52 MiB | 1.22 MiB/s, done.
Resolving deltas: 100% (15322/15322), done.
[hrj@HRJ ~]$ ls ~/.local/share/caelestia
assets  CMakeLists.txt  components  extras  flake.lock  flake.nix  LICENSE  modules  nix  plugin  README.md  scripts  services  shell.qml  utils
[hrj@HRJ ~]$ ~/.local/share/caelestia/install.fish
bash: /home/hrj/.local/share/caelestia/install.fish: No such file or directory
[hrj@HRJ ~]$ 




sudo pacman -S \
kitty \
waybar \
rofi-wayland \
thunar \
dunst \
wl-clipboard \
brightnessctl \
networkmanager





git clone https://aur.archlinux.org/yay.git

cd yay

makepkg -si




[hrj@HRJ yay]$ echo $XDG_CURRENT_DESKTOP
GNOME
[hrj@HRJ yay]$ nvidia-smi
bash: nvidia-smi: command not found
[hrj@HRJ yay]$ hyprland --version
Hyprland 0.55.2 built from branch v0.55.2 at commit 39d7e209c79d451efab1b21151d5938289da838d clean (version: bump to 0.55.2).
Date: Sat May 16 12:59:19 2026
Tag: v0.55.2, commits: 7319

Libraries:
Hyprgraphics: built against 0.5.1, system has 0.5.1
Hyprutils: built against 0.13.1, system has 0.13.1
Hyprcursor: built against 0.1.13, system has 0.1.13
Hyprlang: built against 0.6.8, system has 0.6.8
Aquamarine: built against 0.12.0, system has 0.12.0

Version ABI string: 39d7e209c79d451efab1b21151d5938289da838d_aq_0.12_hu_0.13_hg_0.5_hc_0.1_hlg_0.6
no flags were set

[hrj@HRJ yay]$ ^C
[hrj@HRJ yay]$ cd -
/home/hrj
[hrj@HRJ ~]$ nvidia-smi
bash: nvidia-smi: command not found
[hrj@HRJ ~]$ 


