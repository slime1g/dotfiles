# wallpaper
*config:*
 vim ~/.config/labwc/autostart

# Screenshot

# Bereich auswählen, direkt in die Zwischenablage
grim -g "$(slurp)" - | wl-copy

# ganzer Bildschirm in die Zwischenablage
grim - | wl-copy

# Bereich als Datei speichern
grim -g "$(slurp)" ~/Pictures/shot.png

# ganzer Bildschirm als Datei mit Zeitstempel
grim ~/Pictures/shot-$(date +%F-%H%M%S).png

Voraussetzung:
sudo pacman -S grim slurp wl-clipboard

screenrecord
wf-recorder 
