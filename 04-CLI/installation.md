# 📩 **Installation**
We will be downloading important tools to help setup our development environment (a workspace made of software applications that help us develop an app).

## **＞ Command Line Interface (CLI)**
The command line interface is a text-based program that runs on computers. Instead of using your mouse to point and click at graphic icons, use the CLI to type only a couple keywords to accomplish the same (and even more) actions in a fraction of the time. <br>
Here are some actions the CLI can do faster and easier:

<details>
    <summary>Navigating and creating folders and files</summary>
    <img src="images/cli-with-gui-output.gif">
</details>

<details>
    <summary>Opening existing applications</summary>
    <img src="images/cli-opening-app.gif">
</details>

<li>Downloading software</li>
<li>Interacting with GitHub repositories</li>
<br>

*Using the CLI increases our productivity as developers.*
<br>

## 🐧 **WSL**
WSL is a CLI app offered by Microsoft that allows you to run Linux commands on a Windows computer.
<details>
    <summary>What is Linux?</summary>
    Windows and MacOS are both operating systems, the essential software that manages the computer's software and hardware. Like Windows and MacOS, Linux is another operating system (OS). However, Linux is an open-source OS, meaning its users can freely access, redistribute and modify it, a huge reason it rose in popularity.
</details>

### ***Downloading WSL***
<ol>
    <li>
        <details>
            <summary>"Run [Windows PowerShell] as Administrator"</summary>
            <img src="images/running-powershell-as-administrator.jpg">
        </details>
    </li>
    <li>Once open type this command: <br><code>wsl --install -d Ubuntu</code></li>
    <li>Wait through installation:</li>
        <ul style="list-style-type: circle">
            <li>
            <details>
                <summary>Installation process should look like this:</summary>
                <img src="images/wsl-during-download.jpg">
            </details>
            </li>
        </ul>
    <li>Once completed, a new Ubuntu window will open asking for your username</li>
        <ul style="list-style-type: circle">
            <li>
                Username should follow structure like <code>nurikim</code> (full name, no spaces, no capitals)
            </li>
        </ul>
    <li>Then, it asks for your password which for everyone, is <code>ict</code></li>
        <ul style="list-style-type: circle">
            <li>
                <details>
                    <summary><strong>The characters will not show as you type; just press enter after writing <code>ict</code></strong></summary>
                    <img src="images/wsl-account-creation.jpg">
                </details>
            </li>
        </ul>
    <li>
        <details>
            <summary>If installed properly, you should see this line:</summary>
            <ul style="list-style-type: circle">
                <img src="images/wsl-successful-account-creation.jpg">
            </ul>
        </details>
    </li>
</ol>

### ***Using WSL to Download Packages***
Copy and paste this command in WSL and press enter: <br> 
<code>sudo apt update && sudo apt upgrade && sudo apt install nodejs && sudo apt install npm</code> 
<details>
    <summary><strong>Optional</strong>: Reveal to find what each part of the command means.<br></summary>
<ul>
<li><code>&&</code>: After running the command on the left, run the command on the right.</li>

<li><code>apt</code>:
    Calls Advanced Package Tool (APT), a collection of repositories that hold software packages.</li>

<li><code>sudo apt update</code>: 
    Browses through a list of packages on <code>apt</code> and copies the latest version of each package onto the computer.</li>

<li><code>sudo apt upgrade</code>:
    Upgrades all <code>apt</code> packages that are currently stored on the computer.</li>

<li>
<code>sudo apt install nodejs</code>:
    <ul>
        <li>As a superuser (<code>sudo</code>) <code>install</code> <code>nodejs</code> (package name) from a list of packages held by <code>apt</code> </li> 
    </ul>
</li>

<li>Not in the command but useful to know: <code>[package name] -v</code>:
    <ul>
        <li><code>-v</code> asks the computer to display the package's version</li>
        <li>If running the command does not display its version number, it's telling you the package has not been installed yet
    </ul>
</li>
</ul>
</details>
<br>

### ***Installing the WSL VSCode Extension***
Extensions are software add-ons that can be added to your development environment on VSCode. These often enhance your productivity as a developer through added support for programming languages, debuggers, code formatters, 
<br>

## 👩‍💻 **VSCode**
VSCode is an IDE (integrated development environment) application which essentially helps developers edit, run, and commit their code to GitHub. Think of Google Docs but for code.

### ***Correctly Opening VSCode***
We need to open VSCode through the command line so we can implement Git into our project.
<details>
    <summary>What is Git?</summary>
    Git is a piece of open-source software that tracks changes in code files and allows collaboration between developers working on the same project.<br>
    GitHub, as we covered earlier, is designed around Git.
</details>
<ol>
    <li>Open Windows PowerShell normally (do not "Run as administrator")</li>
    <li>
        <details>
            <summary><code>wsl</code></summary>
            Open WSL
        </details>
    </li>
    <li>
        <details>
            <summary><code>cd Desktop</code></summary>
            <ul>
                <li><code>cd</code>: Change directories (go into the specified folder)</li>
                <li><code>Desktop</code>: Change directories into your computer's Desktop to access its files, folders, or apps
            </ul>
        </details>
    </li>
    <li>
        <details>
            <summary><code>ls</code></summary>
            List everything (i.e. files, folders, apps, etc.) that is in your current directory/folder
        </details>
    </li>
    <li>
        <details>
            <summary><code>cd fsd</code></summary>
            Change into/open the <code>fsd</code> folder that is on your Desktop
        </details>
    </li>
    <li>
        <details>
            <summary><code>code [repository/folder name]</code></summary>
            <ul>
                <li><code>code</code>: Open the specified repository/folder on your computer with VSCode</li>
            </ul>
        </details>    
    </li>
</ol>