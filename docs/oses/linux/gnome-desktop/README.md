<!-- Basic Github README.MD Header -->
<div style="text-align: right;"> 
	<a href="https://annebrown.ca">
		<img src="../../../static/img/logo-ab.png" width="20"/>
	</a> 
	annebrown.ca
</div>
<div style="text-align: right;">
	<sub>
		<a href="https://github.com/annebrown/?tab=repositories">MyRepos</a>
		/docs-priv/oses/linux/gnome-desktop/README.md
	</sub>
 </div>
<!-- End of Header -->


# Gnome Desktop

## Dark Theme

```bash
vim ~/.config/gtk-3.0/settings.ini
```

```bash
[Settings]
gtk-application-prefer-dark-theme = true
```

and

```bash
gnome-tweaks&
```

to set **Appearance** > **Legacyt Application**s > **Adwaita-dark**

## Settings Apps

```
gnome-tweaks
gnome-control-center
```

## gnome-terminal

Added to ```.bash_aliases```:

```bash
alias gterm='gnome-terminal --title="$USER@$HOSTNAME: $PWD \$" &'
alias gterm='xfce4-terminal --title="$USER@$HOSTNAME: $PWD \$" &'
```

