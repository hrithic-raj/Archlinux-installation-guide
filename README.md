[hrj@HRJ caelestia]$ which quickshell
/usr/bin/quickshell
[hrj@HRJ caelestia]$ which caelestia
/usr/bin/caelestia
[hrj@HRJ caelestia]$ ls ~/.config/hypr
hyprland  hyprland.conf  scheme  scripts  variables.conf
[hrj@HRJ caelestia]$ ls ~/.config/fish
config.fish  functions
[hrj@HRJ caelestia]$ 



sed -n '1,50p' ~/.local/share/caelestia/hypr/hyprland.conf



◄ 0s ◎ sed -n '1,50p' ~/.local/share/caelestia/hypr/hyprland.conf             ⌂ 14:27
$hypr = ~/.config/hypr
$hl = $hypr/hyprland
$cConf = ~/.config/caelestia

# Variables (colours + other vars)
exec = cp -L --no-preserve=mode --update=none $hypr/scheme/default.conf $hypr/scheme/current.conf
source = $hypr/scheme/current.conf
source = $hypr/variables.conf

# Maybe create hyprland configs
exec = $hypr/scripts/configs.fish $cConf

# User variables
source = $cConf/hypr-vars.conf

# Default monitor conf
monitor = , preferred, auto, 1

# Configs
source = $hl/env.conf
source = $hl/general.conf
source = $hl/input.conf
source = $hl/misc.conf
source = $hl/animations.conf
source = $hl/decoration.conf
source = $hl/group.conf
source = $hl/execs.conf
source = $hl/rules.conf
source = $hl/gestures.conf
source = $hl/keybinds.conf
source = $hl/scrolling.conf

# User configs
source = $cConf/hypr-user.conf
