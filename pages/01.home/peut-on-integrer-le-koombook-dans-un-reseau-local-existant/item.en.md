---
title: 'Can I integrate the KoomBook to an existing local network?'
date: '02-05-2018 12:41'
publish_date: '02-05-2018 12:41'
taxonomy:
    category:
        - 'Network Configuration'
    author:
        - Florian
---

If the structure receiving the KoomBook has its own local network (either fiber or WiFi) with different devices connected to it, it could be useful to integrate the KoomBook to this system.  This would, in effect, permit any machine in the network to access http://koombook.lan.  

Unfortunately, it is not that symple.  Each operating system has its own manner of exploring local networks and sorting domain names (http://koombook.lan -> 192.168.0.48) to associate them with local IP addresses.

You thus need to make use of a native system.  There is a native system for almost every operating system: 
* Bonjour for Mac
* Avahi for Linux 
* ZeronConf/Bonjour for Windows
* Android does not have one!

Android is very popular and used a lot around the world and in projects that we lead.  However, we cannot **easily** integrate the KoomBook into a local network.  You thus need to resort to hiring a qualified technician to help the Android system find devices on the local network through the DNS resolution (remember http://koombook.lan is associated with 192.168.0.48).

You can find more information about [integration with a local network](https://bsf.gitbooks.io/formation-koombook/content/fr/deploiement_dans_un_reseau_local.html) on GitBook for the KoomBook teaching guide.