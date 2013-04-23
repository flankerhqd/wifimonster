wifimonster
===========

Wifi sniffing and hijacking tool

Currently the tool is able to 

* sniff cookie and form passwords from open wifi in monitor mode
* one-click to launch a browser with sniffed cookie

This tool does not require ARP attack, just silent sniffing, thus invisible to victim. Besides, the sniffing does not require
one to associate one AP, making it even more diffcult to detect.

#Requirements:

* PyQT >4
* Scapy >2.0


#Usage:

e.g: python cookiemonster.py -i en0 [-c 1]

    File / Interface
        -i --interface <interface>    Choose specified interface
        -f --file <filename>         Choose specified filename
        -c --channel <channel>      Choose specified channel (For Mac OS X only)
        
On poping cookie window, right click on *useragent* items and select "launch attack" to open a browser using sniffed cookie.
Sniffed passwords are stored in *monsterCookie.log*
