---
category: Dictionnaires
path: '/Dictionnaires'
title: "Itération sur les éléments d'un dictionnaire"
layout: null
---

### Itération sur les valeurs

~~~ python
for value in d.values():
  print( "valeur :", value)
~~~

### Itération sur les clés

~~~ python
for key in d.keys():
  print("cle :", key )
  print("valeur :", d[key])
~~~

### Itération sur les couple clé-valeur

~~~ python
for key, value in d.items():
  print("cle :", key)
  print("valeur :", value)
~~~
