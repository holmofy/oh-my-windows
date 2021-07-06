# oh-my-windows

vim, tmux, zsh refer to [oh-my-mac](https://github.com/holmofy/oh-my-mac)

Windows Developer

## 1. Windows Package Manager

* [microsoft/WinGetCli](https://github.com/microsoft/winget-cli)  ![](https://img.shields.io/github/stars/microsoft/winget-cli)

* [Choco](https://github.com/chocolatey/choco)  ![](https://img.shields.io/github/stars/chocolatey/choco)

* [Scoop](https://github.com/lukesampson/scoop)  ![](https://img.shields.io/github/stars/lukesampson/scoop)

推荐用scoop或choco

### install scoop
```sh
# Configure Scoop to install global programs to a Custom Directory by changing SCOOP_GLOBAL
$env:SCOOP_GLOBAL='F:\GlobalScoopApps'
[Environment]::SetEnvironmentVariable('SCOOP_GLOBAL', $env:SCOOP_GLOBAL, 'Machine')

# run the installer
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
# or shorter
iwr -useb get.scoop.sh | iex
```

> 安装完成后如果出现命令找不到，先检查一下环境变量是否加到Path中。
> 如果用scoop安装软件找不到，可以`scoop update`一下

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

> 将git bash添加到windows-terminal中：https://stackoverflow.com/questions/56839307/adding-git-bash-to-the-new-windows-terminal
 
## 3. App

**app bucket**

```sh
scoop bucket add extras            # https://github.com/lukesampson/scoop-extras
scoop bucket add versions          # https://github.com/scoopinstaller/versions
scoop bucket add java              # https://github.com/scoopinstaller/Java
scoop bucket add nerd-fonts        # https://github.com/matthewjberger/scoop-nerd-fonts
scoop bucket add jetbrains         # https://github.com/Ash258/Scoop-JetBrains
scoop bucket add nonportable       # https://github.com/TheRandomLabs/scoop-nonportable
scoop bucket add nightlies         # https://github.com/scoopinstaller/nightlies
```

**Recommended app**
```sh
scoop install git                  # PortableGit-2.30.1-64-bit.7z.exe
scoop install powertoys            # https://github.com/microsoft/PowerToys
scoop install typora               # markdown编辑器
scoop install adopt8-hotspot       # adopt-jdk
scoop install lazygit              # https://github.com/jesseduffield/lazygit
scoop install oh-my-posh3          # https://github.com/jandedobbeleer/oh-my-posh
```

> awesome scoop: https://github.com/tapannallan/awesome-scoop

https://github.com/NickeManarin/ScreenToGif

https://github.com/QL-Win/QuickLook
