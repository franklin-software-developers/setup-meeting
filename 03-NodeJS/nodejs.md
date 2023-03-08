# Install NodeJS
Open PowerShell in VSCode and type:
```
bash
```
Download Node Version Manager (NVM).
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
Open up the bash profile file using VSCode.
```
code ~/.bash_profile
```
Copy this into the file that pops up.
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

Go back to PowerShell, copy and paste to 'save' changes: <br>
 ```
 source ~/.bash_profile
 ```
Use nvm to install the latest stable version of node.
 ```
 nvm install --lts
 ```
 If this outputs a version number, everything installed correctly!<br>
```
node -v
```