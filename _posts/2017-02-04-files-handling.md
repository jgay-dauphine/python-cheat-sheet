---
category: Fichiers
path: '/Fichiers'
title: 'Gestion des fichiers'
layout: null
---

### Ouvrir un fichier

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

~~~python
fileObject.close()
~~~

### Ecriture d'un fichier texte


~~~python
file = open("testfile.txt","w") 
 
file.write("Hello World") 
file.write("This is our new text file") 
file.write("and this is another line.") 
file.write("Why? Because we can.") 
 
file.close()
~~~

### Lecture dans un fichier texte

~~~python
file = open("testfile.text", "r")
print file.read()      # Affiche tout le fichier
print file.read(5)     # Affiche les 5 premiers caractères
print file.readline()  # Affiche la première ligne
print file.readline(3) # Affiche la 3ème ligne
print file.readlines() # ['line 1', 'line 2', ..., 'last line'] 
file.close()
~~~


