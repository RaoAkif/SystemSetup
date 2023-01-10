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

## Nodejs LTS, Git, Github, Chrome, Firefox, Visual Studio Code, Zoom
```
choco install nodejs-lts git github-desktop googlechrome firefox visualstudiocode zoom -y
```

## Update All Choco Packages
```
choco upgrade all -y
```

## Uninstall a Package
```
choco uninstall PACKAGENAME
```
---

## GitHub Integration

### Generate SSH Keys
```
ssh-keygen -t rsa -C "raoakif"
```

### Installing Touch-CLI for UNIX systems
```
npm install touch-cli -g
```

## Remove Microsoft Edge Browser
Go to:
`C:\Program Files (x86)\Microsoft\Edge\Application\102.0.1245.44\Installer`
Open cmd prompt: run
```
setup.exe --uninstall --system-level --verbose-logging --force-uninstall
```

