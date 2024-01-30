# Neo Vim config
---

### dependency packages
- neovim
- vim plug
- clang (in clang users)
- yarn
- nodejs (>= 16.18.0)


### How to config

1. install depandency packages

```
// example in archlinux

// install packages
sudo pacman -S neovim clang yarn

// install vim-plug
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'

```

2. install neovim plugins

```
// open init.vim (~/.config/nvim/init.vim)
nvim init.vim

// install plugin
:w
:so %
:PlugInstall
```

3. coc.nvim config

```
// clang install
:CocInstall coc-clangd
:CocCommand clangd.install

// pyright install
:CocInstall coc-pyright

```
