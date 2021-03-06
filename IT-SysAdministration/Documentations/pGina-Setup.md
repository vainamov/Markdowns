## pGina Setup Documentation

#### Requires
- Windows 7 or higher
- A configured LDAP server
- pGina (Downloadable at https://github.com/pgina/pgina/releases)
> Note: It is highly recommended to create a recovery point and/or using a virtual machine for testing first.

#### Documentation Setup
|OS|pGina|
|---|---|
|Windows 10 Pro x86<br/>(Version 1607 Build 14393.953)<br/>FI-fi<br />3.02GB RAM / 70GB ROM|pGina 3.1.8.0|

***
### Configure pGina
#### Activate Plugins
In pGina, open the tab "Plugin Selection" and tick the boxes "Authentication", "Authorization" and "Gateway" on both the LDAP plugin and the Local Machine plugin.  

![Plugin](https://sjwtzq.bl3302.livefilestore.com/y4mJPx0WRL9v3788HAD_9P7eVlqdK2O6N3eUsdudm6f1mJcm4BYfqxn3fhZhR4QD8Vdl0mD_fLGc_SuXaxTjQuHs6u11isZnZSvaihWEJ_vlUjYFPFL1DV9_2tx67moirwPfqP6lYfXH9RS8FIrUU1stpnOu29zM6z9FY_9V27oiU7402gYOYKU35AsD_gpICR9krSKfi05sVBwPSJl4szCEQ?width=825&height=669&cropmode=none)  

#### Re-order Plugins
Open the "Plugin Order" tab and use the arrow buttons to make sure that LDAP comes first in "Authorization" and "Gateway" but last in "Authentication".  

![Plugin](https://sjzi2q.bl3302.livefilestore.com/y4mvUpQwc-rk1b6WCpfif9Ii1wI1VLaclS7LJwW5JEibWa0LwkZMmcBpgEmG0XHHqgNO20fIrokA4Rwv-ibUecO2yATDJ03ILgi5PDdTCkAjKwiK2yae2xASe0VFR38lUgWdZPr9aSVvvNf7Xl9spkTwPXMGOm4JrnyQ-RIrXNYIj3D_j7ZaVslvNUwH4yJrK1hicscQpsiGdSfelKo-1UA6A?width=825&height=671&cropmode=none)  

#### Configuring the LDAP Plugin
(Depending on your server configuration, this step might be different for you.)  
Head back to the "Plugin Selection" tab and double click the LDAP entry.  

![Plugin](https://sjzwzw.bl3302.livefilestore.com/y4mAYEvx4Ahky5KWpD_chdEO8zaSzfm0njvQpuuN1pbhlD6pMPlVlngPokmmMfkdG1PXBAnWuHeX_2ok_cIN8HBuJOyDZpBBKJh5icBf8JY_4Q1-DJHi4TJfGmBMMbVzWl-5d0VtIHXk51rYf4WkYGRu4Pw5VgE1ADZLWm3SzgDRvnxVDRnRBqavdbhZ8nI2ZEGli52r_XEVlRGL8ZhKjZM_Q?width=702&height=534&cropmode=none)

#### Authentication
Given you have a server running on `10.60.20.251:1389` with a structure like this:
- dc=ldap,dc=festival,dc=ml
  - ou=groups
    - cn=Administrators
    - cn=Users
  - ou=members
    - uid=user1
    - uid=user2
    - uid=...
  
Your configuration should look like the above screenshot. However, depending on your server software you might need to change the Member Attribute value to `memberUid` and/or the User DN Pattern to start with `cn=%u,`.

#### Authorization
Next, switch to the "Authorization" tab at the bottom and configure it so it fits your needs (head to the [pGina docs](http://pgina.org/docs/v3.1/ldap.html) and look for "Authorization Options" for more details).  

#### Group-Mapping (Gateway)
Finally, open the "Gateway" tab and map your LDAP groups to the corresponding local groups to ensure everyone will have the correct permissions.  

![Plugin](https://sjw78w.bl3302.livefilestore.com/y4m4AV0uDn-O4GQ_Ff6NG3naMAMKZeiTl7O1-AEyIIpHJfCO3Q-_Qzan2lfeeWW8mZFACh6tEy0JKM3c5LXxcee83REABLxZ9Z0jjEEQmMMj1xg3ewTMkxjEuUk4G4tNKARG6z7gp2gewJL7VBlV1NfKNFPGUAAmgxN6IAmam9Qj4Vtc17pCFBGDe4qQYDxD3FK9GFPFedw1ug62ukM0oOPHg?width=703&height=313&cropmode=none)  

> Note: Make sure to use the exact local group names. If you're unsure about the correct spelling open the command line interface (`WIN+R` > `cmd`) and enter the `net localgroup` command. It produces an output similar to the one shown below and lists all existing groups.  

![Plugin](https://dz6qlg.bl3302.livefilestore.com/y4mhBva97CJTCbSk6pUoqFzIkZccUDCUsJOMUIkPOnXwb6f4MXafvUMgmz3GO7tnK8WA_hQ6Aqp6TA8QbvOUPSw5suEO-ewzq6K52dWC0X0-L41jmt3NpsKU6JqnY4bU7wdknGPYQHR61BAERKiSZUmqVRwU_Orvm0I4_D9tTgoqwqknWoQfTbkFZWQ5Ck9mlGq8iK-wYppSx9eDgAun_VwjA?width=660&height=347&cropmode=none)  

Save your configuration and click "Apply" in pGina to submit your changes to the registry.  

***
### Testing
There are two possible ways of testing your pGina setup. You can either use the built-in simulation or just keep logging off and back on again, decide for yourself which method you prefer.
  
***
### Troubleshooting
Should you run into issues with your pGina setup, there are several things that might help you. First, check the simulation log (click the "Show Log" button in the Simulation tab). It should provide enough details to determine where things mess up. If this doesn't help you fixing the problem on your own, head to the [closed issues on the pGina repository](https://github.com/pgina/pgina/issues?q=is%3Aissue+is%3Aclosed) and check if your problem has been discovered and solved already. If none of this was successful, [create a new issue](https://github.com/pgina/pgina/issues/new) and try to describe your situation as detailed as possible (include the log as well).
  
***
### Finishing Touches
- Double click the Local Machine plugin in the "Plugin Selection" tab and check "Remove account and profile after logout when account does not exist prior to logon."  
  This will force Windows to delete the profile created by pGina and prevent the `C:\Users\`-folder from overcrowding.
- Open the "General" tab and assign an image to the pGina service. You can also enter a MOTD (message of the day) and configure a message to display when connecting. This will change the appearance of the pGina entry in the login screen.
  
***
### Automatic Drive Mapping
Using [pGina 3.2.1.1 Beta](https://github.com/pgina/pgina/releases/tag/v3.2.1.1) or newer, will provide a plugin called "Drive Mapper". Bespoken plugin has the ability to automatically map network drives (e.g. a home directory on a samba server) to the local machine. If a stable version of pGina is prefered, it is also possible to download the plugin individually and include it in the existing pGina installtion by placing it in the plugins folder `C:\Program Files\pGina\Plugins\Core\`.  

![Plugin](https://dz50rq.bl3302.livefilestore.com/y4mSqh1KqdBCg_cflJAUyekxXWHxcM1ShKWQf5EM8zhBLPivVOBwGQlAUOw9be7eBkKwj5pYtk3cTOAeaFj0HZa48QBWjSK6jg-xjSEuq2qEAJgeU5STtgAOYHAuUZY8uysUr6nmnGvvQHMvcBMAU0qKd7h-PgvJHPLSnWV--tuqECGqRsmbs-tiQHiqa4G3Lc4IheIDNTLRcLWKlACnvx-7A?width=825&height=622&cropmode=none)
