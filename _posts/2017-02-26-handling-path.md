---
category: Fichiers
path: '/Fichiers'
title: 'Gestion des chemins de fichiers'
layout: null
---

### Gestion des chemins de fichiers

Pour gérer les chemins de fichiers il est plus simple (et protable) d'utiliser l'utilitaire path de la
bibliothèque os :

~~~ python
import os

path = os.path.join("c:\\", "repertoire", "sous-repertoire", "fichier")
~~~
