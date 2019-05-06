# Raspberry Pi 3.5 inch display driver
This driver is based on KeDeI LCD displays.<br>
Initial driver is downloaded from http://en.kedei.net/raspberry/raspberry.html<br>
However, running the initial driver will not make your display work, and people are confused why.<br>
In order to work you have to do some modifications in /boot/config.txt file to start the display.<br>
<br>
I've automated the process and all you have to do before running the script is:<br>
sudo raspi-config<br>
set the OpenGL mode to Fake KMS<br>
run LCD_show/lcd_35<br>
<br>
To revert again to HDMI, simply run LCD_show/lcd_hdmi