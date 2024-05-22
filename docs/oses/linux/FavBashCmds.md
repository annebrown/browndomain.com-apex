<!-- Basic Github README.MD Header -->
<div style="text-align: right;"> 
	<a href="https://annebrown.ca">
		<img src="../../static/img/logo-ab.png" width="20"/>
	</a> 
	annebrown.ca
</div>
<div style="text-align: right;">
	<sub>
		<a href="https://github.com/annebrown/?tab=repositories">MyRepos</a>
		/docs-priv/oses/linux/FabBashCmds.md
	</sub>
 </div>
<!-- End of Header -->



# Files and Directories

## Aliases set in .bash_aliases

```bash
la # - ls -s
ll # ls -l
```

tree

# SSH

## Client

```bash
sudo apt install -y openssh-client
```

## Connect

```bash
ssh anne@adwv
ssh -v anne@dev # verbose
ssh -o ServerAliveInterval=60 user@host # unstable networks
ssh -2 -o ConnectTimeout=5 
```

# Server

```bash
sudo apt install -y openssh-server
```

Enable ssh server

```bash
sudo systemctl enable ssh
```

Allow ssh Thru Firewall

```bash
sudo ufw allow ssh
```

## Server control

```bash
sudo systemctl start ssh
sudo systemctl stop ssh
sudo systemctl restart ssh
sudo systemctl status ssh
```
