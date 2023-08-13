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

# vim config
```
set nu
syntax on "语法高亮
set encoding=utf-8

set autoindent "自动缩进
set cindent
set smartindent "为c语言提供自动缩进

set tabstop=4
set softtabstop=4
set shiftwidth=4

set laststatus=0

"set mouse=a
"set clipboard+=unnamed

noremap <Up> <NOP>
noremap <Down> <NOP>
noremap <Left> <NOP>
noremap <Right> <NOP>

imap jj <ESC>

let mapleader="," "默认是\
```
# nerdtree
```
Plug 'preservim/nerdtree'

nnoremap <leader>n :NERDTreeFocus<CR>
nnoremap <C-n> :NERDTree<CR>
nnoremap <C-t> :NERDTreeToggle<CR>
nnoremap <C-f> :NERDTreeFind<CR>
```

# Install coc.nvim
```
brew install node
Plug 'neoclide/coc.nvim'

npm install -g yarn
cd ~/.local/share/nvim/plugged/coc.nvim
yarn install && yarn build

:CocInstall coc-json coc-tsserver
:CocInstall coc-sourcekit
:CocInstall coc-clangd
:CocList extensions
"哎呀呀，鸡儿烦😡
```


