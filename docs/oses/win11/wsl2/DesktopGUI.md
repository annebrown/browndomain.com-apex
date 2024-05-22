md headers here

## Install Distro
Get Ubuntu Distro from MSStore, then:
```bash
sudo apt-get update
sudo apt-get upgrade
```
## Block ACPI features from being installed
```bash
sudo apt-mark hold acpid acpi-support
```
## 3. Install Desktop
```bash
sudo apt install xfce4 xfce4-goodies gdm3 xwayland nautilus
```

## Run desktop
```bash
pkill Xwayland; Xwayland :1 & xw_pid=$!; WAYLAND_DISPLAY= DISPLAY=:1 dbus-launch startxfce4; kill $xw_pid
```
Reference:
[Easiest WSL2 Desktop Setup Possible](https://www.reddit.com/r/bashonubuntuonwindows/comments/1ajbzyk/easiest_wsl2_desktop_setup_possible/?onetap_auto=true&one_tap=true)

## Configure git
[See Git Config](../../git/README.md)

## Config Host
```bash
git clone https://github.com/annebrown/dotfiles.git .dotfiles
sudo apt install stow
cd .dotfiles
stow bash vim
```
## Install Chrome
Firefox broken on Ubuntu WSL2.  
```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
udo dpkg -i google-chrome-stable_current_amd64.deb
```
If errors during install:
```bash
sudo apt -f install
```
## If gnome-terminal is throwing errors
```bash
wsl --update --pre-release
```
## Non-Desktop Fix
If session won't start for non-desktop apps:
Enable lxdm.

## VSCode Opens in Win11
For WSL2 hosts, do not install VSCode in linux. 
