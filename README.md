My Finale dwm/suckless build enjoy!

To use,
first clone the repo
```
git clone https://github.com/IBM-5100-PC/suckless.git 
```
then cd to suckless directory
```
cd suckless
```
cd to what program to compile e.g. :dwm
```
cd dwm
```
then compile it!
```
sudo make clean install
 ```
create/edit ```~/.dwm/autostart.sh```
```
slstatus & #status bar
picom & # compositor
nitrogen --restore # wallpaper
```
edit ```~/.xinitrc``` and add
```
exec /usr/local/bin/dwm
```
and if you are not using an login manager you can add this to your ```~/.profile``` in bash or ```~/.zshrc``` in zsh.
```
if [[ -z "$DISPLAY" ]] && [[ $(tty) = /dev/tty1 ]]; then
. startx
logout
fi
```
