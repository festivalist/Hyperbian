# Hyperbian
Raspberry 3 or 4 hyperbian configuration &amp; description

1. Load and flash Hyperbian image, get image here: https://github.com/Hyperion-Project/HyperBian/releases
2. boot raspi
3. SSH in
4. use credentials User: hyperion, Password: ambientlight
5. run the following command to start hyperion web interface
6. sudo systemctl disable --now hyperion@pi
7. sudo systemctl enable --now hyperion@root


Alternative testing on raspi 4

1. Flash rapberry pi os lite 64 bit to cd card
2. boot and wait
3. ssh in and execute
```
sudo apt update && sudo apt upgrade -y
```
```__
wget https://github.com/awawa-dev/HyperHDR/releases/download/v20.0.0.0/HyperHDR-20.0.0.0-Linux-aarch64.deb
__```

```
old
wget https://github.com/awawa-dev/HyperHDR/releases/download/v19.0.0.0/HyperHDR-19.0.0.0-Linux-armv6l.deb
wget https://github.com/awawa-dev/HyperHDR/releases/download/v21.0.0.0beta2/HyperHDR-21.0.0.0.bookworm.beta2-aarch64.deb
```



```
sudo apt install ./HyperHDR-20.0.0.0-Linux-aarch64.deb
```
```
old
sudo apt install ./HyperHDR-19.0.0.0-Linux-armv6l.deb
sudo apt install ./HyperHDR-21.0.0.0.bookworm.beta2-aarch64.deb
```


```
sudo sed -i '/^User/d' /etc/systemd/system/hyperhdr\@.service
```
```
sudo systemctl daemon-reload
```
```
sudo service hyperhdr@pi restart
```
```
sudo service hyperhdr@pi status
```

Leds:
top: 72
bottom: 71
left: 41
right: 40
input position: 183
Mode: brg oder grb (jeweils zweiter teil rot)



