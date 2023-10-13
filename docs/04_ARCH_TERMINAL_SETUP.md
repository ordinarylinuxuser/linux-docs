# Installation of Hardware Drivers for Arch Linux Gnome

## Prerequisites

1. You have the [Base Installation](01_ARCH_INSTALL_BASE.md) done.

## Installation Steps

   - Install Alacritty
  
        ```sh
        sudo pacman -S alacritty
        ```
   - Install zsh & zsh-completion
        ```sh
        sudo pacman -S zsh zsh-completions ttf-hack-nerd bat fd exa tree
        ```
   - Install oh-my-zsh
        ```sh
        sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

        #syntax highlighting
        git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

        #auto suggestion
        git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
        ```
   - Install fzf
        ```sh
        git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
        ~/.fzf/install
        ```