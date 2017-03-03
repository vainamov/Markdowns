## Windows 10 Installation Documentation

#### Host
|OS|Specs|Virtualization Software|
|---|---|---|
|Windows 10 Pro x64<br/>(10.0.14393 Build 14393)<br/>DE-de|Lenovo B71-80 80RJ00HMGE<br/>Intel Core i7-6500U, 8GB DDR3L SDRAM <br/> AMD Radeon M330 2GB 17,3"<br/>1TB Seagate ST1000LM024/HN-M101MBB|VMware® Workstation 12 Player<br/>(12.5.2 build-4638234)|

#### Virtual Machine
|OS|Specs|
|---|---|
|Windows 10 Pro x86<br/>(10.0.14393 Koontikäännös 14393)<br/>FI-fi|3.02Gt RAM / 70Gt ROM|

### Download Windows ISO
https://www.microsoft.com/de-de/software-download/windows10

### Download VMware® Workstation Player
https://my.vmware.com/de/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/12_0

### Configure The Virtual Machine
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

### Configure The Windows Installation
