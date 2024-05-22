
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
		/docs-priv/oses/linux/SSH.md
	</sub>
 </div>
<!-- End of Header -->

# SSH Password-less Logins



```bash
ssh-keygen -t rsa
eval $(ssh-agent -s)
ssh-add ~/.ssh/filename
ssh-copy-id user@host.com
ssh-keyscan -H host.com >> ~/.ssh/known_hosts
vim config
```

~/.ssh/config:
```
Host hostnamealias
        HostName hostname
        IdentityFile=~/.ssh/hostname
        User username
```
## Example:
```bash
ssh-keygen -t rsa
eval $(ssh-agent -s)
ssh-add ~/.ssh/adev
ssh-copy-id anne@adev
ssh-keyscan -H adev >> ~/.ssh/known_hosts
```
~/.ssh/config:
```bash
config:
Host dev
  Hostname adev
  IdentityFile=~/ssh/adev
  User anne

  ```
