# Domogik-pi2-sd-image from DEVELOP branch

http://dl.free.fr/s6wmZguga

For now you need at least a 4go sd card. The image could work on a 2go but has not been test for that.
Don't forget for now it is just a proof of concept, it hasn't been test for long running period.

Almost all plugins are install with this version in dev branch.

Based on last Raspbian-jessie-lite (2016-05-10)

SSH enable by default & dhcp enable

##First boot after burning the card:

Expand filesysem:

- Connect a keyboard and a screen to the pi2, login as pi/raspberry, sudo raspi-config and expand filesystem.
- It could be slow to login on 1st boot don't worry. After that reboot to aplly new filesystem.
- When expand will be finished, you can put your pi in another place and play with domogik.

For me it tooks ~1 and 2 minutes to have the domogik admin page ready after powering the pi2.

##Default value:

Domogik/Domoweb use default port (40406/40404), no ssl, and default login/password (admin/123)

User/password for ssh:
pi/raspberry

User domoweb as password *domopass*

##Change to make to accord your installation:

***In /etc/domoweb.cfg line 5 change rest_url to your pi2 IP.***

##If domogik don't start automatically re-run the installation:

http://docs.domogik.org/domogik/develop/en/enduser/installation/index.html#install-domogik

$ cd /opt/dmg/domogik/

$ sudo ./install.py

$ sudo /etc/init.d/domogik restart

##Mysql part:

Mysql db root password is *domopass*

Tuning mysql with information took here:
http://workshop.botter.ventures/2014/02/09/how-to-install-and-optimize-mysql-on-raspberry-pi/

##Hardware information:

I have test it on a pi1 model B (1st gen), it is working but really not useable at all.

Recommended at least a pi2 model B.

It has been test and validate on a pi3 by dertione here : https://github.com/domogik/domogik/issues/324#issuecomment-241289542
