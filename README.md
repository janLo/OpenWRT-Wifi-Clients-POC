# Query OpenWRT WiFi Clients

This is a simple POC for the OpenWRT ubus JSON-RPC interface
to query associated WiFi clinets from the running hostapd.

This can be useful as trigger for various home automation
actions like lowering the heating temp if everyone is "gone"
(or everyones phone is off).

The usage is very simple:

    ./wifi_clients.py <server> <username> <passwd> <wifi_1> [<wifi_2> ...]

For examle:

    $ ./wifi_clients.py 192.168.0.1 user pass wlan0 wlan1
    08:11:aa:bb:aa:dd, f8:d1:aa:dd:ba:bc

For more information see:
http://wiki.openwrt.org/doc/techref/ubus#access_to_ubus_over_http
