Installing firmware for broadcom 4312
https://askubuntu.com/questions/486917/lenovo-s10-bcm-4312-rev-01-wifi-not-functioning
apt-get install linux-firmware-nonfree
modprobe -r b43
modprobe b43
and see the error
https://ubuntuforums.org/showthread.php?t=1830336
apt-get install --reinstall b43-fwcutter firmware-b43-installer
try reload b43 again. If successful, ip addr should give the wlan interface.
