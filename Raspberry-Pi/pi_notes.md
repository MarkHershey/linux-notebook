#Coding Notes 
##Linux/ Raspbian/ Raspberry Pi

[Setup a Static IP Address](https://raspberrypi.stackexchange.com/questions/37920/how-do-i-set-up-networking-wifi-static-ip-address/74428#74428)

[how-do-i-set-up-networking-wifi-static-ip-address](https://raspberrypi.stackexchange.com/questions/37920/how-do-i-set-up-networking-wifi-static-ip-address)

[network configuration](https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md)

[Set Static IP address but also getting Dynamic](https://www.raspberrypi.org/forums/viewtopic.php?f=28&t=111709&sid=a0c26106977cd12d6ae5cca41a63a174&start=25)

[Pi Camera Python Docs](https://picamera.readthedocs.io/en/release-1.13/index.html)

Current Pi's IP: `10.12.20.137`		
Connect to Pi via SSH: `ssh pi@10.12.20.137`	
Current passwd: `hh****911`

---
`ifconfig`	
`ip -4 addr show | grep global`
`ip route | grep default | awk '{print $3}'`
`cat /etc/resolv.conf`

`sudo passwd` Reset UNIX password, (this password is also the system password, and the password for connecting SSH.)


`nano [path/filename]` Open and edit file


`/etc/network/interfaces` This file is not supposed to be changed by any user.

`sudo nano /etc/dhcpcd.conf` Edit **dhcpcd** configuration file with admin permission: Set Static IP etc. 

**SUTD_Wifi** Router IP:

`10.12.0.1`

SUTD Domain Name Server (DNS) Address:

`192.168.2.100`
`192.168.2.101`

Search Domains: (not sure what it is yet)

`sutd.edu.sg`
`stf.sutd.edu.sg`

Install Python Packages for specific python version only: [Ref](https://docs.python.org/3/installing/index.html)
`python3 -m pip install <package name>`

[Other solutions](https://stackoverflow.com/questions/10763440/how-to-install-python3-version-of-package-via-pip-on-ubuntu)
[Other solutions2](https://help.dreamhost.com/hc/en-us/articles/115000699011-Using-pip3-to-install-Python3-modules)
















