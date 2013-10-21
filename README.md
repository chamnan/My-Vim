This is my VIM configuration for Ubuntu

Installation/Configuring
------------------------

paste the following into the Terminal.

```
git clone https://github.com/chamnan/My-Vim ~/.vim
ln -s ~/.vim/vimrc ~/.vimrc
```
- Font Installation:
	- Font Config:

```
wget https://github.com/Lokaltog/powerline/raw/develop/font/PowerlineSymbols.otf 
wget https://github.com/Lokaltog/powerline/raw/develop/font/10-powerline-symbols.conf
mkdir -p ~/.fonts/ && mv PowerlineSymbols.otf ~/.fonts/
fc-cache -vf ~/.fonts
mkdir -p ~/.config/fontconfig/conf.d/
mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
```
- Font patching:
	1. Download the font of your choice from [powerline-fonts](https://github.com/Lokaltog/powerline-fonts).
	2. Move your patched font to `~/.fonts/`
	3. Run `fc-cache -vf ~/.fonts` to update your font cache

	For more info about Powerline [Font patching](https://powerline.readthedocs.org/en/latest/fontpatching.html)
