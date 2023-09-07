# Python CheatSheet

## Méthodes intégrées 

- **strip()**
Elle sert à supprimer les espaces avant et après l'objet

```py
name = "      blabla    "
print(name.strip())
>>>blabla
```

- **title()**
Met en capitale à chaque début de mot

```py
print('hello world'.title())
>>> Hello World
```

## Methode #split
Permet de séparer une chaine de caractères par ses espaces et de stocker le tout dans un tableau

```py
message = "1 2 3 4 5"
print(message.split())
>>> ['1', '2', '3', '4', '5']
```

## Methode #ord
Permet de récupérer le code ASCII d'un ou plusieurs caractères

```py
print(ord('k'))
>>>107
```

## Methode #chr
Permet de récupérer le caractère d'un code ASCII

```py
print(chr(107))
>>>k
```

