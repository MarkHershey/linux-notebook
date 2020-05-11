## 1

For raspberry pi with Raspbian OS:

```
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
```

Change the content of the file to:

```
ctrl_interface=/var/run/wpa_supplicant
eapol_version=2
ap_scan=0

network={
        key_mgmt=IEEE8021X
        eap=PEAP
        identity="100xxxx"
        password="password"
        phase1="peaplabel=0"
        phase2="auth=MSCHAPV2"
}
```

Save & exit & restart

## 2

Run this in the terminal:

```
sudo wpa_supplicant -c /etc/wpa_supplicant/wpa_supplicant.conf -D wired -i eth0
```


# Wireless connection

```
network={
        ssid="ssid network"
        proto=RSN
        key_mgmt=WPA-EAP
        pairwise=CCMP
        auth_alg=OPEN
        eap=PEAP
        identity="user"
        password=hash:XXXXX
}

```






```
network={
        ssid="AU_WiFi"
        # For hidden SSIDs
        scan_ssid=1
        mode=0
        key_mgmt=WPA-EAP
        pairwise=CCMP TKIP
        identity="XXXXXXXX"
        password="XXXXXXXX"
        phase1="peaplabel=0"
        phase2="auth=MSCHAPV2"


}

```
