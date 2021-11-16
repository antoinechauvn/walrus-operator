# Découverte du walrus opérateur dans une condition basique

</br>

> Qu’est-ce que l’opérateur morse ?
L’opérateur que l’on nomme opérateur morse est un opérateur noté := et permettant de simultanément faire une allocation et un test dans la même expression. Il est associé à ce nom du fait de sa ressemblance avec l’animal (les yeux et les défenses).

```py
__author__ = "Chauvin Antoine"
__copyright__ = ""
__credits__ = ["Chauvin Antoine"]
__license__ = ""
__version__ = "1.0"
__maintainer__ = "Chauvin Antoine"
__email__ = "antoine.chauvin@live.fr"
__status__ = "Production"


#  Dans un premier temps on effectue un assignement normal
var = 1
if var > 1:
    print("oui")

# Le Walrus Operator permet d'effectuer un assignement au sein même d'une condition
if (var := 1) > 0: # On donne à var la valeur 1
    print(var)
    print("oui")

if var := 1 > 0:  # ERREUR ici on a oublié les parenthèses
    """Dans ce cas var est un booléen qui vaut True si la 
    condition >0 est remplie et False dans le cas contraire"""
    print(var)
    print("oui")
```

###### © 2021 stats4decision & realpython
