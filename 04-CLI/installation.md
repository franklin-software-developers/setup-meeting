# ＞ Command Line Interface (CLI)
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

<strong>Using the CLI increases our productivity as developers.</strong>

## WSL
WSL is a CLI app offered by Microsoft that allows you to run Linux commands on a Windows computer.
<details>
    <summary>What is Linux?</summary>
    Windows and MacOS are both operating systems, the essential software that manages the computer's software and hardware. Like Windows and MacOS, Linux is another operating system (OS). However, Linux is an open-source OS, meaning its users can freely access, redistribute and modify it, a huge reason it rose in popularity.
</details>

### Downloading WSL
<ol>
    <li>
        <details>
            <summary>"Run [Windows PowerShell] as Administrator"</summary>
            <img src="">
        </details>
    </li>
    <li>Once open type this command: <br><code>wsl --install -d Ubuntu</code></li>
    <li>Wait through installation:</li>
        <ul style="list-style-type: circle">
            <li>
            <details>
                <summary>Installation process should look like this:</summary>
                <img src="">
            </details>
            </li>
        </ul>
    <li>Once completed, a new Ubuntu window will open asking for your username</li>
        <ul style="list-style-type: circle">
            <li>
                <details>
                    <summary>Username should follow structure like <code>nurikim</code>:</summary>
                    <img src="">
                </details>
            </li>
        </ul>
    <li>Then, it asks for your password which for everyone, is <code>ict</code></li>
        <ul style="list-style-type: circle">
            <li>
                <details>
                    <summary><strong>The characters will not show as you type; just press enter after writing <code>ict</code></strong></summary>
                    <img src="">
                </details>
            </li>
        </ul>
    <li>If installed properly, you should see this line:</li>
        <ul style="list-style-type: circle">
            <img src="">
        </ul>
</ol>

### Using WSL to Download Packages
Copy and paste this command in WSL to run it: <br> 
<code>sudo apt update && sudo apt upgrade && nodejs -v && sudo apt install nodejs && sudo apt install npm</code> 
<br><br>
Optional: Read on to find what each part of the command means.<br>

<code>&&</code>:
    After running the command on the left, run the command on the right.

<code>sudo apt update</code>: 
    Browses through a list of packages on <code>apt</code> and copies the latest version of each package onto the computer.

<code>sudo apt upgrade</code>:
    Upgrades all <code>apt</code> packages that are currently stored on the computer.

<code>nodejs -v</code>:
    <ul>
        <li><code>nodejs</code> is the package name <br></li>
        <li><code>-v</code> asks the computer to display the package's (<code>node</code>) version</li>
        <li>If running the command does not display its version number, it's telling you the package has not been installed yet
    </ul>

<code>sudo apt install nodejs</code>:
    <ul>
        <li>As a superuser (<code>sudo</code>) <code>install</code> <code>nodejs</code> (package name) from a list of packages on <code>apt</code> </li> 
    </ul>
