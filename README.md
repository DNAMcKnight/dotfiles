## Note: to make this work you first need to copy the dotfiles to `home/mcknight/`

# Step 1 
## install zsh antigen


`yay -S zsh antigen`

# Step 2

## Fonts 
### Download the fonts from here and copy all the fonts (excluding MACOS!) to `/home/mcknight/.local/share/fonts/`

`https://github.com/gaplo917/Ligatured-Hack/releases/`

# Step 3
## Antigen
### Create a folder called `dotfiles` and create a file called `.antigenrc` add the following lines to that file

```
source /usr/share/zsh/share/antigen.zsh

# Load the oh-my-zsh's library
antigen use oh-my-zsh

antigen bundle ohmyzsh/ohmyzsh
antigen bundle git
antigen bundle zsh-users/zsh-autosuggestions
antigen bundle zsh-users/zsh-completions
antigen bundle zsh-users/zsh-syntax-highlighting
antigen bundle docker
antigen bundle docker-compose

# Load the theme
antigen theme romkatv/powerlevel10k

# Tell antigen that you're done
antigen apply`

```

# Step 4
## Load Antigen
### Edit your `.zshrc` file to load antigen, add the following line at the end of the file

`source ~/.antigenrc`

# Step 5
## Shell
### set zsh as the main shell

`chsh -s $(which zsh)`

# Step 6
## Zsh Setup/Settings
### Relog or reboot for the last command to take effect, or just type zsh and go through the setting process, if you want to change the settings it's all saved in the `.zshrc` file.


# Setp 7
## Theme Settings
### To change theme settings run this command

`pk10 configure`
