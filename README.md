# Hyperbian
Raspberry 3 or 4 hyperbian configuration &amp; description

1. Load and flash Hyperbian image, get image here: https://github.com/Hyperion-Project/HyperBian/releases
2. boot raspi
3. SSH in
4. use credentials User: hyperion, Password: ambientlight
5. run the following command to start hyperion web interface
# old 6. sudo /usr/share/hyperion/bin/hyperiond
7. sudo systemctl disable --now hyperion@pi
8. sudo systemctl enable --now hyperion@root


Alternative

1. Flash rapberry pi os lite 64 bit to cd card
2. boot and wait
3. ssh in
4. sudo apt update && sudo apt upgrade -y
5. wget https://github.com/awawa-dev/HyperHDR/releases/download/v20.0.0.0/HyperHDR-20.0.0.0-Linux-`uname -m`.deb
6. sudo apt install ./HyperHDR-20.0.0.0-Linux-`uname -m`.deb
7. sudo sed -i '/^User/d' /etc/systemd/system/hyperhdr\@.service
8. sudo systemctl daemon-reload
9. sudo service hyperhdr@pi restart
10. sudo service hyperhdr@pi status
