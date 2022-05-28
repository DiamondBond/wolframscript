# Introduction
Wolframscript 13.0.1 PKGBUILD for Arch Linux.

# Prerequisites
This PKGBUILD needs an rpm downloaded from https://account.wolfram.com/products/downloads/wolframscript placed in the same directory.

# Installation
```
# navigate where you cloned this repo to
cd ~/git/wolframscript

# run makepkg
makepkg -si
```

# Remove
```
yay -R wolframscript
```

# Note
It's probably best to independently manage this package; add it to your
PkgIgnore in /etc/pacman.conf.
