## Windows 10 Installation Documentation

#### Host
|OS|Specs|Virtualization Software|
|---|---|---|
|Windows 10 Pro x64<br/>(Version 1703 Build 15063.138)<br/>DE-de|Lenovo B71-80 80RJ00HMGE<br/>Intel Core i7-6500U, 8GB DDR3L SDRAM <br/> AMD Radeon M330 2GB 17,3"<br/>1TB Seagate ST1000LM024/HN-M101MBB|VMware® Workstation 12 Player<br/>(12.5.2 build-4638234)|

#### Virtual Machine
|OS|Specs|
|---|---|
|Windows 10 Pro x86<br/>(Version 1607 Build 14393.953)<br/>FI-fi|3.02GB RAM / 70GB ROM|

***
### Download Windows ISO
https://www.microsoft.com/de-de/software-download/windows10

### Download VMware® Workstation Player
https://my.vmware.com/de/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/12_0

***
### Configure Virtual Machine
|Step|Screenshot<br/>(Click for larger view)|
|---|---|
|Create a new virtual machine|[![Create a new virtual machine](https://rsfd8g.bl3302.livefilestore.com/y3mHdrvMLRKPsYk4E8zJxl-2mTzRdXbWMdWpKSqYCIcg5pTU7WA-T26YMNSvO5aRn5nc2r3vBAL8dt2YXrCUcPPTNZ0cMGeJN3B47Idly_-tZ8HN1bf1YkRIyRGCZkEpQvdSdg4iYjq3dO9DYQSlvlnOPT5Q8SYlMxv7S_wVpL8uTk?width=256&height=223&cropmode=none)](https://rsfd8g.bl3302.livefilestore.com/y3mHdrvMLRKPsYk4E8zJxl-2mTzRdXbWMdWpKSqYCIcg5pTU7WA-T26YMNSvO5aRn5nc2r3vBAL8dt2YXrCUcPPTNZ0cMGeJN3B47Idly_-tZ8HN1bf1YkRIyRGCZkEpQvdSdg4iYjq3dO9DYQSlvlnOPT5Q8SYlMxv7S_wVpL8uTk?width=700&height=609&cropmode=none)|
|Select the Windows ISO file|[![Select Windows ISO file](https://rsdlrg.bl3302.livefilestore.com/y3mnsWAHa-_64uc1P42azPxgEOAqc_7Joc9rP_nluYLbknoo4bDBwBKmXhHvjLdG-X3Yhpk5AYtgZUiKP71DLQlWzphKbs_F4b6ViQAPiZHNz3sNu_Mey36M9-XmUmiQaq_KNqBCaMApIvthsGbdMjmCe3V7An6aQqTzJ9TFwW6XlQ?width=256&height=223&cropmode=none)](https://rsdlrg.bl3302.livefilestore.com/y3mnsWAHa-_64uc1P42azPxgEOAqc_7Joc9rP_nluYLbknoo4bDBwBKmXhHvjLdG-X3Yhpk5AYtgZUiKP71DLQlWzphKbs_F4b6ViQAPiZHNz3sNu_Mey36M9-XmUmiQaq_KNqBCaMApIvthsGbdMjmCe3V7An6aQqTzJ9TFwW6XlQ?width=700&height=609&cropmode=none)|
|Name the virtual machine and select a location|[![Select vm name and location](https://rscofg.bl3302.livefilestore.com/y3mHhxH8CrHWcJLRpXFM36tWyopuHaN2wn8-4borte9mG3-gh212grxE_yw5iZsU7yS1rsNDWtpHFsyuuEcaHrmZy5aXF8Ipbd1SQ7iI5toKpo-pCQWtOapfzEmr0gnGl0PTDJGpub1xAP1h0Xlz8WlB5nNKNzbbvxHzTXzi27hi4c?width=256&height=223&cropmode=none)](https://rscofg.bl3302.livefilestore.com/y3mHhxH8CrHWcJLRpXFM36tWyopuHaN2wn8-4borte9mG3-gh212grxE_yw5iZsU7yS1rsNDWtpHFsyuuEcaHrmZy5aXF8Ipbd1SQ7iI5toKpo-pCQWtOapfzEmr0gnGl0PTDJGpub1xAP1h0Xlz8WlB5nNKNzbbvxHzTXzi27hi4c?width=700&height=609&cropmode=none)|
|Specify the disk size for the new virtual machine|[![Specify disk size](https://rscvxq.bl3302.livefilestore.com/y3mTyROs_bSHjNjVtnx36Vlexr6yd9cZokbgZ3J5x3UMgwt0H1tmj8OtUMZNYcIc-C4-lhYUBY5e1VkeRwybYzj2koWyc8IfkYmgq4ybpiZsFCGvBLjP7n3luoTRLbM6xC4iWdFK-STt21jMu58cDxEV44DRt5nQmaVJcPwFwlnTd0?width=256&height=223&cropmode=none)](https://rscvxq.bl3302.livefilestore.com/y3mTyROs_bSHjNjVtnx36Vlexr6yd9cZokbgZ3J5x3UMgwt0H1tmj8OtUMZNYcIc-C4-lhYUBY5e1VkeRwybYzj2koWyc8IfkYmgq4ybpiZsFCGvBLjP7n3luoTRLbM6xC4iWdFK-STt21jMu58cDxEV44DRt5nQmaVJcPwFwlnTd0?width=700&height=609&cropmode=none)|
|Customize the hardware|[![Customize the hardware](https://rsfkoq.bl3302.livefilestore.com/y3m66B5nXK0LIPcXiqqiA9CqNu23WyhswXWnh6b1ceSk3aPSG1vzpwosofqvGAroWdpfiJux0LUi8OE4tJBpjc8EgFxzTtY95aLS0WxHjxXJrhhHzK1SNQHKU0xQHco5PYyyWq2Ss6zEmc0c5xWY_-UT4m942_UVi6rKRgUtCqHmA0?width=256&height=223&cropmode=none)](https://rsfkoq.bl3302.livefilestore.com/y3m66B5nXK0LIPcXiqqiA9CqNu23WyhswXWnh6b1ceSk3aPSG1vzpwosofqvGAroWdpfiJux0LUi8OE4tJBpjc8EgFxzTtY95aLS0WxHjxXJrhhHzK1SNQHKU0xQHco5PYyyWq2Ss6zEmc0c5xWY_-UT4m942_UVi6rKRgUtCqHmA0?width=700&height=609&cropmode=none)|
|Allocate the RAM|[![Allocate RAM](https://rseuua.bl3302.livefilestore.com/y3mgkkZ0iK2jmIdwooQV7jLifObjFx-zJ_u_0Wjg5HSnJTIYI5mHAoxoB4Zb-5-szAT0y6T7bNLJ4LcvHdfw4DomGEJO_cL9DEO2Hao3X11GRu_R-2pzAYfxE4lZ2z9eeOkKuO4oPAIP4xPeFVdVAdV190c9_IgEFrkHKtbvGaeSRk?width=256&height=223&cropmode=none)](https://rseuua.bl3302.livefilestore.com/y3mgkkZ0iK2jmIdwooQV7jLifObjFx-zJ_u_0Wjg5HSnJTIYI5mHAoxoB4Zb-5-szAT0y6T7bNLJ4LcvHdfw4DomGEJO_cL9DEO2Hao3X11GRu_R-2pzAYfxE4lZ2z9eeOkKuO4oPAIP4xPeFVdVAdV190c9_IgEFrkHKtbvGaeSRk?width=700&height=609&cropmode=none)|
|Select the network mode|[![Select network mode](https://rschnw.bl3302.livefilestore.com/y3mXgoRCqN6PcNSdQeT-Q0L66KJ5VTJcPrYPCU_2DOGwHRqq4fd5_ME3KhwypG38er4C1ddaqNNlT2FaGNw1lH2sC5LVNK_iJJ3z6ldBjvlPGa_5GLGW6bNmpWqmDITh5aXlx0_aV7vHABiB7vqRVq_-7UHLsPsYTSfkfG3Wby00_w?width=256&height=223&cropmode=none)](https://rschnw.bl3302.livefilestore.com/y3mXgoRCqN6PcNSdQeT-Q0L66KJ5VTJcPrYPCU_2DOGwHRqq4fd5_ME3KhwypG38er4C1ddaqNNlT2FaGNw1lH2sC5LVNK_iJJ3z6ldBjvlPGa_5GLGW6bNmpWqmDITh5aXlx0_aV7vHABiB7vqRVq_-7UHLsPsYTSfkfG3Wby00_w?width=700&height=609&cropmode=none)|

Click finish to create the virtual machine.

***
### Configure Windows Installation
(The ISO used in this process was set to finnish, hence this documentation only contains finnish screenshots. When referring to elements on the screen, the documentation will include the finnish text to help you find the corresponding item/button on the screenshot.)
#### Select Language and Region
Select the desired language, region and keyboard layout and click "Next" ("Seuraava"). On the next page, click "Install Now".  

![Region And Language](https://rsegwg.bl3302.livefilestore.com/y3mK2nWv4_UNdn1FONBnmB34wMKmJrXm6y6Wf_YK1dBzkHwW9vTQXLtoliHBLqQ2PIpk00zHxVK3jh-LaIryueYaepCwAXYX7YkFSuChFIS3cGMS7SNY4GlaCBWGyIg7IVdI4twEbkvbMGgKbLDh3-Q2p5q7-ghfbOOXPwRFXC7hmU?width=1024&height=557&cropmode=none)
#### Activate Windows
Enter your license key and click "Next" ("Seuraava") or click "I don't have a product key" ("Minulla ei ole tuoteavainta") to activate Windows later on.  

![Key](https://sjxqlq.bl3302.livefilestore.com/y3mQ_EyLtgidJaFOASlrVei6NGI6XMHIStfmWxaqr6-zG7r6Q4ql8p2I25F3NgS5TDmryQfPuRmzicKwx_8mbD5XRAP8Y-KniAR9hoXC3CQ_WPbV_8FJcU_UMq_Mp6yBAbXtQAXLfhKQu5S1BuW80igrOC1AaWcpFzwzeal3qv6ApI?width=1024&height=557&cropmode=none)
#### Select Windows Version
Depending on your license key you can decide between Windows 10 Pro, Home or Education and x86 or x64 architecture. Select the version and click "Next" ("Seuraava").  

![Version](https://sjzpia.bl3302.livefilestore.com/y3mnfVETf77SiBmr-F9OJq51KqIgFBX_5BeqM7n7jrZYlCOyrTZQ0hMIrx6-5ZY8xmDXVk85ZzluhH0KGYdiAQRWR8yX1NrWqLWQGOKAyeSXLCEpv9LGAc4msqYoBbEkdLdI5TGZIooGdgZajybVyvwzDAfKzx17KqQGSXflwu6Yxs?width=1024&height=557&cropmode=none)
#### EULA
You have to (read and) accept the EULA (End-User License Agreements) before you can install Windows. Tick "I accept the license terms" ("Hyäksyn käyttöoikeussopimuksen ehdot") and click "Next" ("Seuraava").  

![EULA](https://sjwmuq.bl3302.livefilestore.com/y3meAoOQ2SZjqomdp5mFyBCc1DUrsJGRdIB8Bhavuaaq_fqXHhUdOE8HR8eoRj_YXBNYnZTzXF01K-WvuZPi7rGVX-RZQKDp2ul_na9rtDF0yHlriW4HXHAIbxpb-uLYIGBap2ttcmozezYe5BnhCEKpMK5WsuRgaHB2riuhPC-eeQ?width=1024&height=557&cropmode=none)
#### Select Installation Method
You can decide if you want to reinstall Windows keeping all files and settings from an existing installation ("Upgrade"/"Päivitys") or want a fresh install ("Custom"/"Mukautettu").  

![Method](https://sjxx3a.bl3302.livefilestore.com/y3mmE04zVlZcFj-5rxYxfaPz0HO_abZC8ng1OfvKmpK4mvSTNglaN5TveH2wYA3fXuo-OByp7yRNA8SnIehqSliSr6hLzbNq250an9aRlV8rYrfhZ9ii9mN_Rt3-4E2hcjIREw6KQe7Q9eqmFkyBdhu1Wd7C40vBNJhHlj8NgBEbvw?width=1024&height=557&cropmode=none)
#### Create Partitions
Use "New" ("Uusi") to create a new partition. Windows will automatically create a system-reserved partition (500MB) for each partition you create. However, you can delete them ("Poista") and expand ("Laajenna") your partitions to re-assign the 500MB. Select the partition you want to install Windows on and click "Next" ("Seuraava"). Windows will now start the installation.

![Partitions](https://sjwfcg.bl3302.livefilestore.com/y3moMmTCkDP7fwHPacmcY8OCgBBiTodGE29iQH7dkztTucAbibnr6rk-Dn36csOuzSY9qD8OIIHdDHEaswzROHyPYRshEV1899efYBOjZdmEelI3E7O93-2ylU0wYVgDMZu7-8Mqye3tj31lSPiXI6GFfrXdk_vwD_nx2HPgqwfos0?width=1024&height=557&cropmode=none)

### Finishing Touches
- Navigate through the Windows Customization (using "Advanced" where possible) and disable all data-sensitive options. (Eg. "Send search terms and inputs to Microsoft to improve the functionality of Cortana" or whatsoever)
- Choose between a private installation or a business installation.
- Create a local Windows account. Even if you want to use a Microsoft Account, create a local account first and connect it afterwards.
- After the virtual machine reboots, click "I Finished Installing" in VMware Workstation.
- In VMware Workstation: Navigate to Player > Manage > Install VMware Tools. It will reboot your virtual machine and load a virtual cd to the vm's drive. Execute the set-up to install the VMware Tools.
