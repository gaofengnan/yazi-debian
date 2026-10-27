![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/gaofengnan/yazi-debian/total)
![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/gaofengnan/yazi-debian/latest/total)
![GitHub Release](https://img.shields.io/github/v/release/gaofengnan/yazi-debian)
![GitHub Release Date](https://img.shields.io/github/release-date/gaofengnan/yazi-debian)

<h1>
   <p align="center">
     <a href="https://yazi.org/"><img src="https://github.com/gaofengnan/yazi-debian/blob/main/yazi-logo.png" alt="yazi Logo" width="128" style="margin-right: 20px"></a>
     <a href="https://www.debian.org/"><img src="https://github.com/gaofengnan/yazi-debian/blob/main/debian-logo.png" alt="Debian Logo" width="104" style="margin-left: 20px"></a>
     <br>yazi for Debian
   </p>
</h1>
<p align="center">
 Yazi (means "duck") is a terminal file manager written in Rust, based on non-blocking async I/O. It aims to provide an efficient, user-friendly, and customizable file management experience.
</p>

# yazi for Debian

> Fork of [dariogriffo/yazi-debian](https://github.com/dariogriffo/yazi-debian) (MIT); the original packaging is by Dario Griffo. Served at [deb.gaofn.xyz](https://deb.gaofn.xyz) for Debian 12 (bookworm) and 13 (trixie).

This repository contains build scripts to produce the _unofficial_ Debian packages
(.deb) for [yazi](https://github.com/sxyazi/yazi/) hosted at [deb.gaofn.xyz](https://deb.gaofn.xyz)

Currently supported debian distros are:
- Bookworm
- Trixie
- Sid

This is an unofficial community project to provide a package that's easy to
install on Debian. If you're looking for the yazi source code, see
[yazi](https://github.com/sxyazi/yazi/).

## Install/Update

### The Debian way

```sh
sudo install -d -m 0755 /etc/apt/keyrings
sudo curl -fsSL https://deb.gaofn.xyz/deb.gaofn.xyz.gpg -o /etc/apt/keyrings/deb.gaofn.xyz.gpg
sudo curl -fsSL https://deb.gaofn.xyz/deb.gaofn.xyz.sources -o /etc/apt/sources.list.d/deb.gaofn.xyz.sources
# Debian 12 (bookworm): fetch deb.gaofn.xyz-bookworm.sources instead
sudo apt update
sudo apt install -y yazi
```

### Manual Installation

1. Download the .deb package for your Debian version available on
   the [Releases](https://github.com/gaofengnan/yazi-debian/releases) page.
2. Install the downloaded .deb package.

```sh
sudo dpkg -i <filename>.deb
```
## Updating

To update to a new version, just follow any of the installation methods above. There's no need to uninstall the old version; it will be updated correctly.

## Roadmap

- [x] Produce a .deb package on GitHub Releases
- [x] Set up a debian mirror for easier updates

## Disclaimer

- This repo is not open for issues related to yazi. This repo is only for _unofficial_ Debian packaging.
