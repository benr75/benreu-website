---
layout: post
title: Setting up WireGuard VPN on Debian 11
categories: []
tags: []
status: publish
type: post
published: true
meta: {}
---
Putting this here to remind myself the next time I need to do this ;). 

Update package information

`sudo apt update`

Install WireGuard

`sudo apt install wireguard`

Reboot

`sudo reboot`

Debian 11 uses resolvectl, symlink it to resolvconf so WireGuard can use it

`sudo ln -s /usr/bin/resolvectl /usr/local/bin/resolvconf`

Enable resolved

`sudo systemctl enable systemd-resolved.service`

Start WireGuard

`sudo wg-quick up PATH_TO_YOUR_WIREGUARD_CONF`


For reference:
<https://superuser.com/questions/1500691/usr-bin-wg-quick-line-31-resolvconf-command-not-found-wireguard-debian>

<https://superuser.com/questions/1427311/activation-via-systemd-failed-for-unit-dbus-org-freedesktop-resolve1-service>

------
