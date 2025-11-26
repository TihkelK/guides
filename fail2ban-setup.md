# FAIL2BAN-SETUP
```
sudo apt install fail2ban -y
```
```
sudo nano /etc/fail2ban/jail.d/sshd.conf
```
```
[sshd]
enabled = true
backend = systemd
maxretry = 3
bantime = 24h
```
```
sudo systemctl restart fail2ban.service
```
