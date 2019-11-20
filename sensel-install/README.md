# Installation of Sensel Library

The sensel lib must be installed to use the functions provided!

## Arch linux install:

```
# Install debtap (outside of this repo)
git clone https://aur.archlinux.org/debtap.git
cd debtap
makepkg -si


# Navigate to this directory (sensel-install)
cd sensel-install
debtap -P senselliblinux0.8.2.deb
cp senselliblinux0.8.2.deb sensellib
cd sensellib
makepkg -si
```
