


### dir()

La fonction dir() permet d'accéder aux éléments présents dans l'espace de travail.

~~~ python
>>> dir()
['__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__']
>>> a = 1
>>> dir()
['__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__', 'a']
>>> import math
>>> dir()
['__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__', 'a', 'math']
>>> 
~~~

Elle permet également d'accéder aux fonctions applicables à certains éléments

~~~ python
>>> dir(a)
['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__', 
(...)
'bit_length', 'conjugate', 'denominator', 'from_bytes', 'imag', 'numerator', 'real', 'to_bytes']
~~~

### type()

La fonction type permet de connaitre le type actuel d'une variable. N'oubliez pas que les variables changent de type
en fonction de ce qu'elles contiennent

~~~ python
>>> a = 1
>>> type(a)
<class 'int'>
>>> a = "Salut"
>>> type(a)
<class 'str'>
~~~

### help()

La fonction help() permet d'accéder à l'aide en ligne dans un interpréteur. Elle peut également fournir la documentation
disponible sur une fonction.

~~~ python
>>> help()

Welcome to Python 3.6's help utility!
(...)
help> quit
>>>
~~~

~~~ python
>>> help(print)
Help on built-in function print in module builtins:

print(...)

(...)
>>>
~~~
