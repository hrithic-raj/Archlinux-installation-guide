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
