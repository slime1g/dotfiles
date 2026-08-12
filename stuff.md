# wallpaper
*config:*
 vim ~/.config/labwc/autostart

# Screenshot
grim -g "$(slurp)" - | wl-copy
grim - | wl-copy
grim -g "$(slurp)" ~/Pictures/shot.png
grim ~/Pictures/shot-$(date +%F-%H%M%S).png
Voraussetzung:
sudo pacman -S grim slurp wl-clipboard
screenrecord
wf-recorder 

### all things we need
`sudo pacman -S --needed \
  labwc xorg-xwayland \
  alacritty bemenu bemenu-wayland fuzzel swaybg \
  grim slurp wl-clipboard wf-recorder \
  pipewire pipewire-pulse pipewire-audio wireplumber \
  sof-firmware alsa-ucm-conf alsa-utils rtkit \
  mesa vulkan-intel intel-media-driver libva-utils \
  brightnessctl \
  papirus-icon-theme adwaita-icon-theme \
  ttf-go-nerd ttf-dejavu noto-fonts noto-fonts-emoji \
  thunar gvfs tumbler \
  firefox fastfetch \
  git vim libxml2 wget openssh \
  networkmanager glib2 dconf \
  tlp acpid`
### AUR
  yay -S yambar wlopm