---
category: OS
path: '/Os'
title: 'Sous quel système je suis ?'
layout: null
---

### OS et Platform

Pour savoir sous quel système un script est en cours d'exécution il existe 
plusieurs solutions. La solution suivante reste une solution tout à fait portable et 
simple d'utilisation :

~~~ python
>>> import os
>>> os.name
'nt'
>>> import platform
>>> platform.system()
'Windows'
>>> platform.release()
'Vista'
~~~

Voici donc une manière simple et élégante de gérer des appels différents dans vos scripts :

~~~ python
import os
import platform

(...)

if platform.system().lower() == "windows":
  # action pour windows
else if platform.system().lower() == "darwin":
  # action pour MACOS
else if platform.system().lower() == "linux":
  # action pour Linux
~~~
