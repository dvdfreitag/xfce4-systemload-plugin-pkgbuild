# xfce4-systemload-plugin-pkgbuild

## Building from scratch and installing

1. Clone this repository
2. Download, extract, configure, and build with makepkg
3. Install with makepkg (or pacman)

```bash
# Clone
git clone https://github.com/dvdfreitag/xfce4-systemload-plugin-pkgbuild.git
cd xfce4-systemload-plugin-pkgbuild
# Install any dependencies before downloading and building
makepkg --syncdeps
# Install package
makepkg --install
# Or, install package using pacman directly
pacman -U xfce4-systemload-plugin-1.2.4dovid-1-x86_64.pkg.tar.xz
```

## Installing a binary release

1. Navigate to the "Releases" page [here](https://github.com/dvdfreitag/xfce4-systemload-plugin/releases), and download the newest release
2. Use pacman to install the file

```bash
# Download release
wget https://github.com/dvdfreitag/xfce4-systemload-plugin/releases/download/1.2.4dovid/xfce4-systemload-plugin-1.2.4dovid-1-x86_64.pkg.tar.xz
# Install it
pacman -U xfce4-systemload-plugin-1.2.4dovid-1-x86_64.pkg.tar.xz
```
