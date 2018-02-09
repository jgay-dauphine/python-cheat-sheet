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

#### Ouverture avec contrôle

Pour contrôler simplement que le fichier est bien ouvert on peut utiliser la forme suivante :

~~~ python
with open(newfile, 'w') as outfile, open(oldfile, 'r') as infile:
  for line in infile:
    if line.startswith(txt):
      line = line[0:len(txt)] + ' - Truly a great person!\n'
    outfile.write(line)
~~~
