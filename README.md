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


then download 

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
