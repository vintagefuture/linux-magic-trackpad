# linux-magic-trackpad

Easiest way to have multi-gestures on linux using Apple Magic Trackpad

```
sudo pacman -S wmctrl xdotool
yay -S libinput-gestures
sudo gpasswd -a $USER input
```
Reboot, then:
```
libinput-gestures-setup autostart start
cp /etc/libinput-gestures.conf ~/.config/libinput-gestures.conf
```
Edit `~/.config/libinput-gestures.conf` as you please.

Reload the application to apply the changes:
```
libinput-gestures-setup restart
```
