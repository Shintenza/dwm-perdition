# DWM-PERDITION

[Preview](./preview.png)

Dwm is an extremely fast, small, and dynamic window manager for X. Dwm is created by the suckless guys.  This is my personal build of dwm.  I applied a number of patches to make dwm more "reliable" rather than "suckless". 

## Patches used in this build:
- alwayscenter (makes centered dialog boxes)
- attachaside (new windows appears in the stack rather than as the master)
- autostart (looks for autostart.sh in ~/.dwm and runs that script after startup)
- colorbar (gives you more options when it comes to the bar's color settings)
- cyclelayoyts (gives you a keybinding to cycle through the avaliable layouts)
- restartsig (ability to restart dwm without killing it)
- rotatestack (moves the window through the stack)
- swallow ([check here](https://www.youtube.com/watch?v=92uo5OBOKfY))
- systray (displays systray)
- vaniygaps (this patch applies gapps but also a number of layouts)

## Dependencies:

Here is the list of dependencies that you should consider installing.
- [Iosevka NF](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Iosevka.zip)
- [dmenu](https://tools.suckless.org/dmenu/)
- [libxft](https://aur.archlinux.org/packages/libxft-bgra/)

## Running dwm:

If you use a login manager (such as lightdm or sddm) you have to create a file called `dwm.desktop` in `usr/share/xsessions` directory. It should looke like this:
	[Desktop Entry]
	Encoding=UTF-8
	Name=Dwm
	Comment=Dynamic window manager
	Exec=dwm
	Icon=dwm
	Type=XSession

