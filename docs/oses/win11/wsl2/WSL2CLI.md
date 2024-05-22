md headers here

Run from windows command line.

.exe extension is not required.

```
# Info 
wsl --l		# list distros
wsl -l -v	# verbose list

# Start
wsl
bash
wsl -d distro-name 	        # startup a specific distro
usl -u anne -d distro-name	# login as anne

# Shtudown
wsl --shutdown
wsl -t distro 		# terminate/shutdown a distro

# Change default user 
dist_name config --default-user anne

# Set Default Distro
wsl -s distro-name

# Delete
wsl --unregister distro_name

# Terminate/Shutdown
wsl -t distro_name
wsl --shutdown    # All running distros

```
