---
category: Dictionnaires
path: '/Dictionnaires'
title: 'Créer un dictionnaire'
layout: null
---

### Qu'est-ce qu'un dictionnaire

Les dictionnaires sont les tableaux associatifs de python, ils permettent d'associer des valeurs à des clés qui ne sont pas
forcément des entiers. C'est une technique simple et efficace pour stocker des données.

### Création d'un dictionnaire

~~~ python
d = dict()

d["key"] = value
d["key2"] = value2
~~~

~~~ python
d = { "key": value, "key2": value2 }
~~~

### Création à partir de deux listes de même taille

~~~ python
>>> l = '123456789'
>>> c = 'ABCDEFGHI'
>>> dict(zip(l,c))
{'8': 'H', '6': 'F', '3': 'C', '5': 'E', '9': 'I', 
'7': 'G', '1': 'A', '4': 'D', '2': 'B'}
>>> dict(zip(c,l))
{'G': '7', 'F': '6', 'C': '3', 'I': '9', 'E': '5', 
'A': '1', 'H': '8', 'B': '2', 'D': '4'}
~~~

### Supprimer un couple clé-valeur

deux méthodes :
* utiliser la suppresion globale 'del'
* utiliser la fonction 'pop(key)' des dictionnaires

~~~ python
>>> del d[2]
>>> d
{'key': 2}
~~~

~~~ python
>>> d.pop('key')
2
~~~

Attention la fonction pop() renvoit la valeur, ce qui peut être très utile.
