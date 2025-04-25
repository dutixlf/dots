# There is mine compact dotfiles
guys, there is MINE dotfiles. DO NOT MAKE PR, PLEASE.

## installation
I'll create **install.sh** soon. maybe tomorrow? next week? in month? idk =)

### please install:
* hyprland
* fish
* kitty
* waybar
* albert launcher


### Extracting

**so, start with**
```bash
$ cp .config /home/$USER/.config/
```

**link default waybar path to *.config***
```bash
$ rm -r /etc/xdg/waybar/* # if waybar was started once
$ ln -s /home/$USER/.config/waybar/ /etc/xdg/waybar/
```

**copy albert launcher config to albert's themes destination**
```bash
$ cp albert.ini /usr/share/albert/widgetsboxmodel-ng/themes/Black\ And\ White.ini
```

**now you need to change some example configs for hyprland**
```bash
$ ls
appearance.conf   hyprland.conf           keybinds.conf          windowrules.conf
autostart.conf    hyprpaper.example.conf  monitors.example.conf
environment.conf  input.conf              programs.conf

$ nano hyprpaper.example.conf monitors.example.conf
```

### Now relog

*note: if u have fucking shit like*
```bash
Welcome to fish, the friendly interactive shell
Type help for instructions on how to use fish
⋊> ~
```

*just type*
```bash
$ set -U fish_greeting
```
