# makh00ra-nepsan0n
Stay anonymous on LINUX or Kali

First we need tor,, its probably already installed but if not:


apt-get install tor


Then we need to edit the tor config in /etc/default/tor to allow it to be ran as daemon


gedit /etc/default/tor


you will see: RUN_DAEMON="no"

change it to say "yes"

control it with the commands:


service tor start


service tor stop


service tor restart


service tor status

now open the torrc file


gedit /etc/tor/torrc

and add this to the bottom:
Quote

    VirtualAddrNetwork 10.192.0.0/10
    AutomapHostsOnResolve 1
    TransPort 9040
    DNSPort 53
    
(Referencedd BY Backbox)

then download 
By Typing 
cd Desktop
git clone https://github.com/makh00ra/makh00ra-nepsan0n
 then a folder name makh00ra-nepsan0n will be downloade on your desktop

┌─────────[root@makh00ra] 
|-[~/Desktop] 
└─>[08:58:37]─> git clone https://github.com/makh00ra/makh00ra-nepsan0n
 now type:
 
 ┌─────────[root@makh00ra] 
|-[~/Desktop] 
└─>[09:03:44]─> cd makh00ra-nepsan0n

┌─────────[root@makh00ra] 
|-[~/Desktop/makh00ra-nepsan0n] 
└─>[09:03:51]─> ls
makh00ra.sh  README.md

┌─────────[root@makh00ra] 
|-[~/Desktop/makh00ra-nepsan0n] 
└─>[09:03:55]─> 

 ./makh00ra.sh start
┌─────────[root@makh00ra] 
|-[~/Desktop/makh00ra-nepsan0n] 
└─>[09:08:14]─> ./makh00ra.sh start

anonymity through TOR service will be activated on your system
 

Inspired By
============

ParrotSec AnonSurf core module


this script is preinstalled on Parrot Security OS

and its aim is to provide a strong system-wide anonymization module for another OS



how to use this repo
====================

This makh00ra folder contains the sources of our deb package


the makhoora deb package can be used to correctly install it on a debian/ubuntu system
(COMING SOON)


there is also a bash script that can be used independently on any system with iptables and a tor transproxy
but not all the features of the packet are available
