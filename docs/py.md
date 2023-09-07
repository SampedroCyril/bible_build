# Python (.py)


## Bases

Afficher dans le terminal "Hello World !"

- **print()**

```py
print("Hello World !")
```

Arguments du print()

- **print("lol", sep="", end="")**

La fonction print peut prendre plusieurs arguements tels que `sep` ou `end`
- sep : permet de définir les séparateurs dans le print, par défaut `sep = " "`
- end : permet de définir la fin de la ligne qui est par défaut `end = "\n"` qui veut dire retour à la ligne.

Demander à l'utilisateur d'entrer quelque chose

- **Input()** 

```py
name = input("Quel est votre nom :" )
print("Bonjour ", name, "!")
```

Vérififer le type de la variable

- **type()**

```py
my_var = "lol"
type(my_var)
```
> Ressort le type de la variable qui est `str` dans ce cas là

Le python est un langage du type **dynamique**, une variable n'a pas de type prédéfini parmis cette liste :
- integer (nombre) 
- string (chaine de caractères) 
- boolean (vrai ou faux)
- ...

exemple :
```py
a = 1
a = "lol"
print(a)
```
> Affichera `lol` sans erreur.

Pour transformer une chaine de caractère en entier, on appelle ce concept le **cast**
- str => int :
```
number = "12"
number = int(number)
```

## Les fonctions

Les fonctions font partis des bases en programmation et notamment en python.

Voici un exemple de fonction qui affiche "Hello World", nous allons juste créer une fonction sans arguments.

```py
def hello_world():
  print("Hello World")

hello_world()
```
Voici un exemple de fonction avec argument et qui affiche "Bonjour" et votre nom

```py
def hello_you(name):
  print("Bonjour",name)
```

Pour aller un peu plus loin, nous allons créer une fonction du type "none" ou "procédure"

```py
def calcul_addition(a,b):
  return a+b

nombre_a = int(input("a = "))
nombre_b = int(input("b = "))
print(calcul_addition(nombre_a,nombre_b))
```


## Les conditions

Pour vérifier le contenue des variables et renvoyer un boolean (pour vérifier si / sinon si / sinon. Les controll flow `if elif et else` vous permettent de faire cela

```py
age = int(input("Entrez votre age : "))
if age < 18:
  print("Vous êtes mineur")
elif age > 18 and age < 50:
  print("Vous êtes Majeur")
else: # Va prendre tout ce qui est supérieur a 50
  print("Vous êtes un vieux du cul")
```

L'opérateur `and` va permettre de vérifier 2 conditions, pour le `elif` (sinon si) cela va vérifier si l'age est supérieur a 18 et inférieur à 50. Si une des deux conditions n'est pas remplis cela va skip la condition et ne pas rentrer dedans. Dans le même genre vous avez l'opérateur `or` qui permet de vérifier plusieurs conditions, et si l'une des conditions est remplie alors on va rentrer dans le controll flow.

Il existe une autre façon de poser des conditions que `if elif else`, cela permet de rendre le code plus lisible losque vous avez beaucoup de conditions qui s'enchainent 

```py
choice = int(input("1 ou 2 : "))
match choice:
    case 1:
        print(1)
    case 2:
        print(2)
```

Pour résumer :

- if = si + condition
- elif = sinon si + condition
- else : sinon => Prend tout le reste

- AND = opérateur booléen qui vérifie que plusieurs conditions doivent êtres remplies
- OR = opérateur booléen qui vérifi si l'une des conditions est remplie

- match + variable a vérifier
    - case = condition a vérifier


Pour plus de contenu voir la page [Python CheatSheet](cheatsheet_py.md)