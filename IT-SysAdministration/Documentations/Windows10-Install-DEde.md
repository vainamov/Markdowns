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
(Für diese Dokumentation wurde eine finnischsprachige ISO verwendet. Die Screenshots enthalten daher ausschließlich finnische Texte. Zum besseren Verständnis werden hier bei Verweisen auf UI Elemente die finnischen Bezeichnungen mit angegeben.)
#### Sprache und Region wählen
Die gewünschte Sprache und Region, sowie das gewünschte Tastaturlayout auswählen und auf "Weiter" ("Seuraava") klicken.  

![Region And Language](https://rsegwg.bl3302.livefilestore.com/y4mmUjIrmrNXvnvFFaOSkRAeY9DTCp70t41dlMz4rfOynk2BH8X5TaRr2HZM0foc5bJTEJXfvpc5JiQrccyx33k1vBJz75nk_EXWhQ245uV6xuqep6vHjEzyxUR2zlip-aEPcw4lNOyY5R-W3x1wt0Hi7lJOjJbxZQKgVbflXm450o7yDObOD9AsWO-P5lIb8qxihjKq4Ol2e6JW9PxP8_uLw?width=619&height=458&cropmode=none)
#### Aktivierung
Entweder den Lizenzschlüssel eingeben (sofern vorhanden) und mit "Weiter" ("Seuraava") bestätigen, oder "Ich habe keinen Produkt Key" ("Minulla ei ole tuoteavainta") auswählen um die Aktivierung später durchzuführen.  

![Key](https://sjxqlq.bl3302.livefilestore.com/y4mHOpNByZQYsm1fKTo7lfkPabqQ5g7GVy7SgmKnamFnmpJiDtTcsiwyFXYO9RKoiDD6gUUlKldApE8zvUTG5j3SDL6awvSinmrGc8WOIdh7u4sriSkIX3D0RX3qDgTq-LAYqYfWRD2H4k7FJXfduYalbToVS3WrEdsvjaCZJNq5JbUzm7n33jRLpAiZZZNjpt8tuRqMMR41Z8O54WmazEiUw?width=641&height=483&cropmode=none)
#### Windows Version wählen
In Abhängigkeit von der ISO und dem Lizenzschlüssel stehen die Versionen Windows 10 Pro, Home oder Education, sowie die jeweiligen x86 bzw. x64 Architekturen zur Verfügung. Die gewünschte Version auswählen und mit "Weiter" ("Seuraava") bestätigen.  

![Version](https://sjzpia.bl3302.livefilestore.com/y4mbEz5wByks-EZzwBerV8RiERcdDpcZyFCwe9pPBDkmGP4mudYXe2nCD0mc-wSTdKuAl-Vl-SAtwY1bWTVs26AdM7kHbnZ9BsC3q8tF-UNJLxFguuXENkjGs1E5wyJwTbnso7UrtTUN4AQcHpWO8eQ6vA8WeXIfJb1yJO1cZkqqIs94I4aYwzMEOM1Xqlcd8buGYugTXHWYV51bodONEwo_Q?width=641&height=483&cropmode=none)
#### EULA
Bevor die Windows Installation gestartet werden kann, muss die EULA (Endbenutzer-Lizenzvereinbarung) (gelesen und) bestätigt werden. Mit "Ich akzeptiere die Lizenzbedingungen" ("Hyäksyn käyttöoikeussopimuksen ehdot") bestätigen und "Weiter" ("Seuraava") klicken.  

![EULA](https://sjwmuq.bl3302.livefilestore.com/y4mgqmnAi4St0ZkfwIRDjBB0hLd66wtCGTlcYOVF7ABrVryZnK8qf5c5rVAjDwMyqsf3acYqewUldmTj19mILlx-NjLwXisYLUitYXpJ_8igaD3PX8DyOfYo6ea163dyHpWa78xtaqVbK-5fFyz9eNvsfQM5fBnx0bWkUJtF8q3SZcexxdiyJKz-d9pIMRCqgQ7cLPOuR0be4FOYiDit20JLQ?width=641&height=481&cropmode=none)
#### Installationsmethode wählen
Es gibt die Möglichkeit Windows neu zu installieren und dabei alle Dateien zu behalten ("Upgrade"/"Päivitys") oder einen sogenannten "Fresh-Install" durchzuführen. Hierbei werden alle Dateien auf der Festplatte gelöscht. ("Benutzerdefiniert"/"Mukautettu").  

![Method](https://sjxx3a.bl3302.livefilestore.com/y4mSvE-E3vv0z85NGon6Mg_DtDDyzulP1p_fXtncLJyb5XkKdzCIfCvVZahtkVS26MHF0DzV4sL39WvDvkWEzn0n8VurThhhl9h9MFdYwgVQuK9VR4KDmjH2tZk_reXO8bCzmmY5h9NEADbZIbkkI1FtSmvmFQ3j4o9jO6WilJowBw9QtEJziiWv6IZuIkyTeqlYAMtBc-YLHk2h7aQ4MDttg?width=640&height=479&cropmode=none)
#### Partitionen erstellen
Mit "Neu" ("Uusi") werden neue Partitionen erstellt. Windows wird hierbei automatisch eine system-reservierte Partition (500MB) für jeder erstelle Partition anlegen. Allerdings lassen sich diese löschen ("Poista") und die bestehenden Partitionen erweitern ("Laajenna") um die 500MB neu zu vergeben. Mit einem Klick auf die gewünschte Installationspartition und "Weiter" ("Seuraava") beginnt Windows mit der Installation.

![Partitions](https://sjwfcg.bl3302.livefilestore.com/y4m3652mOZAXYAdHBZu1NLbRUKOPg4UrV7t5MDSvbQA4xb_p9rQCHnJ2s376HytyazIgjt-IaJlHga8bJ7zWiSfM7zCSYIKUmoodGLCqmBsHveV3FEjG1WQmVBghzyljmvIZGpCX_AZ5pd6-9zy2psHOQhE9UBG83p4PUYVGupo8-yOJFbmsth-mnYU9Eup-ijJ5dVHsMGkMfyPdhHCgpCrwQ?width=640&height=480&cropmode=none)

### Abschließen
- Beim Konfigurieren von Windows ("Angepasst" wo möglich wählen) sollten alle Datenschutz-relevaten Optionen deaktiviert werden.
- Es sollte zwischen einer privaten und einer Business Installation entschieden werden.
- Es sollte immer zu erst ein lokaler Account erstellt werden. Selbst wenn die Verwendung eines Microsoft Accounts geplant ist, sollte erst ein lokaler Account erstellt werden und dieser dann mit dem Microsoft Account verbunden werden.
- Nach dem Neustart der VM "I Finished Installing" in VMware Workstation auswählen.
- In VMware Workstation: Nach "Player > Manage > Install VMware Tools" navigieren. Die virtuelle Maschine wird daraufhin neustarten und ein Setup für die VMware Tools in das Laufwerk der VM laden.
