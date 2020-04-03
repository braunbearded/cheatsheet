# Programs
* pdf: zathura/okular/qpdfview
* image view: feh/sxiv
* screenshot: import
* clipboard: xclip
* notfication: notify-send
* disk usage (tree): ncdu
* partion (gui): gparted
* Get Window class: xprop
* Get Key pressed: xev
* Show keys pressed: screenkeys
* stopuhr: termdown
* ocr: tesseract/ocrmypdf
* notes: xournalpp
* paint (alternative): pinta
* filemanager: ranger, pcmanfm
* calculator: bc, speedcrunch
* webcam-settings: v4l-utils
* wifi-settings: nmtui

# pacman
* update database: sudo pacman -Syy
* update && upgrade: sudo pacman -Syu
* install package: sudo pacman -S package_name
* remove package: sudo pacman -Rns
* Uninstall unneeded packages:pacman -Rns $(pacman -Qdtq)
* clear cache /var/cache/pacman: sudo pacman -Scc
* clear cache pacman/aur: sudo yay -Scc
* list explictly installed packages: sudo pacman -Qe
* list explictly installed aur packages: sudo pacman -Qm
* list unsued packages: sudo pacman -Qtdq
* list packages which required X: sudo pacman -Sii packagename_x
* file ownd by package: pacman -Qo /path/to/file
* yay skip check: yay -S --mflags --nocheck packagename
* list all packages: pacman -Sgg
* install from file input: pacman -S - < file

# Manjaro specific
+ update mirror sort by download speed:
+ sudo pacman-mirrors --fasttrack && sudo pacman -Syyu

# Mounting
* mount via ssh:
* sshfs user@ip:/remote/path ~/local/path
* unmount ssh:
* fusermount3 -u ~/local/path

# docker
* remove all docker stuff: sudo docker system prune -a --volumes
* start deamen: sudo systemctl start docker.service
* start container: sudo docker start <id>
* remove not needed childs: docker rmi $(docker images --filter "dangling=true" -q --no-trunc)

# Syncthing
* Conflict files: "*sync-conflict-*"

# Cron log
* journalctl -u cronie.service

# Last command from terminal in vim buffer, execute on exit
* fc

# open random file from dir
* ls | shuf | head -n 1 | xargs prog

# rebuild initram fs
* sudo mkinitcpio -P

# rebuild grub config
* sudo grub-mkconfig -o /boot/grub/grub.cfg

# add user to group
* sudo usermod -a -G examplegroup exampleusername

# mac address spoofing
* ip link show interface
* ip link set dev interface down
* ip link set dev interface address XX:XX:XX:XX:XX:XX
* ip link set dev interface up

# List size for all directorys
* cd /
* ncdu --exlclude "/path" .

# ADB
* install package: cmd package install-existing <package>
* remove package: pm uninstall -k --user 0 <package>
* installed apps on user 0 (default): pm list packages --user 0
* all apps: pm list packages --user 0 -u

