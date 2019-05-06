Initial install steps

sudo apt-get update
sudo apt-get upgrade

wget http://en.kedei.net/raspberry/v6_1/LCD_show_v6_1_3.tar.gz

tar -xvzf LCD_show_v6_1_3.tar.gz
cd LCD_show_v6_1_3

sudo ./LCD35_v

sudo raspi-config

set OpenGL Fake KMS

add rows below to /boot/config.txt
hdmi_group=2
hdmi_mode=35
dtparam=spi=off

hdmi_force_hotplug=1
gpu_mem=32
start_x=0
enable_uart=1
dtoverlay=w1-gpio