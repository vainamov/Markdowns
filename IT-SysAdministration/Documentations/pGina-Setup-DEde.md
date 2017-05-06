## pGina Setup Dokumentation

#### Vorraussetzungen
- mind. Windows 7
- konfigurierter LDAP Server
- pGina (https://github.com/pgina/pgina/releases)
> Warnung: Es wird empfohlen einen Sicherungspunkt zu erstellen bzw. eine Testinstallation in einer virtuellen Maschine durchzuführen.

#### Technische Daten
|Betriebssystem|pGina Version|
|---|---|
|Windows 10 Pro x86<br/>(Version 1607 Build 14393.953)<br/>FI-fi<br />3.02GB RAM / 70GB ROM|pGina 3.1.8.0|

***
### pGina konfigurieren
#### Plugins aktivieren
Den Tab "Plugin Selection" öffnen und einen Haken bei "Authentication", "Authorization" und "Gateway" setzen, sowohl für das LDAP Plugin als auch für das Local Machine Plugin.  

![Plugin](https://sjwtzq.bl3302.livefilestore.com/y4mJPx0WRL9v3788HAD_9P7eVlqdK2O6N3eUsdudm6f1mJcm4BYfqxn3fhZhR4QD8Vdl0mD_fLGc_SuXaxTjQuHs6u11isZnZSvaihWEJ_vlUjYFPFL1DV9_2tx67moirwPfqP6lYfXH9RS8FIrUU1stpnOu29zM6z9FY_9V27oiU7402gYOYKU35AsD_gpICR9krSKfi05sVBwPSJl4szCEQ?width=825&height=669&cropmode=none)  

#### Plugin Reihenfolge anpassen
Den Tab "Plugin Order" öffnen und mit Hilfe der Pfeil-Buttons sicherstellen, dass das LDAP Plugin an erster Stelle in "Authorization" und "Gateway" steht, aber in "Authentication" an letzter Stelle.  

![Plugin](https://sjzi2q.bl3302.livefilestore.com/y4mvUpQwc-rk1b6WCpfif9Ii1wI1VLaclS7LJwW5JEibWa0LwkZMmcBpgEmG0XHHqgNO20fIrokA4Rwv-ibUecO2yATDJ03ILgi5PDdTCkAjKwiK2yae2xASe0VFR38lUgWdZPr9aSVvvNf7Xl9spkTwPXMGOm4JrnyQ-RIrXNYIj3D_j7ZaVslvNUwH4yJrK1hicscQpsiGdSfelKo-1UA6A?width=825&height=671&cropmode=none)  

#### LDAP Plugin konfigurieren
(In Abhängigkeit der LDAP Konfiguration und der verwendeten Server Software können die Angaben in den folgenden Schritten abweichen.)  
Im Tab "Plugin Selection" einen Doppelklick auf das LDAP Plugin machen um die Einstellungen zu öffnen.  

![Plugin](https://sjzwzw.bl3302.livefilestore.com/y4mAYEvx4Ahky5KWpD_chdEO8zaSzfm0njvQpuuN1pbhlD6pMPlVlngPokmmMfkdG1PXBAnWuHeX_2ok_cIN8HBuJOyDZpBBKJh5icBf8JY_4Q1-DJHi4TJfGmBMMbVzWl-5d0VtIHXk51rYf4WkYGRu4Pw5VgE1ADZLWm3SzgDRvnxVDRnRBqavdbhZ8nI2ZEGli52r_XEVlRGL8ZhKjZM_Q?width=702&height=534&cropmode=none)

#### Authentication
Für einen LDAP Server mit der Adresse `10.60.20.251:1389` und folgender Struktur:
- dc=ldap,dc=festival,dc=ml
  - ou=groups
    - cn=Administrators
    - cn=Users
  - ou=members
    - uid=user1
    - uid=user2
    - uid=...
  
sollte die Konfiguration so aussehen wie auf dem Screenshot. Nichtsdestotrotz, je nach verwendeter Server Software muss das "Member Attribute" evtl. zu `memberUid` geändert werden und/oder das "User DN Pattern" mit `cn=%u,` beginnen.

#### Authorization
Im Authorization Tab können Einstellungen zur Vergabe von Rechten vorgenommen werden. Die [pGina Dokumentation](http://pgina.org/docs/v3.1/ldap.html) enthält im Abschnitt "Authorization Options" ausführlichere Infos.  

#### Gruppen-Mapping (Gateway)
Der "Gateway" Tab stellt Einstellungen bereit, um LDAP Benutzer anhand ihrer LDAP Gruppen lokalen Gruppen zuzuweisen.  

![Plugin](https://sjw78w.bl3302.livefilestore.com/y4m4AV0uDn-O4GQ_Ff6NG3naMAMKZeiTl7O1-AEyIIpHJfCO3Q-_Qzan2lfeeWW8mZFACh6tEy0JKM3c5LXxcee83REABLxZ9Z0jjEEQmMMj1xg3ewTMkxjEuUk4G4tNKARG6z7gp2gewJL7VBlV1NfKNFPGUAAmgxN6IAmam9Qj4Vtc17pCFBGDe4qQYDxD3FK9GFPFedw1ug62ukM0oOPHg?width=703&height=313&cropmode=none)  

> Warnung: Die lokalen Gruppennamen müssen 100% übereinstimmen. Eine Liste aller lokalen Gruppen und ihrer exakten Schreibweise liefert der `net localgroup`-Command. (`WIN+R` > `cmd` > `ENTER` > `net localgroup` > `ENTER`). Der Command erzeugt eine Ausgabe ähnlich der des folgenden Screenshots.  

![Plugin](https://dz6qlg.bl3302.livefilestore.com/y4mhBva97CJTCbSk6pUoqFzIkZccUDCUsJOMUIkPOnXwb6f4MXafvUMgmz3GO7tnK8WA_hQ6Aqp6TA8QbvOUPSw5suEO-ewzq6K52dWC0X0-L41jmt3NpsKU6JqnY4bU7wdknGPYQHR61BAERKiSZUmqVRwU_Orvm0I4_D9tTgoqwqknWoQfTbkFZWQ5Ck9mlGq8iK-wYppSx9eDgAun_VwjA?width=660&height=347&cropmode=none)  

Um die Änderungen zu übernhemen muss "Save" geklickt werden **und** "Apply" in pGina, da sonst die Änderungen nur in pGina gespeichert werden werden aber nicht in der Registry übernommen werden.  

***
### Testen der Konfiguration
Es stehen 2 Möglichkeiten zum Testen der Einstellungen zur Verfügung. Zum einen, kann die in pGina integrierte Simulation benutzt werden oder der umständlichere Weg über Ab- und Anmelden.
  
***
### Troubleshooting
Gesetz des Falles das beim Testen Fehler auftreten sollten, stehen verschiedene Hilfen bereit. Zuallererst sollte der Simulationslog gesichtet werden ("Show Log" Button im Simulation Tab). In der Regel stellt dieser ausreichend Informationen bereit um die Fehlerquelle eindeutig zu identifizieren. Sollte dies nicht ausreichen um das Problem zu beheben, empfiehlt es sich die [geschlossenen Issues in der pGina Repository](https://github.com/pgina/pgina/issues?q=is%3Aissue+is%3Aclosed) anzusehen, eventuell trat eben jenes Problem bereits in der Vergangenheit auf und wurde bereits gelöst. Sollte wider Erwarten das Problem dort nicht aufgeführt sein, muss [ein neuer Issue erstellt](https://github.com/pgina/pgina/issues/new) werden. Hierbei sollte das Problem so detailiert wie möglich beschrieben werden und auch der Simulationslog angehängt werden.
  
***
### Abschließen
- Mit einem Doppelklick auf das Locale Machine Plugin im "Plugin Selection" Tab lässt sich die Option "Remove account and profile after logout when account does not exist prior to logon." aktivieren. Infolgedessen wird Windows nach dem Abmelden den von pGina erstellten Benutzerordner wieder entfernen und so verhindern, dass der `C:\Users\`-Ordner überfüllt wird.
- Im "General" Tab lässt sich überdies das Aussehen des pGina Services anpassen. Es besteht die Möglichkeit ein Bild festzulegen sowie eine MOTD (message of the day) und eine Nachricht beim Verbinden anzuzeigen.
  
***
### Automatisches Drive Mapping
Ab der [3.2.1.1 Beta](https://github.com/pgina/pgina/releases/tag/v3.2.1.1) enthält pGina das "Drive Mapper" Plugin. Es ermöglicht beim Anmelden automatisch Netzwerklaufwerke einbinden zu lassen (z.B. ein Home Verzeichnis auf einem NAS). Sofern der Einsatz von Stable Releases präferiert wird, besteht die Möglichkeit das Plugin alleine in die bestehende pGina Installtion einzubinden, indem man die `.dll` im Plugin Verzeichnis von pGina (`C:\Program Files\pGina\Plugins\Core\`) ablegt.  

![Plugin](https://dz50rq.bl3302.livefilestore.com/y4mSqh1KqdBCg_cflJAUyekxXWHxcM1ShKWQf5EM8zhBLPivVOBwGQlAUOw9be7eBkKwj5pYtk3cTOAeaFj0HZa48QBWjSK6jg-xjSEuq2qEAJgeU5STtgAOYHAuUZY8uysUr6nmnGvvQHMvcBMAU0qKd7h-PgvJHPLSnWV--tuqECGqRsmbs-tiQHiqa4G3Lc4IheIDNTLRcLWKlACnvx-7A?width=825&height=622&cropmode=none)
