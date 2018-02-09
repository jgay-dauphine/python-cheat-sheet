


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

### help()
