# oh-my-windows

Windows Developer

## 1. Windows Package Manager

* [microsoft/WinGetCli](https://github.com/microsoft/winget-cli)  ![](https://img.shields.io/github/stars/microsoft/winget-cli)

* [Choco](https://github.com/chocolatey/choco)  ![](https://img.shields.io/github/stars/chocolatey/choco)

* [Scoop](https://github.com/lukesampson/scoop)  ![](https://img.shields.io/github/stars/lukesampson/scoop)

推荐用scoop

```sh
# Configure Scoop to install global programs to a Custom Directory by changing SCOOP_GLOBAL
$env:SCOOP_GLOBAL='F:\GlobalScoopApps'
[Environment]::SetEnvironmentVariable('SCOOP_GLOBAL', $env:SCOOP_GLOBAL, 'Machine')

# run the installer
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
# or shorter
iwr -useb get.scoop.sh | iex
```

## 2. Terminal

 * [microsoft/terminal](https://github.com/microsoft/terminal)  ![](https://img.shields.io/github/stars/microsoft/terminal)
 
 * [alacritty](https://github.com/alacritty/alacritty)  ![](https://img.shields.io/github/stars/alacritty/alacritty)
 
 * [cmder](https://github.com/cmderdev/cmder) ![](https://img.shields.io/github/stars/cmderdev/cmder)

 * [terminus](https://github.com/Eugeny/terminus) ![](https://img.shields.io/github/stars/Eugeny/terminus)
 
 * [FluentTerminal](https://github.com/felixse/FluentTerminal) ![](https://img.shields.io/github/stars/felixse/FluentTerminal)
 
 > https://github.com/Awesome-Windows/Awesome#terminal
 
 推荐microsoft/terminal
 
 ```sh
scoop bucket add extras
scoop install windows-terminal
 ```
 
## 3. App

```sh
scoop install git                  # PortableGit-2.30.1-64-bit.7z.exe
scoop bucket add extras            # https://github.com/lukesampson/scoop-extras
scoop install typora               # markdown编辑器
...
```
