# VENTOY-USB-SETUP
### Setup:
Download "ventoy-x.x.xx-linux.tar.gz" from: https://www.ventoy.net/en/download.html
```
cd ~/Downloads/
7z x ventoy-x.x.xx-linux.tar.gz
7z x ventoy-1.1.07-linux.tar
cd ventoy-x.x.xx/
lsblk -f
sudo ./Ventoy2Disk.sh -i /dev/sda
```

### Usage:
Just copy the ISO files to the USB folder.
```
lsblk -f
sudo mount /dev/sdaX /mnt/ventoy/
cp /path/to/file.iso /mnt/ventoy/
```
