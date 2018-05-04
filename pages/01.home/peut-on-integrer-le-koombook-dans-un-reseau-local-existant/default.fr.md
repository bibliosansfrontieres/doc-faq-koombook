---
title: 'Peut-on intégrer le KoomBook dans un réseau local existant ?'
date: '02-05-2018 12:41'
publish_date: '02-05-2018 12:41'
taxonomy:
    category:
        - 'Configuration réseaux'
    author:
        - Florian
---

Si la structure recevant le KoomBook dispose de son propre réseau local (filaire et wifi) avec différents appareils connectés à ce dernier, il peut être intéressant d'intégrer le KoomBook à cet écosystème. Cela permet en effet, à partir de n'importe quelle machine du réseau de joindre le site http://koombook.lan

Cela n'est malheureusement pas si simple. Chaque système d'exploitation possède sa propre manière d'explorer le réseau local et de résoudre des noms de domaines (http://koombook.lan -> 192.168.0.48) afin de les associer à des adresse IP.

Il existe donc un système natif pour presque chaque système d'exploitation: 
* Bonjour pour Mac
* Avahi pour Linux 
* ZeronConf/Bonjour pour Windows
* Android n'en possède aucun !

Android est massivement utilisé à travers le monde et dans les projets que nous menons, malgré cela nous ne pourrons pas **facilement** intégrer le KoomBook dans un réseau local. il faudra recourir à l'intervention d'un technicien qualifié pour aider le système Android à trouver facilement grâce à la résolution DNS (Rappel : association de http://koombook.lan à l'adresse 192.168.0.48) des appareils sur le réseau local.

Vous trouverez plus d'informations sur [l'intégration dans un réseau local](https://bsf.gitbooks.io/formation-koombook/content/fr/deploiement_dans_un_reseau_local.html) sur le GitBook du cycle de Formation KoomBook.