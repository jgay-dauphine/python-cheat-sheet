---
category: Fichiers
path: '/Fichiers'
title: 'Gestion des chemins de fichiers'
layout: null
---

### Construction d'un chemin

Pour gérer les chemins de fichiers il est plus simple (et protable) d'utiliser l'utilitaire path de la
bibliothèque os :

~~~ python
import os

path = os.path.join("c:\\", "repertoire", "sous-repertoire", "fichier")
~~~

### Récupération du répertoire dans un path

~~~ python
import os

directory = os.path.dirname(file_path)
~~~
