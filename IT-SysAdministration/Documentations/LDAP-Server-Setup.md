## LDAP Sever Setup Documentation

#### Requires
- Windows 7 or higher
- A configured LDAP server
- LDAP Admin (Downloadable at http://ldapadmin.org/download/ldapadmin.html)

#### Documentation Setup
|OS|LDAP Server|
|---|---|
|Windows 10 Pro x64<br/>(Version 1703 Build 15063.138)<br/>DE-de|OpenDJ 3.0.0|

***
### LDAP Server Setup
#### Connecting
In LDAP Admin, click the top left "Connect" button and double click the "New Connection" entry.  

![LDAP](https://dz7zoa.bl3302.livefilestore.com/y4mJkBFLh2BT9ZbXgrIZGQWvSNqMIbqm4qQec6fty3VQAYClgAv9fpVeXYta1rcX6yZO2mG7WSBkzTpkfBew75x2vWzEppdO8tMaH5o_SXWS2pI_4qe8c7nNLoJ117sW3s-XyGFX1X2_eScQ43npYKieoF8gkSefM38K94l9gish5tvdMOd8aka-Tq0_G_pMDGFwwiM9T79c33VyRby9KEO8Q?width=452&height=419&cropmode=none)  

Enter your corresponding server data and confirm with "OK". After adding the server, double click the entry to connect.
  
#### Implementing Basic Structure
Select your base dn and press `Ctrl+O` to create new organizational units (OU). In the example, we created one for all groups, and one for all members (/users).
  
#### Creating Groups
Select the `ou=groups` entry and press `Ctrl+G` to create a new group.
