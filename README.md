# locate-lost-wifi-device
How to physically locate a lost WiFi access point that still sends a WiFi signal

Download Kali Linux ("Live Boot" version) from https://www.kali.org/get-kali/#kali-live

Enter the following commands:
```
sudo airmon-ng
--> shows a list of all WiFi devices installed and accessible to Kali Linux

sudo airmon-ng start wlan0
--> replace wlan0 with the name of the correct WiFi "interface"

sudo airmon-ng
--> the interface should now be called "wlan0mon"

sudo airodump-ng wlan0mon
```
Try to find the lost WiFi device by walking around and trying to make the `PWR` value go to 0 (zero).


## Links
- WifiInfoView by NirSoft
- https://www.nirsoft.net/utils/wifi_information_view.html
- https://play.google.com/store/apps/details?id=com.vrem.wifianalyzer
- https://github.com/VREMSoftwareDevelopment/WiFiAnalyzer
- MoocherHunter
- https://superuser.com/questions/601005/how-do-i-physically-find-a-wifi-device-using-a-laptop-or-mobile-phone
- https://lifehacker.com/how-can-i-find-a-lost-device-when-its-in-silent-mode-1082395852
- https://www.youtube.com/watch?v=EWmSnE4MTyk WifiInfoView
- https://www.accessagility.com/blog/locating-rogue-access-points
- https://www.dnsstuff.com/de/wlan-analyse-software
- https://alternativeto.net/software/wifi-analyzer/?license=free
- https://forum.churchitnetwork.com/t/need-to-find-a-physical-wifi-router-wireless-access-point/949
- https://community.spiceworks.com/topic/2010487-missing-ap-how-can-i-locate-it
- https://www.reddit.com/r/Hacking_Tutorials/comments/lbf9i7/how_to_track_a_device_connected_to_wifi/ airodump-ng / aircrack-ng / Kali Linux
- https://www.youtube.com/watch?v=uKZb3D-PHS0 HakByte: Advanced WiFi Scanning with Airodump-ng
- https://www.aircrack-ng.org/doku.php?id=newbie_guide
- https://www.aircrack-ng.org/doku.php?id=airodump-ng
