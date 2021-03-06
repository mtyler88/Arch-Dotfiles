# Arch-Dotfiles
## Needed programs
tmux
vim
zsh
the-silver-searcher
ripgrep
fd-rs
xmonad
xmobar
tmuxp
nm-applet
insync
pasystray
gpmdp
pavucontrol
google chrome
rofi
rxvt-patched-unicode
scrot
haskell-hostname
-- For scrot, make sure the folder ~/pictures/screenshots exists
compton
light-locker
fzf
xinit-xsession -- To run the ~/.xinitrc file as a session (for xmonad)

## Terminal
using urxvt as the terminal (install rxvt-unicode-patched from the aur)

## Setting up vim
Using plug, install with:
```sh
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
Once installed, and using the .vimrc install the plugins with ":PlugInstall"

Need to compile youcompleteme
Go into the folder plug downloaded it and run 
```sh
./install.py --clang-completer --system-libclang
```

## Xmonad
Install xmonad and xmobar
Use this guide: http://brianbuccola.com/how-to-install-xmonad-and-xmobar-via-stack/

and add this into /usr/share/xsessions/xmonad.desktop:
[Desktop Entry]
Encoding=UTF-8
Type=Application
Name=Xmonad
Comment=Lightweight X11 tiled window manager written in Haskell
Exec=xmonad
Icon=xmonad
Terminal=false
StartupNotify=false
Categories=Application

## tmuxp
Install tmuxp to help with managing sessions in tmux

## Oh My ZSH
using oh my zsh, install from the git rather than aur
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
## Installing rust
Run: $ curl https://sh.rustup.rs -sSf | sh

