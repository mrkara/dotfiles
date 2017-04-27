
# Dotfiles

Some of my configuration files and resources I use everyday. I do my best to keep them readable and useful to everyone.

### vimrc
![Screenshot](screenshots/vim1.png?raw=true "Screenshot")

Cherry-picked plugins, bunch of customizations and (hopefully) not-too-invasive keybindings. Make sure you've read it first before applying.

**Depends:** vim (>=8) (+python), vimplug, exuberant-ctags, silversearcher-ag (>= 0.29.1)

##### How to setup
* apt-get install powerline 
* apt-get install silversearcher-ag
* sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)" 
* git clone https://github.com/junegunn/fzf.git $ZSH_CUSTOM/plugins/fzf 
* $ZSH_CUSTOM/plugins/fzf/install --bin 
* git clone https://github.com/Treri/fzf-zsh.git $ZSH_CUSTOM/plugins/fzf-zsh 
* git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions

After running those, get "fasd" from: https://github.com/clvv/fasd and simply run "make install".

**Depends:** oh-my-zsh, powerline, fasd, fzf, fzf-zsh, silversearcher-ag, zsh-autosuggestions

### bashrc

Nothing really fancy. Just sane defaults, Powerline and Fasd integration.
To make powerline and fasd play nice together, I've made a small change, simply run:
> cp powerline.sh /usr/share/powerline/bindings/bash/powerline.sh

**Depends:** powerline, fasd
