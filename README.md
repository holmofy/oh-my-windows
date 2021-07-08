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
scoop bucket add jetbrains         # https://github.com/Ash258/Scoop-JetBrains
scoop bucket add nonportable       # https://github.com/TheRandomLabs/scoop-nonportable
scoop bucket add nightlies         # https://github.com/scoopinstaller/nightlies
scoop bucket add nerd-fonts        # https://github.com/matthewjberger/scoop-nerd-fonts
```

**Cli app**
```sh
scoop install unxutils             # GNU utilities for Win32: http://unxutils.sourceforge.net/
scoop install coreutils            # GNU utilities for Windows mingw
scoop install git                  # PortableGit-2.30.1-64-bit.7z.exe
scoop install pasteboard           # https://github.com/uzxmx/pasteboard
scoop install lazygit              # https://github.com/jesseduffield/lazygit
scoop install oh-my-posh3          # https://github.com/jandedobbeleer/oh-my-posh
scoop install posh-git             # https://github.com/dahlbyk/posh-git
scoop install adopt8-hotspot       # adopt-jdk
scoop install tldr                 # Interactive tldr pages
scoop install cht                  # cli cheat sheet
scoop install docker               # Docker容器
scoop install nvm                  # node version manager: https://github.com/coreybutler/nvm-windows
nvm node_mirror <url>              # set node mirror for china
nvm npm_mirror <url>               # set npm-cli mirror for china
nvm install <version>              # nvm install node
nvm use <version>                  # nvm use node
npm install -g nrm                 # npm registry manager
scoop install pyenv                # https://github.com/pyenv-win/pyenv-win
pyenv install <version>            # install python
pip install mycli                  # https://github.com/dbcli/mycli
```

> bash completion: https://github.com/scop/bash-completion

**Gui app**
```sh
scoop install powertoys            # https://github.com/microsoft/PowerToys
scoop install typora               # markdown编辑器
scoop install switchhosts          # https://github.com/oldj/SwitchHosts
scoop install vscode               # https://github.com/Microsoft/vscode
scoop install screentogif          # https://github.com/NickeManarin/ScreenToGif
scoop install quicklook            # https://github.com/QL-Win/QuickLook
scoop install shadowsocks          # https://github.com/shadowsocks/shadowsocks-windows
scoop install v2rayn               # https://github.com/2dust/v2rayN
```

> awesome scoop: https://github.com/tapannallan/awesome-scoop


