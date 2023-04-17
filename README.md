# popos-fullstack-dev-setup

## Setting up WSL2 
```
# Open PowerShell as admin
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

#list installed versions, if none install
wsl --list --verbose
wsl --set-version #{Distro name} {Distro Version}
wsl --set-default-version 2
```

## Connecting to a running Docker container in WSL
```
#Find out your WSL IP from powershell
wsl hostname -I

#Use that ip to connect to container and don't forget to expose port on container like "-p 5432:5432" for a postgres image
```
