# Instruction Install My Best Terminal

The operating system I use is Ubuntu 20.04.1 LTS

List of this readme:
- [Install zsh](#install-zsh)
- [Install kitty](#install-kitty)
- [Install powerlevel10k](#install-powerlevel10k)

## Install zsh[^zsh]
[^zsh]: Zsh, also known as the Z shell, extends functionality of the Bourne Shell (sh), offering newer features and more support for plugins and themes
1. Type in your terminal `sudo apt install zsh`
2. Then type `chsh -s $(which zsh)` or `chsh -s /usr/bin/zsh` to change the default shell to zsh
3. Then input your password
4. Type `zsh --version` to check if zsh is installed
5. Restart your terminal
6. You will see the setup of zsh like this
![zsh](https://www.tecmint.com/wp-content/uploads/2020/10/New-User-Zsh-Setup.png)
If you want to exit choose `0` or if you want to change the default shell choose `1` and you will see the setup of zsh like this.
![zsh](https://www.tecmint.com/wp-content/uploads/2020/10/Zsh-Main-Menu.png)
If you want to see more, click [this](https://www.tecmint.com/install-zsh-in-ubuntu/)
7. Check your terminal with `echo $SHELL` and you will see `/usr/bin/zsh` or title of your terminal will be `zsh` like this ![zsh](https://cdn.statically.io/img/i.ibb.co/Pwc57Y8/2023-02-05-09-43.png)
8. Finally its done! :tada:

## Install kitty[^kitty]
[^kitty]: [kitty](https://sw.kovidgoyal.net/kitty/) is a fast, feature full, GPU based terminal emulator
1. Type in your terminal `curl -L https://sw.kovidgoyal.net/kitty/installer.sh | sh /dev/stdin`
2. Create symbolic links to add kitty and kitten to PATH (assuming ~/.local/bin is in your system-wide PATH[^system-wide-PATH]).
type `ln -sf ~/.local/kitty.app/bin/kitty ~/.local/kitty.app/bin/kitten /usr/local/bin/`
[^system-wide-PATH]: The (default) system wide `PATH` is set in the `/etc/environment` file. If you want to check your system-wide PATH type `cat /etc/environment` in your terminal. Then you will see something like this `PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games"`
3. Place the kitty.desktop file somewhere it can be found by the OS
type `cp ~/.local/kitty.app/share/applications/kitty.desktop /usr/share/applications/`
4. Check your application launcher to see if kitty is listed, and its done! :tada:

## Install powerlevel10k[^powerlevel10k]
[^powerlevel10k]: To see complete installation and instruction click [this](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)
1. Download font MesloLGS NF from [here](https://github.com/romkatv/powerlevel10k#fonts)
2. Extract the downloaded file and install the font
3. Install powerlevel10k by typing `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k` and `echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc` like [this](https://github.com/romkatv/powerlevel10k#manual)
4. Restart your terminal
5. You will see setup of powerlevel10k like this ![powerlevel10k](https://cdn.statically.io/img/i.ibb.co/Jq7nFdQ/2023-02-05-09-21.png)
Follow the instruction until finish setup
6. Finally its done! :tada: