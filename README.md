# System Setup

## Install Chocolatey
Open `CMD` with Admin permission and run:
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

### Enlist Choco Packages
```
choco list --local-only
```

## Template for Choco Commands
```
choco install PACKAGENAME -y
```

## Nodejs LTS, Git, Github, Chrome, Firefox
```
choco install nodejs-lts git googlechrome firefox visualstudiocode -y
```

## Update All Choco Packages
```
choco upgrade all -y
```

## Uninstall a Package
```
choco uninstall PACKAGENAME
```
