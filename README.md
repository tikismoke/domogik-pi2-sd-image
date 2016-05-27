# domogik-pi2-sd-image

For now you need an 8go SD card, but it will be solved a day.

Repo to host the pi2 sd card of domogik in deve branch

SSH enable by default
Dhcp enable

Domogik/Domoweb use default port (40406/40404), no ssl, and default login/password (admin/123)

User/password for ssh:
pi/raspberry

User domoweb as domopass as password

Mysql db root password domopass

Change to make to accord your installation:

In /etc/domoweb.cfg line 5 change rest_url to your pi2 IP.

In /etc/domogik/domogik-mq-cfg change ip by your pi2 IP


Plugin install with this version:

-diskfree

-generic

-karotz

-nabaztag

-notify

-ozwave

-ping

-script

-vdevice

-wheather

-wol

https://snag.gy/PiFH6L.jpg
