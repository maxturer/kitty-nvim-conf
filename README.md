# Terminal Configuration 
I have so many devices going on right now

## Useful links
[Kitty Terminal Docs](https://sw.kovidgoyal.net/kitty/)

[Lazyvim Docs](https://www.lazyvim.org/)

## Things to Install
Kitty terminal, readability utilities ([lsd](https://github.com/lsd-rs/lsd) and [fzf](https://github.com/junegunn/fzf)), neovim, fastfetch. These are all available on arch package manager via pacman (most available via mac homebrew as well but i have yet to try them all as i am forced to, not glad to, use macos on the work laptop i port this config to)

first, install these (python-pynvim is optional but useful later): 
```
sudo pacman -S kitty neovim fastfetch lsd fzf pokemon-colorscripts python-pynvim
```

Iosevka font is available via pacman install as `ttf-iosevka-term-slab` or nerd font `ttf-iosevkatermslab-nerd`. homebrew has `font-iosevka-slab` and `font-iosevka-term-slab-nerd-font`. if going with nerd font change font family in kitty.conf to 'IosevkaTermSlab NerdFont'. if you don't know what that is or care ignore that part completely

clipboard util if you are a linux user who needs it because you learned linux on a manual arch install and are stuck like this now, which is likely because this repo is just for me (wl-clipboard is for wayland but xclip is fine on x11): 
```
sudo pacman -S w-clipboard xdg-utils mailcap
```
then install [oh-my-zsh](https://ohmyz.sh/#install) and the modified the [lazyvim starter](https://www.lazyvim.org/installation)
### zshrc plugins etc
agnosterzak theme! essential for visually-oriented people who live on the terminal!
it's in here as `agnosterzak.zsh-theme` or [on github](https://raw.githubusercontent.com/zakaziko99/agnosterzak-ohmyzsh-theme/master/agnosterzak.zsh-theme). if using my file from here just move her: `cp agnosterzak.zsh-theme ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes`

install zsh-autosuggestions and zsh-syntax-highlighting. sounds unimportant but surprisingly not
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

if not using arch, the `.zshrc` file here has `archlinux` plugin, so remove line 7. on work laptop i changed this line to `macos`. there are more plugins on [the ohmyzsh wiki](https://github.com/ohmyzsh/ohmyzsh/wiki/plugins), still determining how useful they all are~

## Important post-installation notes
on fastfetch: there are a couple fastfetch configs i've gone through but i believe the pokemon is non-negotiable

please enjoy running `kitten themes`. if you are using this with my [terminal music player](https://github.com/maxturer/mpd-rmpc-config), it's set up for mona lisa theme, but making it adaptive to any theme is coming soon (please look forward to it)
