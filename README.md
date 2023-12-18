# Surendoy Remote Proxy-Server Configurator Light
__SRPSС Light__ is software allows you to quickly configure a vps for a proxy server with 120 unique ipv6 addresses for connection and 
the ability to upload authentication data to a MySQL database.

## How to choose a vps?
__VPS Requirement:__
  - Ubuntu 20.04
  - Ipv6 subnet access
  - Ports are not blocked

__Verified hosters:__
 - [4vps.su](https://4vps.su/)
 - [pq.hosting](https://pq.hosting/)
 - ...

## Quick start
All actions are performed on behalf of the __root__ user


After connecting to the VPS, update and upgrade OS:
```
apt-get install update --force-yes -y && apt-get install upgrade --force-yes -y
```
Install Git:
```
apt-get install git --force-yes -y
```
Clone repository:
```
git clone https://github.com/sunrekay/SRPSС-Light
```
Go inside the folder:
```
cd SRPSС-Light
```
Install requirements:
```
pip install -r requirements.txt
```
And start configuration:
```
python configurator.py
```

After configuring the vps, the authentication data is saved in the "auth" file, but if you need to upload the data to the MySQL database, 
then in the settings.py it is necessary to specify the data for connection.