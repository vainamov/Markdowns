## Windows 10 Installation Dokumentation

#### Host
|Betriebssystem|Technische Daten|Virtualisierungs Software|
|---|---|---|
|Windows 10 Pro x64<br/>(Version 1703 Build 15063.138)<br/>DE-de|Lenovo B71-80 80RJ00HMGE<br/>Intel Core i7-6500U, 8GB DDR3L SDRAM <br/> AMD Radeon M330 2GB 17,3"<br/>1TB Seagate ST1000LM024/HN-M101MBB|VMware® Workstation 12 Player<br/>(12.5.2 build-4638234)|

#### Virtuelle Maschine
|Betriebssystem|Technische Daten|
|---|---|
|Windows 10 Pro x86<br/>(Version 1607 Build 14393.953)<br/>FI-fi|3.02GB RAM / 70GB ROM|

***
### Download Windows ISO
https://www.microsoft.com/de-de/software-download/windows10

### Download VMware® Workstation Player
https://my.vmware.com/de/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/12_0

***
### Virtuelle Maschine konfigurieren
|Schritt|Screenshot<br/>(Anklicken für größere Ansicht)|
|---|---|
|Neue virtuelle Maschine erstellen|[![Create a new virtual machine](https://rsfd8g.bl3302.livefilestore.com/y3mHdrvMLRKPsYk4E8zJxl-2mTzRdXbWMdWpKSqYCIcg5pTU7WA-T26YMNSvO5aRn5nc2r3vBAL8dt2YXrCUcPPTNZ0cMGeJN3B47Idly_-tZ8HN1bf1YkRIyRGCZkEpQvdSdg4iYjq3dO9DYQSlvlnOPT5Q8SYlMxv7S_wVpL8uTk?width=256&height=223&cropmode=none)](https://rsfd8g.bl3302.livefilestore.com/y3mHdrvMLRKPsYk4E8zJxl-2mTzRdXbWMdWpKSqYCIcg5pTU7WA-T26YMNSvO5aRn5nc2r3vBAL8dt2YXrCUcPPTNZ0cMGeJN3B47Idly_-tZ8HN1bf1YkRIyRGCZkEpQvdSdg4iYjq3dO9DYQSlvlnOPT5Q8SYlMxv7S_wVpL8uTk?width=700&height=609&cropmode=none)|
|Windows 10 ISO auswählen|[![Select Windows ISO file](https://rsdlrg.bl3302.livefilestore.com/y3mnsWAHa-_64uc1P42azPxgEOAqc_7Joc9rP_nluYLbknoo4bDBwBKmXhHvjLdG-X3Yhpk5AYtgZUiKP71DLQlWzphKbs_F4b6ViQAPiZHNz3sNu_Mey36M9-XmUmiQaq_KNqBCaMApIvthsGbdMjmCe3V7An6aQqTzJ9TFwW6XlQ?width=256&height=223&cropmode=none)](https://rsdlrg.bl3302.livefilestore.com/y3mnsWAHa-_64uc1P42azPxgEOAqc_7Joc9rP_nluYLbknoo4bDBwBKmXhHvjLdG-X3Yhpk5AYtgZUiKP71DLQlWzphKbs_F4b6ViQAPiZHNz3sNu_Mey36M9-XmUmiQaq_KNqBCaMApIvthsGbdMjmCe3V7An6aQqTzJ9TFwW6XlQ?width=700&height=609&cropmode=none)|
|Namen und Speicherort der VM festlegen|[![Select vm name and location](https://rscofg.bl3302.livefilestore.com/y3mHhxH8CrHWcJLRpXFM36tWyopuHaN2wn8-4borte9mG3-gh212grxE_yw5iZsU7yS1rsNDWtpHFsyuuEcaHrmZy5aXF8Ipbd1SQ7iI5toKpo-pCQWtOapfzEmr0gnGl0PTDJGpub1xAP1h0Xlz8WlB5nNKNzbbvxHzTXzi27hi4c?width=256&height=223&cropmode=none)](https://rscofg.bl3302.livefilestore.com/y3mHhxH8CrHWcJLRpXFM36tWyopuHaN2wn8-4borte9mG3-gh212grxE_yw5iZsU7yS1rsNDWtpHFsyuuEcaHrmZy5aXF8Ipbd1SQ7iI5toKpo-pCQWtOapfzEmr0gnGl0PTDJGpub1xAP1h0Xlz8WlB5nNKNzbbvxHzTXzi27hi4c?width=700&height=609&cropmode=none)|
|Festplattengröße festlegen|[![Specify disk size](https://rscvxq.bl3302.livefilestore.com/y3mTyROs_bSHjNjVtnx36Vlexr6yd9cZokbgZ3J5x3UMgwt0H1tmj8OtUMZNYcIc-C4-lhYUBY5e1VkeRwybYzj2koWyc8IfkYmgq4ybpiZsFCGvBLjP7n3luoTRLbM6xC4iWdFK-STt21jMu58cDxEV44DRt5nQmaVJcPwFwlnTd0?width=256&height=223&cropmode=none)](https://rscvxq.bl3302.livefilestore.com/y3mTyROs_bSHjNjVtnx36Vlexr6yd9cZokbgZ3J5x3UMgwt0H1tmj8OtUMZNYcIc-C4-lhYUBY5e1VkeRwybYzj2koWyc8IfkYmgq4ybpiZsFCGvBLjP7n3luoTRLbM6xC4iWdFK-STt21jMu58cDxEV44DRt5nQmaVJcPwFwlnTd0?width=700&height=609&cropmode=none)|
|Hardware konfigurieren|[![Customize the hardware](https://rsfkoq.bl3302.livefilestore.com/y3m66B5nXK0LIPcXiqqiA9CqNu23WyhswXWnh6b1ceSk3aPSG1vzpwosofqvGAroWdpfiJux0LUi8OE4tJBpjc8EgFxzTtY95aLS0WxHjxXJrhhHzK1SNQHKU0xQHco5PYyyWq2Ss6zEmc0c5xWY_-UT4m942_UVi6rKRgUtCqHmA0?width=256&height=223&cropmode=none)](https://rsfkoq.bl3302.livefilestore.com/y3m66B5nXK0LIPcXiqqiA9CqNu23WyhswXWnh6b1ceSk3aPSG1vzpwosofqvGAroWdpfiJux0LUi8OE4tJBpjc8EgFxzTtY95aLS0WxHjxXJrhhHzK1SNQHKU0xQHco5PYyyWq2Ss6zEmc0c5xWY_-UT4m942_UVi6rKRgUtCqHmA0?width=700&height=609&cropmode=none)|
|RAM zuweisen|[![Allocate RAM](https://rseuua.bl3302.livefilestore.com/y3mgkkZ0iK2jmIdwooQV7jLifObjFx-zJ_u_0Wjg5HSnJTIYI5mHAoxoB4Zb-5-szAT0y6T7bNLJ4LcvHdfw4DomGEJO_cL9DEO2Hao3X11GRu_R-2pzAYfxE4lZ2z9eeOkKuO4oPAIP4xPeFVdVAdV190c9_IgEFrkHKtbvGaeSRk?width=256&height=223&cropmode=none)](https://rseuua.bl3302.livefilestore.com/y3mgkkZ0iK2jmIdwooQV7jLifObjFx-zJ_u_0Wjg5HSnJTIYI5mHAoxoB4Zb-5-szAT0y6T7bNLJ4LcvHdfw4DomGEJO_cL9DEO2Hao3X11GRu_R-2pzAYfxE4lZ2z9eeOkKuO4oPAIP4xPeFVdVAdV190c9_IgEFrkHKtbvGaeSRk?width=700&height=609&cropmode=none)|
|Netzwerkmodus auf "Bridged" setzen|[![Select network mode](https://rschnw.bl3302.livefilestore.com/y3mXgoRCqN6PcNSdQeT-Q0L66KJ5VTJcPrYPCU_2DOGwHRqq4fd5_ME3KhwypG38er4C1ddaqNNlT2FaGNw1lH2sC5LVNK_iJJ3z6ldBjvlPGa_5GLGW6bNmpWqmDITh5aXlx0_aV7vHABiB7vqRVq_-7UHLsPsYTSfkfG3Wby00_w?width=256&height=223&cropmode=none)](https://rschnw.bl3302.livefilestore.com/y3mXgoRCqN6PcNSdQeT-Q0L66KJ5VTJcPrYPCU_2DOGwHRqq4fd5_ME3KhwypG38er4C1ddaqNNlT2FaGNw1lH2sC5LVNK_iJJ3z6ldBjvlPGa_5GLGW6bNmpWqmDITh5aXlx0_aV7vHABiB7vqRVq_-7UHLsPsYTSfkfG3Wby00_w?width=700&height=609&cropmode=none)|

Auf "Finish" klicken um die Einrichtung abzuschließen.

***
### Windows Installation konfigurieren
(Für diese Dokumentation wurde eine finnischsprachige ISO verwendet. Die Screenshots enthalten daher ausschließlich finnische Texte. Zum besseren Verständnis, werden hier bei Verweisen auf die Screenshots die finnischen Bezeichnungen mit angegeben.)
#### Sprache und Region wählen
Die gewünschte Sprache und Region, sowie das gewünschte Tastaturlayout auswählen und auf "Weiter" ("Seuraava") klicken.  

![Region And Language](https://rsegwg.bl3302.livefilestore.com/y3mK2nWv4_UNdn1FONBnmB34wMKmJrXm6y6Wf_YK1dBzkHwW9vTQXLtoliHBLqQ2PIpk00zHxVK3jh-LaIryueYaepCwAXYX7YkFSuChFIS3cGMS7SNY4GlaCBWGyIg7IVdI4twEbkvbMGgKbLDh3-Q2p5q7-ghfbOOXPwRFXC7hmU?width=1024&height=557&cropmode=none)
#### Aktivierung
Entweder den Lizenzschlüssel eingeben (sofern vorhanden) und mit "Weiter" ("Seuraava") bestätigen, oder "Ich habe keinen Produkt-Key" ("Minulla ei ole tuoteavainta") auswählen um die Aktivierung später durchzuführen.  

![Key](https://sjxqlq.bl3302.livefilestore.com/y3mQ_EyLtgidJaFOASlrVei6NGI6XMHIStfmWxaqr6-zG7r6Q4ql8p2I25F3NgS5TDmryQfPuRmzicKwx_8mbD5XRAP8Y-KniAR9hoXC3CQ_WPbV_8FJcU_UMq_Mp6yBAbXtQAXLfhKQu5S1BuW80igrOC1AaWcpFzwzeal3qv6ApI?width=1024&height=557&cropmode=none)
#### Windows Version wählen
In Abhängigkeit vom Lizenzschlüssel stehen die Versionen Windows 10 Pro, Home oder Education, sowie die jeweiligen x86 bzw. x64 Architekturen zur Verfügung. Die gewünschte Version auswählen und mit "Weiter" ("Seuraava") bestätigen.  

![Version](https://sjzpia.bl3302.livefilestore.com/y3mnfVETf77SiBmr-F9OJq51KqIgFBX_5BeqM7n7jrZYlCOyrTZQ0hMIrx6-5ZY8xmDXVk85ZzluhH0KGYdiAQRWR8yX1NrWqLWQGOKAyeSXLCEpv9LGAc4msqYoBbEkdLdI5TGZIooGdgZajybVyvwzDAfKzx17KqQGSXflwu6Yxs?width=1024&height=557&cropmode=none)
#### EULA
Bevor die Windows Installation gestartet werden kann muss die EULA (Endbenutzer-Lizenzvereinbarung) (gelesen und) bestätigt werden. Mit "Ich habe die EULA gelesen und akzeptiert" ("Hyäksyn käyttöoikeussopimuksen ehdot") bestätigen und "Weiter" ("Seuraava") klicken.  

![EULA](https://sjwmuq.bl3302.livefilestore.com/y3meAoOQ2SZjqomdp5mFyBCc1DUrsJGRdIB8Bhavuaaq_fqXHhUdOE8HR8eoRj_YXBNYnZTzXF01K-WvuZPi7rGVX-RZQKDp2ul_na9rtDF0yHlriW4HXHAIbxpb-uLYIGBap2ttcmozezYe5BnhCEKpMK5WsuRgaHB2riuhPC-eeQ?width=1024&height=557&cropmode=none)
#### Installationsmethode wählen
Es gibt die Möglichkeit Windows neu zu installieren und dabei alle Dateien zu behalten ("Upgrade"/"Päivitys") oder einen sogenannten "Fresh-Install" durchzuführen. Hierbei werden alle Dateien auf der Festplatte gelöscht. ("Angepasst"/"Mukautettu").  

![Method](https://sjxx3a.bl3302.livefilestore.com/y3mmE04zVlZcFj-5rxYxfaPz0HO_abZC8ng1OfvKmpK4mvSTNglaN5TveH2wYA3fXuo-OByp7yRNA8SnIehqSliSr6hLzbNq250an9aRlV8rYrfhZ9ii9mN_Rt3-4E2hcjIREw6KQe7Q9eqmFkyBdhu1Wd7C40vBNJhHlj8NgBEbvw?width=1024&height=557&cropmode=none)
#### Partitionen erstellen
Mit "Neu" ("Uusi") werden neue Partitionen erstellt. Windows wird hierbei automatisch eine system-reservierte Partition (500MB) für jeder erstelle Partition anlegen. Allerdings lassen sich diese löschen ("Poista") und die bestehenden Partitionen erweitern ("Laajenna") um die 500MB neu zu vergeben. Mit einem Klick auf die gewünschte Installationspartition und "Weiter" ("Seuraava") beginnt Windows mit der Installation.

![Partitions](https://sjwfcg.bl3302.livefilestore.com/y3moMmTCkDP7fwHPacmcY8OCgBBiTodGE29iQH7dkztTucAbibnr6rk-Dn36csOuzSY9qD8OIIHdDHEaswzROHyPYRshEV1899efYBOjZdmEelI3E7O93-2ylU0wYVgDMZu7-8Mqye3tj31lSPiXI6GFfrXdk_vwD_nx2HPgqwfos0?width=1024&height=557&cropmode=none)

### Abschließen
- Beim Konfigurieren von Windows ("Benutzerdefiniert" wo möglich wählen) sollten alle Datenschutz-relevaten Optionen deaktiviert werden.
- Es sollte zwischen einer privaten und einer Business Installation.
- Es sollte immer zu erst ein lokaler Account erstellt werden. Selbst wenn die Verwendung eines Microsoft Accounts geplant ist, sollte erst ein lokaler Account erstellt werden und dann mit dem Microsoft Account verbunden werden.
- Nachdem dem Neustart der VM "I Finished Installing" in VMware Workstation auswählen.
- In VMware Workstation: Nach Player > Manage > Install VMware Tools navigieren. Die virtuelle Maschine wird daraufhin neustarten und ein Setup für die VMWare Tools in das Laufwerk der VM laden.
