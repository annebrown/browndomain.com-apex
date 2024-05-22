<!-- Basic Github README.MD Header -->
<div style="text-align: right;"> 
	<a href="https://annebrown.ca">
		<img src="../../static/img/logo-ab.png" width="20"/>
	</a>annebrown.ca
</div>
<div style="text-align: right;">
	<sub>
		<a href="https://github.com/annebrown/?tab=repositories">MyRepos</a>
		/docs-priv/README.md
	</sub>
 </div>
<!-- End of Header -->

# New Host Config


## DO THIS FIRST

```bash
sudo apt update
sudo apt update -y
sudo apt install -y git stow
git clone https://github.com/annebrown/dotfiles.git ~/.dotfiles
cd .dotfiles
stow bash vim
bash
```

### WSL

```bash
ln -s "/mnt/c/Users/anne/My Drive" ~/gdrive
```

# Configure Git Global Env

See [======Insert Reference to ref: git/README.md======].

## Gnome Desktop
```bash
sudo apt install ubuntu-desktop gnome
```

## xfce4 Desktop

### Don't use xfce
Wayland probs.

### Install
```bash
sudo apt install xfce4 xfce4-goodies gdm3 xwayland nautilus
```
### Start Desktop


```bash
pkill Xwayland; Xwayland :1 & xw_pid=$!; WAYLAND_DISPLAY= DISPLAY=:1 dbus-launch startxfce4; kill $xw_pid
```
or
```bash
xfdesktop
```
