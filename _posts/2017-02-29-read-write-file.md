---
category: Fichiers
path: '/Fichiers'
title: 'Ecritre/Lecture dans un fichier'
layout: null
---

### Ecriture d'un fichier texte

~~~ python
file = open("testfile.txt","w") 
 
file.write("Hello World") 
file.write("This is our new text file") 
file.write("and this is another line.") 
file.write("Why? Because we can.") 
 
file.close()
~~~

### Lecture dans un fichier texte

~~~ python
file = open("testfile.text", "r")
print file.read()      # Affiche tout le fichier
print file.read(5)     # Affiche les 5 premiers caractères
print file.readline()  # Affiche la première ligne
print file.readline(3) # Affiche la 3ème ligne
print file.readlines() # ['line 1', 'line 2', ..., 'last line'] 
file.close()
~~~
