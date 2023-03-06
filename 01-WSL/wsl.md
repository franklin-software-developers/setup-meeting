# WSL Installation
Open Windows "Start" menu.
<br><br>
Start typing "Windows Powershell".
<br><br>
"Run as Administrator".
<br><br>
Install WSL.
```
wsl --install
```
Lists all available Linux distros:
```
wsl --list --online
```
Install Ubuntu-20.04 distro specifically.
```
wsl --install -d Ubuntu-20.04
```
Username: [your full name]
```
nurikim
```
Password will not show bullet points as you type! Just type: 
```
ict
```
Update all remote packages.
```
sudo apt update
```
Press ```y``` when asked:
```
sudo apt full-upgrade
```