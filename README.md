# vim_config

```
brew install neovim
```

# zshrc
```
vim .zprofile
alias vim="nvim"
```

# install vim-plug
```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

```
mkdir -p .config/nvim
vim .config/nvim/init.vim
```

```
call plug#begin()                                                     
Plug 'morhetz/gruvbox'                                                     
call plug#end() 

:PlugInstall
```
