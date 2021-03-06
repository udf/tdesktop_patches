# Note: Please use the aur package instead: [telegram-desktop-udf-patched](https://aur.archlinux.org/packages/telegram-desktop-udf-patched)

# tdesktop patches
Various patches for [Telegram desktop](https://github.com/telegramdesktop/tdesktop/)

# Usage
(I should probably make this into a PKGBUILD but ¯\\\_(ツ)\_/¯)

These instructions are for Arch Linux, if you use some other distro, reevaluate
your life choices.

1. Clone this PKGBUILD: https://aur.archlinux.org/packages/telegram-desktop-dev/
1. Clone this repo into the same place you cloned the PKGBUILD (or anywhere,
   really)
1. `makepkg --nobuild` to fetch the sources

Apply the patches:
1. `cd src/tdesktop`
1. `git apply /path/to/patch.patch` for each patch that you want
1. `cd ../..`

Build Telegram Desktop with `makepkg --noextract`  
Install Telegram with `sudo pacman -U telegram-desktop-dev-*.pkg.tar.xz`

# Credit
[@streetwalrus](https://github.com/Streetwalus) for [most of the patch ideas](https://github.com/Streetwalrus/dotfiles/blob/571c41d7db651c42068a8101389074027d5ce732/scripts/telegram-desktop).
