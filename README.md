git clone https://github.com/caelestia-dots/caelestia.git ~/.local/share/caelestia


fish ./install.fish \
  --aur-helper yay \
  --vscode code


[hrj@HRJ caelestia]$ fish ./install.fish \
  --aur-helper yay \
  --vscode code
install.fish: expected <= 0 arguments; got 1
[hrj@HRJ caelestia]$ ^C



[hrj@HRJ caelestia]$ fish ./install.fish
╭─────────────────────────────────────────────────╮
│      ______           __          __  _         │
│     / ____/___ ____  / /__  _____/ /_(_)___ _   │
│    / /   / __ `/ _ \/ / _ \/ ___/ __/ / __ `/   │
│   / /___/ /_/ /  __/ /  __(__  ) /_/ / /_/ /    │
│   \____/\__,_/\___/_/\___/____/\__/_/\__,_/     │
│                                                 │
╰─────────────────────────────────────────────────╯
:: Welcome to the Caelestia dotfiles installer!
:: Before continuing, please ensure you have made a backup of your config directory.
:: [1] Two steps ahead of you!  [2] Make one for me please!





:: Before continuing, please ensure you have made a backup of your config directory.
:: [1] Two steps ahead of you!  [2] Make one for me please!
:: => 1
:: paru not installed. Installing...
[sudo] password for hrj: 
warning: git-2.54.0-1 is up to date -- skipping
warning: base-devel-1-2 is up to date -- skipping
 there is nothing to do
Cloning into 'paru'...
remote: Enumerating objects: 196, done.
remote: Counting objects: 100% (196/196), done.
remote: Compressing objects: 100% (140/140), done.
remote: Total 196 (delta 57), reused 195 (delta 56), pack-reused 0 (from 0)
Receiving objects: 100% (196/196), 63.94 KiB | 10.66 MiB/s, done.
Resolving deltas: 100% (57/57), done.
==> Making package: paru 2.1.0-2 (Sun 31 May 2026 01:46:43 PM IST)
==> Checking runtime dependencies...
==> Checking buildtime dependencies...
==> Installing missing dependencies...
[sudo] password for hrj: 
:: There are 2 providers available for cargo:
:: Repository extra
   1) rust  2) rustup

Enter a number (default=1): ^C
Interrupt signal received

==> ERROR: 'pacman' failed to install missing dependencies.
==> Missing dependencies:
  -> cargo
==> ERROR: Could not resolve all dependencies.
fish: Unknown command: paru
./install.fish (line 147): 
        $aur_helper --gendb
        ^~~~~~~~~~^
:: Installing metapackage...
fish: Unknown command: paru
./install.fish (line 160): 
    $aur_helper -Ui $noconfirm
    ^~~~~~~~~~^
:: /home/hrj/.config/hypr already exists. Overwrite? [Y/n] 
