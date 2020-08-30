# INSTALL
## Install Openbox and Feh
> sudo apt install openbox obconf feh

And then login to openbox wm, right click and type on terminal
> xrandr -s 1920x1080 # set resolution <br>
> mkdir ~/Pictures/wallpaper # make diretory for wallpaper <br>
> feh --bg-scale ~/Pictures/wallpaper/<nameofpicture> # put your wallpaper inside wallpaper folder and select one <br>
> cd ~/.config <br>
> mkdir openbox # make openbox config folder <br>
> cd openbox <br>
> nano autostart # create autostart when you login to openbox

Add the following code
> xrandr -s 1920x1080 <br>
> sh ~/.fehbg &

save, and type on terminal
> openbox --reconfigure

## Install polybar
>sudo apt-get install cmake cmake-data libcairo2-dev libxcb1-dev libxcb-ewmh-dev \
  libxcb-icccm4-dev libxcb-image0-dev libxcb-randr0-dev \
  libxcb-util0-dev libxcb-xkb-dev pkg-config python3-xcbgen \
  xcb-proto libxcb-xrm-dev i3-wm libasound2-dev libmpdclient-dev \
  libiw-dev libcurl4-openssl-dev libpulse-dev \
  libxcb-composite0-dev xcb libxcb-ewmh2 <br>
> git clone https://github.com/jaagr/polybar.git
> cd polybar
> git checkout 3.4.1
> ./build.sh

Use GCC even if Clang is installed ----------------------------- [y/N]: n <br>
Include support for "internal/i3" (requires i3) ---------------- [y/N]: y <br>
Include support for "internal/alsa" (requires alsalib) --------- [y/N]: y <br>
Include support for "internal/pulseaudio" (requires libpulse) -- [y/N]: y <br>
Include support for "internal/network" (requires libnl/libiw) -- [y/N]: y <br>
Include support for "internal/mpd" (requires libmpdclient) ----- [y/N]: y <br>
Include support for "internal/github" (requires libcurl) ------- [y/N]: y <br>
Build "polybar-msg" used to send ipc messages ------------------ [y/N]: y <br>

Done, you can explore polybar, config file is in .config/polybar/config <br>
To start polybar at first time use in terminal : polybar example <br>
If you want to create change on polybar while running use : polybar example -r

## Install rofi menu and kitty terminal
> sudo apt-get install rofi kitty

and done

## Configuration

You can copy all of my config folder to yours <br>
For xrandr it depends on your screen, mine 1920  x 1080 <br>
Openbox use autostart file to start any program on first log <br>
Menu.xml is for keybinding config file and menu.xml is for Right Click Menu on desktop <br>
Config it to being versatile on you <br>
All of the config file is in .config directory <br> <br>
