# Setting up DWM on a Raspberry Pi running Raspbian lite

Make sure git is intalled

```
sudo apt install git
```

Clone the repository from suckless:

```
git clone https://git.suckless.org/dwm
```

Install the required dependencies

```
sudo apt install libx11-dev libxft-dev libxinerama-dev
```

Build and install dwm

```
cd dwm && sudo make clean install
```

Install xinit

```
sudo apt install xinit
```

Confiure `/etc/X11/xinit/xinitrc`

```sh
#!/bin/sh

# /etc/X11/xinit/xinitrc
#
# global xinitrc file, used by all X sessions started by xinit (startx)

# invoke global X session script
# /etc/X11/Xsession

exec dwm
```

Enter the desktop environment:

```
startx
```