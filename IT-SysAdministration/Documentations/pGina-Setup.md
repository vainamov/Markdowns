## pGina Setup Documentation

#### Requires
- Windows 7 or higher
- A configured LDAP server
- pGina
> Note: It is highly recommended to create a recovery point and/or try this out in a virtual machine first.

#### Documentation Setup
|OS|LDAP server|pGina|
|---|---|---|
|Windows 10 Pro x86<br/>(10.0.14393 Koontikäännös 14393)<br/>FI-fi<br />3.02Gt RAM / 70Gt ROM|OpenDJ Server 3.0.0|pGina 3.2.4.1 Beta|

***
### Configure pGina
#### Activate Plugins
In pGina, open the tab "Plugin Selection" and tick the boxes "Authentication", "Authorization" and "Gateway" on both the LDAP plugin and the Local Machine plugin.
#### Re-order Plugins
Open the "Plugin Order" tab and use the arrow buttons to make sure that LDAP comes first in "Authorization" and "Gateway" but last in "Authentication".
#### Configuring the LDAP Plugin
(Depending on your server configuration, this step might be different for you.)  
Head back to the "Plugin Selection" tab and double click the LDAP entry.  

![Plugin](https://sjzwzw.bl3302.livefilestore.com/y4mAYEvx4Ahky5KWpD_chdEO8zaSzfm0njvQpuuN1pbhlD6pMPlVlngPokmmMfkdG1PXBAnWuHeX_2ok_cIN8HBuJOyDZpBBKJh5icBf8JY_4Q1-DJHi4TJfGmBMMbVzWl-5d0VtIHXk51rYf4WkYGRu4Pw5VgE1ADZLWm3SzgDRvnxVDRnRBqavdbhZ8nI2ZEGli52r_XEVlRGL8ZhKjZM_Q?width=702&height=534&cropmode=none)

Given you have a server running on 10.60.20.251:1389 with a structure like this:
- dc=ldap,dc=festival,dc=ml
  - ou=groups
    - cn=Administrators
    - cn=Users
  - ou=members
    - uid=user1
    - uid=user2
    - uid=...
  
Your configuration should look like the above screenshot. However, depending on your server software you might need to change the Member Attribute value to "memberUid" and/or the User DN Pattern to start with "cn=%u,".

Next, switch to the "Authorization" tab at the bottom and configure it so it fits your needs (head to the [pGina docs](pgina.org/docs/v3.1/ldap.html) and look for "Authorization Options" for more details).  

Finally, open the "Gateway" tab and map your LDAP groups to the corresponding local groups to ensure everyone will have the correct permissions. Save you configuration and click "Apply" in pGina to submit your changes to the registry.  

***
### Testing
There are two possible ways of testing your pGina setup. You can either use the built-in simulation or just keep logging off and back on again, decide for yourself which method you prefer.
  
***
### Troubleshooting
Should you run into issues with your pGina setup, there are several things that might help you. First, check the simulation log (click the "Show Log" button in the Simulation tab). It should provide enough details to determine where things mess up. If this doesn't help you fixing the problem on your own, head to the [closed issues on the pGina repository](https://github.com/pgina/pgina/issues?q=is%3Aissue+is%3Aclosed) and check if your problem has been discovered and solved already. If none of this was successful, [create a new issue](https://github.com/pgina/pgina/issues/new) and try to describe your situation as detailed as possible (include the log as well). 
