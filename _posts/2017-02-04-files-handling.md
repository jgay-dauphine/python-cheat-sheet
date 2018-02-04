---
category: Files
path: '/Files'
title: 'Gestion des fichiers'

layout: nil
---

### Ouvrir un fichier

#### La fonction open() 

```python
file_object = open("filename", "mode")
```

Les modes :
* 'r' : ouverture du fichier en lecture
* 'w' : ouverture du fichier en écriture (si le fichier existe déjà il est
  détruit)
* 'a' : ouverture du fichier en écriture et on se place à la fin

### Ecriture d'un fichier texte

```file = open("testfile.txt","w") 
 
file.write("Hello World") 
file.write("This is our new text file") 
file.write("and this is another line.") 
file.write("Why? Because we can.") 
 
file.close()```

### Lecture dans un fichier texte
```python
file = open("testfile.text", "r")
print file.read()      # Affiche tout le fichier
print file.read(5)     # Affiche les 5 premiers caractères
print file.readline()  # Affiche la première ligne
print file.readline(3) # Affiche la 3ème ligne
print file.readlines() # ['line 1', 'line 2', ..., 'last line'] 
file.close()
```
