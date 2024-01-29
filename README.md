# Easy suckless installation guide for dummies!! Enjoy!!

## Requiremets
- To build dwm you will need the **Xlib** header files.
- You must have  **libxft-bgra** installed until the libxft upstream is fixed (for dmenu)
- you should have **xlib** header files and **libharfbuzz** build files installed. (for st)

```bash
sudo apt install build-essential libx11-dev libxft-dev  libxinerama-dev libfreetype6-dev libfontconfig1-dev libx11-xcb-dev libxcb-res0-dev libharfbuzz-dev
#This is an example for debian builds.
#If you use any other linux distro then use package manager accordingly.(and if you still don't understand then consider chat-gpt your second father because it will tech you alot.)
```
## Installation Steps(follow them in order)

- `mkdir -p /home/$USER/.suckless`
- `cd /home/$USER/.suckless && git clone https://github.com/0xpwnst4r/suckless-for-dummies.git`
- `cd /home/$USER/.suckless/dwm && sudo make clean install`
- `cd /home/$USER/.suckless/dmenu && sudo make clean install`
- `cd /home/$USER/.suckless/st && sudo make clean install`
- `cd /home/$USER/.suckless/pywal && sudo python setup.py install` 
- `sudo apt install xcompmgr`
- `sudo apt install feh`
- `sudo apt install xdotool`
- `cd /home/$USER/.suckless/fonts && sudo mv sudo mv jetBrainsMono JetBrainsMonoNerd fontawesome-free -t /usr/share/fonts/`
- Goto `/usr/share/xsessions/` path location and make a file named `dwm.desktop` and put the below written script in it.
```
[Desktop Entry]
	Encoding=UTF-8
	Name=Dwm
	Comment=Dynamic window manager
	Exec=/home/$USER/.suckless/autostart
	Icon=dwm
	Type=XSession

```
- Restart your system and select `dwm` instead of your current desktop environment or window manager on login page.
- And you aree goooodddd toooo gooooo.......GG!!
