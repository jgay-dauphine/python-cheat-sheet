---
category: Fichiers
path: '/Fichiers'
title: 'Ouverture/Fermeture de fichier'
layout: null
---

### Ouverture et fermeture d'un fichier

#### La fonction open() 

Elle permet d'ouvrir un fichier et de récupérer un descripteur pour le fichier.
C'est ce descripteur que nous utiliserons pour lire ou écrire dans le fichier.


~~~ python
fileObject = open("filename", "mode")
~~~

Les modes :
* 'r' : ouverture du fichier en lecture
* 'w' : ouverture du fichier en écriture (si le fichier existe déjà il est
  détruit)
* 'a' : ouverture du fichier en écriture et on se place à la fin

#### La fonction close()

Elle permet de fermer un fichier et effectue réellement les écritures dans le
fichier.

~~~ python
fileObject.close()
~~~


