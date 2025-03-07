# Hyperbian
Raspberry 3 or 4 hyperbian configuration &amp; description

1. Load and flash Hyperbian image, get image here: https://github.com/Hyperion-Project/HyperBian/releases
2. boot raspi
3. SSH in
4. use credentials User: hyperion, Password: ambientlight
5. run the following command to start hyperion web interface
6. sudo systemctl disable --now hyperion@pi
7. sudo systemctl enable --now hyperion@root


Alternative

1. Flash rapberry pi os lite 64 bit to cd card
2. boot and wait
3. ssh in
4. sudo apt update && sudo apt upgrade -y
5. wget https://github.com/awawa-dev/HyperHDR/releases/download/v20.0.0.0/HyperHDR-20.0.0.0-Linux-aarch64.deb
6. wget https://github.com/awawa-dev/HyperHDR/releases/download/v21.0.0.0beta2/HyperHDR-21.0.0.0.bookworm.beta2-aarch64.deb
7. wget https://github.com/awawa-dev/HyperHDR/releases/download/v19.0.0.0/HyperHDR-19.0.0.0-Linux-aarch64.tar.gz

Raspi 3b+
8. wget https://github.com/awawa-dev/HyperHDR/releases/download/v19.0.0.0/HyperHDR-19.0.0.0-Linux-armv6l.deb
9. sudo apt install ./HyperHDR-20.0.0.0-Linux-aarch64.deb
10. sudo apt install ./HyperHDR-21.0.0.0.bookworm.beta2-aarch64.deb
11. sudo apt install ./HyperHDR-19.0.0.0-Linux-aarch64.tar.gz

Raspi 3b+
12. sudo apt install ./HyperHDR-19.0.0.0-Linux-armv6l.deb
13. sudo sed -i '/^User/d' /etc/systemd/system/hyperhdr\@.service
14. sudo systemctl daemon-reload
15. sudo service hyperhdr@pi restart
16. sudo service hyperhdr@pi status


Leds:
top: 72
bottom: 71
left: 41
right: 40



