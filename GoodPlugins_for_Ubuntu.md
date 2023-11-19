## HOW TO USE GOOD PLUGINS FOR Ubuntu

> ### Install Zsh 
* ```sudo apt install zsh```
* ```sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

### Install Zsh Theme - "powerlevel10k"
* install fonts : https://github.com/romkatv/powerlevel10k#fonts
* ```git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k```
* ```vi ~/.zshrc``` -> ```ZSH_THEME="powerlevel10k/powerlevel10k"```

### Install Zsh Plugins
* auto suggestions
    * ```git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions```
* syntax highlighting
    * ```git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting```

* ```vi ~/.zshrc``` -> add ```zsh-autosuggestions``` & ```zsh-syntax-highlighting```

### Install Lunarvim
* install neovim
    * ```curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage```
    * ```chmod u+x nvim.appimage```
    * ```./nvim.appimage --appimage-extract```
    * ```sudo mv squashfs-root /```
    * ```sudo ln -s /squashfs-root/AppRun /usr/bin/nvim```

* install Lunarvim
    * ```sudo apt install python3-pip python3-dev```
    * ```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```
    * ```LV_BRANCH='release-1.3/neovim-0.9' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh)```
    * When installation is completed successfully, they will say "Thank you for installing lunarvim~"
    * ```~/.zshrc``` -> add ```echo 'export PATH=$PATH:/home/chaeeon/.local/bin'```

    
