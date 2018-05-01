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
- qimgv(irfanviewer like)
- vtop
community/hub 2.2.9-2
    cli interface for Github
Список установленных пакетов  pacman -Qe
#### AUR GUI

>installed AUR
- firefox-developer-edition-i18n-en-us
- visual-studio-code-bin

- abricotine
- typora
- onedrive-git (CLI)
- inkscape-git

>install AUR
- vim

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


Defaults:chibo      !authenticate
chibo ALL=NOPASSWD: /bin/mount, /bin/umount


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

`pac openssh xclip`

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



# linux notepad
## pac is default
Spectacle

sudo pip install --upgrade pip
pip install numpy




plasma5-applets-kde-arch-update-notifier-git


unrar

locale
locale-gen



It's enough if you add it to your ~/.bashrc:

export LANG=en_US.UTF-8
export LC_MESSAGES="C"

and reboot.


aur glxgears


sudo chmod -R a+rwx /usr

chmod -R o-rx /usr
chown root:root /usr
chmod 4755 /usr









https://wiki.archlinux.org/index.php/ATI
pac partitionmanager xdotool

file:///run/media/manjaro/bc4f3eff-f979-4323-8a26-5bf84943ec2c/etc/pacman.conf
[multilib]
Include = /etc/pacman.d/mirrorlist


/etc/makepkg.conf
MAKEFLAGS="-j$(nproc)"


file:///run/media/manjaro/bc4f3eff-f979-4323-8a26-5bf84943ec2c/etc/locale.conf
LANG=en_US.UTF-8
LC_COLLATE=C
LC_MESSAGES=C


file:///run/media/manjaro/bc4f3eff-f979-4323-8a26-5bf84943ec2c/etc/bash.bashrc
#
# /etc/bash.bashrc
#

# If not running interactively, don't do anything
[[ $- != *i* ]] && return

[[ $DISPLAY ]] && shopt -s checkwinsize

PS1='[\u@\h \W]\$ '

case ${TERM} in
  xterm*|rxvt*|Eterm|aterm|kterm|gnome*)
    PROMPT_COMMAND=${PROMPT_COMMAND:+$PROMPT_COMMAND; }'printf "\033]0;%s@%s:%s\007" "${USER}" "${HOSTNAME%%.*}" "${PWD/#$HOME/\~}"'

    ;;
  screen*)
    PROMPT_COMMAND=${PROMPT_COMMAND:+$PROMPT_COMMAND; }'printf "\033_%s@%s:%s\033\\" "${USER}" "${HOSTNAME%%.*}" "${PWD/#$HOME/\~}"'
    ;;
esac

[ -r /usr/share/bash-completion/bash_completion   ] && . /usr/share/bash-completion/bash_completion
source /etc/profile.d/ps1.sh

