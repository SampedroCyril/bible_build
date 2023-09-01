# HTML (.html)
## L'HTML (HyperText Markup Language) c'est quoi ?

Le HyperText Markup Language, généralement abrégé HTML ou, dans sa dernière version, HTML5, est le langage de balisage conçu pour structurer et représenter les pages web.

## Base du HTML

```HTML
<!DOCTYPE html>
<html>
    <head>
        <title>Titre de la page</title>
    </head>
    <body>
        Contenu de la page
    </body>
</html>
```

## Eléments courants

- En-têtes :

```html
<h1>Titre de niveau 1</h1>
<h2>Titre de niveau 2</h2>
<h3>Titre de niveau 3</h3>
<h4>Titre de niveau 4</h4>
<h5>Titre de niveau 5</h5>
<h6>Titre de niveau 6</h6>
```

- Paragraphes :

```html
<p>Ceci est un paragraphe contenant du texte.<p>
```

- Listes desordonnées :
        
```html
<ul>
    <li>Elément 1</li>
    <li>Elément 2</li>
    ...
</ul>
```
- Listes ordonnées :

```html
<ol>
    <li>Elément 1</li>
    <li>Elément 2</li>
    ...
</ol>
```

- Listes imbriquées

```html
<ul>
    <li>Elément 1</li>
    <ul>
        <li>Elément 1 sous liste 1</li>
        ...            
    </ul>
    <li>Elément 2</li>
    <ol>
        <li>Elément 1 sous liste 2</li>
        ...
    </ol>
    ...
</ul>
```

- Liens HyperText :
> Les liens HyperText sont généralement dans des balises de types "block" comme des `<li>` ou encore des `<p>`.

```html
<p>Voici un paragraphe. Il contient <a href="https://mon_lien_hypertext">un lien</a>.</p>
```
- Images :

```html
<img src="lien_de_mon_image">
```

> Les liens des images ou des liens hypertext peuvent être locales ou en ligne, si votre fichier html se trouve au même endroit (de même pour l'image), le lien sera dit "local". S'il se trouve dans le même dossier, alors il vous suffira juste d'utiliser le fichier comme l'exemple suivant : `mon_fichier.html` ou `mon_image.png`. S'il se trouve dans un sous dossier par rapport au dossier actuel ce sera sous la forme : `mon_sous_dossier/monfichier.html`. Si votre page html ou votre image est en ligne alors ce sera un lien hypertext : `https://mon_lien_hypertext`.

Ceci ne sont que des exemples d'utilisation des balises les plus courantes, pour voir plus voir cliquer [ici](cheatsheet_html.md).

## Attributs

