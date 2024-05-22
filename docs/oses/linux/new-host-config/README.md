<!-- Basic Github Header: annebrown.ca -->
<a href="https://annebrown.ca" text-decoration=none><img src="../../../static/img/logo-ab.png" width="20"/></a>annebrown.ca  
<sub><sub><a href="https://github.com/annebrown/?tab=repositories">
    My Repos:</a> <a href="https://github.com/annebrown/docs-priv/">docs-priv/</a> <a href="/oses/linux/new-host-config/"><!-- Basic Github Header: annebrown.ca -->
     oses/linux/new-host-config/<!-- Basic Github Header: annebrown.ca -->
  </a>README.md
</sub></sub>

---
<!-- End of Header -->

# Linux Host Config

> [!NOTE]
> Do this first.

```bash
$ sudo apt update
$ sudo apt update -y
$ git clone https://github.com/annebrown/dotfiles.git ~/.dotfiles
$ cd .dotfiles
$ stow bash vim
$ bash
```
# WSL

```bash
ln -s "/mnt/c/Users/anne/My Drive" ~/gdrive
```

# Configure Git Global Env

See [MyRepos](https://github.com/annebrown/?tab=repositories)
		[/docs-priv/software/git/#git-config](https://github.com/annebrown/docs-priv/software/git/#git-config)

# Gnome Desktop
```bash
$ sudo apt install ubuntu-desktop gnome
```
# xfce4 Desktop
Don't use xfce
Wayland probs.

## Install
```bash
$ sudo apt install xfce4 xfce4-goodies gdm3 xwayland nautilus
```

# Start Desktop
```bash
$ pkill Xwayland; Xwayland :1 & xw_pid=$!; WAYLAND_DISPLAY= DISPLAY=:1 dbus-launch startxfce4; kill $xw_pid
```
or
```bash
$ xfdesktop
```

