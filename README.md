# First minute Arch Linux guide

## Frome Repousey

### Extra

#### CLI

- pcurses
- ranger
- links
- neomutt
- rtorrent
- transmission-cli
- nmap
- gist
- rsync
- sonic-visualiser
- mps-youtube
- cmus
- feh

#### GUI

>installed
- transmission-qt
- screenfetch
- obs-studio
- geary
- mpv
- dolphin-plugins
- kdegraphics-thumbnailers
- kimageformats
- kdesdk-thumbnailers
- ffmpegthumbs
- raw-thumbnailer
- taglib
- rofi

> AUR
- kde-thumbnailer-apk
- kde-thumbnailer-blender
- kde-thumbnailer-epub

>optional

- qutebrowser
- kdenlive
- rclone
- streamlink
- rawtherapee
- darktable
- digikam
- krita
- ardour
- lmms
- tilda
- wine
- wine-gaming-nine
- flatpak
- kmousetool
- minuet
- kdegames
- nomacs (good alternative for qimgv with more func)

### AUR

#### AUR CLI

- alpine
- telegram-cli-git
- whistle-git
- herrie
- qimgv-git(irfanviewer like)
- vtop

#### AUR GUI

>installed AUR
- firefox-developer-edition-i18n-en-us
- visual-studio-code-bin
- blender-git
- abricotine
- typora
- onedrive-git (CLI)
- inkscape-git

>install AUR
- vim
- vim-plugins
- pkgbrowser
- dropbox
- grub-customizer

>opt
- discord
- skypeforlinux-stable-bin
- slack-desktop
- activitywatch-bin
- google-chrome
- vivaldi
- yandex-disk
- telegram-desktop-bin
- vocal
- teamviewer
- evince-no-gnome
- shufti
- mockingbot
- yed
- kaku-bin
- bitwig-studio
- plasma5-applets-kde-arch-update-notifier-git
- cpu-x-git

#### check

    sup(блядовые рубя ирорят)
    yandex-disk-indicator (погодить)
    fbv fim jfbview fbida(too old way)
    **tomahawk**
    Alacritty
    KBackup

## links

[Package Search](https://www.archlinux.org/packages/?sort=&arch=x86_64&q=obs-studio&maintainer=&flagged=)

[forum](https://forum.archlabslinux.com/)

[General recommendations](https://wiki.archlinux.org/index.php/general_recommendations)

[Core utilities](https://wiki.archlinux.org/index.php/Core_utilities)

[List of applications](https://wiki.archlinux.org/index.php/List_of_applications/Multimedia#GUI_players)

[UE4](https://github.com/Allar/ue4-mp-downloader)

## Shell

### no choise

>https://www.youtube.com/watch?v=0NOAUogSSMo

    https://github.com/fish-shell/fish-shell
>aur `fish-git`

### alias

    ~/.bashrc
    alias alias_name="command_to_run"

- alias pac="sudo pacman -S --needed --noconfirm"
- alias aur="aurman -S --needed --noconfirm"
- alias sauron="aurman -S --force --noconfirm --noedit --pgp_fetch --deep_search"
- alias upd='sudo pacman -Syu'

> To remove a package and its dependencies which are not required by any other installed package:

pacman -Rs *package_name*

> Pacman can update all packages on the system with just one command:

pacman -Syu

### sudo

~$ sudo EDITOR=nano visudo
~$ sudo EDITOR=vim visudo

~$ sudo vim visudo

- root    ALL=(ALL) ALL
>uncommen wheel group
- Defaults:USER_NAME      !authenticate
- USER_NAME ALL=NOPASSWD: /bin/mount, /bin/umount

>to get accese
sudo chmod -R a+rwx /usr

### Ligatures

    https://github.com/tonsky/FiraCode
    https://larsenwork.com/monoid/
    https://be5invis.github.io/Iosevka/

## soft

### vim

[oceanic-next](https://github.com/mhartington/oceanic-next)

[onedark](https://github.com/joshdick/onedark.vim)

### qtile

- https://www.one-tab.com/page/MU0WW2juTt2zUTvnNd17OA
- https://krusader.org/
- http://sunflower-fm.org/
- https://inigo.katxi.org/devel/lfm/

#### keys

- Telegram  /Telegram -startintray
- Steam  /usr/bin/steam %U -silent
- Transmission /usr/bin/transmission-gtk --minimized

## settings

### github

    https://help.github.com/articles/set-up-git/

    git config --global user.name "NAME"
    git config --global user.email "EMAIL"
    ssh-keygen -t rsa -b 4096 -C "EMAIL"

`pac xclip`

Copies the contents of the id_rsa.pub file to your clipboard
`xclip -sel clip < ~/.ssh/id_rsa.pub`

### DPI

bc

>1920/(47.7/2.54)
>
>106
>
>1080/(26.8/2.54)
>
>108


> Note: While you can set any dpi you like and applications using Qt and GTK will scale accordingly, it's recommended to set it to 96, 120 (25% higher), 144 (50% higher), 168 (75% higher), 192 (100% higher) etc., to reduce scaling artifacts to GUI that use bitmaps. Reducing it below 96 dpi may not reduce size of graphical elements of GUI as typically the lowest dpi the icons are made for is 96.
`
> For RandR compliant drivers (for example the open source ATI driver), you can set it by:

~$ xrandr --dpi 144

> Note: Applications that comply with the setting will not change immediately. You have to start them anew.

## wm

### Introduction

    bspwm
    budgie
    cinnamon
    deepin
    fluxbox
    openbox
    i3
    lxde
    mate
    netbook
    pantheon

### Wayland

[Wayland](https://wiki.archlinux.org/index.php/Wayland)

#### Sway

[Sway](https://wiki.archlinux.org/index.php/Sway)

xprop

#### AUR Wayland

- [firefox-wayland](https://aur.archlinux.org/pkgbase/firefox-wayland/)
- [firefox-wayland-hg](https://aur.archlinux.org/pkgbase/firefox-wayland-hg/)
