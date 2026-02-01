# Terminal Configuration 
I have so many devices going on right now

## Useful links
[Kitty Terminal Docs](https://sw.kovidgoyal.net/kitty/)

[Lazyvim Docs](https://www.lazyvim.org/)

## Things to Install
These are all available on arch package manager via pacman (most available via mac homebrew as well but i have yet to try them all as i am forced to, not glad to, use macos on the work laptop i port this config to)

first, install these (python-pynvim is optional but useful later): 
`sudo pacman -S kitty neovim fastfetch pokemon-colorscripts python-pynvim`

clipboard util if you are a linux user who needs it because you learned linux on a manual arch install and are stuck like this now, which is likely because this repo is just for me (wl-clipboard is for wayland but xclip is fine on x11): 
`sudo pacman -S w-clipboard xdg-utils mailcap`

then install the [lazyvim starter](https://www.lazyvim.org/installation)

note: there are a couple fastfetch configs i've gone through but i believe the pokemon is non-negotiable. we need whimsy in 2026
