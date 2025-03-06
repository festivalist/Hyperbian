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


config hyperbian:
tbc
