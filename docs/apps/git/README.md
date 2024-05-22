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
		/docs-priv/software/git/README.md
	</sub>
 </div>
<!-- End of Header -->

# Git

## Git Config

```bash
git config --global user.name "Anne Brown"
git config --global user.email anne@browndomain.com
```

## Personal Access Token

### Create PAT	
Go to github.com -> Settings -> Developer

### Confgure Authentication Manager

Use Github Credential Manager (GCM) in WSL.

```bash
git config --global credential.helper store
```
Git Authn Mgr stores creds on next login.

