# Raspberry Pi 3.5 inch display driver
This driver is based on KeDeI LCD displays.<br>
Initially it's downloaded from http://en.kedei.net/raspberry/raspberry.html<br>
They updated their website and this driver is not possible to be downloaded anymore that's why I've uploaded it here.<br>
However, running the initial driver will not make your display work, and people are confused why.<br>
In order to work you have to do some modifications in /boot/config.txt file to start the display.<br>
<br>
I've automated the process and all you have to do before running the script is:<br>
sudo raspi-config<br>
set the OpenGL mode to Fake KMS<br>
run ./set_lcd<br>
<br>
To revert again to HDMI, simply run ./set_hdmi
<br>
<br>
Please note that this driver uses it's own kernel and it will change yours.<br>
Also this will not work on the newest Raspberry Pi OS, the last version of Raspbian which I managed to get it work is Stretch from 2019-04-08<br>
You can download it here - https://downloads.raspberrypi.org/raspbian/images/raspbian-2019-04-09/
