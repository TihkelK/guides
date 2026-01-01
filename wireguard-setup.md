# WIREGUARD-SETUP
## Install:
```
sudo apt install -y wireguard
```

<br>

## Client side
### Add config file to wireguard directory:
```
sudo cp </path/to/file.conf> /etc/wireguard/[vpn-name].conf
```
### Activate connection with:
```
sudo wg-quick up [vpn-name]
```
#### Optional: Enable startup with:
```
sudo systemctl enable wg-quick@[vpn-name]
```

<br>

## Server side (pivpn):
#### Create new device config file:
```
pivpn -a
```
Follow through the setup guide. After that the config file will be created in the "/home/$USER/configs/" directory.
