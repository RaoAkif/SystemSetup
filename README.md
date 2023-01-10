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

## Nodejs LTS, Git, Github, Chrome, Firefox, Visual Studio Code, Zoom, Postman
```
choco install nodejs-lts git github-desktop googlechrome firefox visualstudiocode zoom postman -y
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

## Set PowerShell Execution Policy Error in Windows Server
```
Open Powershell with Administrator Access: Type below command,
Set-ExecutionPolicy RemoteSigned
Select Y for Yes
All Set !!!
```

---

## GitHub Commands
```
git init
git add .
git status
git commit -m 'your message'
OR
git commit -a

git remote add origin 'your_url_name'
git push -u origin master

Create & Push on New Branch
git pull
git status
git branch list
git checkout NEW_BRANCH 
git checkout -b NEW_BRANCH
git push origin NEW_BRANCH
git push # if on the same branch
git push --set-upstream origin BRANCH_NAME  // If Upstream never created
git branch -a
git remote add [name_of_your_remote] NEW_BRANCH
git push [name_of_your_new_remote] [url]
```
