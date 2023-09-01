# Markdown (Md)
## Le Markdown c'est quoi ?

Tout comme HTML ou LaTeX, Markdown est un langage de balisage. Contrairement aux deux premiers langages, Markdown se veut être facile à lire par les personnes. Les balises ne doivent pas être abstraites, mais proches de leur véritable signification. Le plus simple est d’illustrer mes propos avec un exemple pour mettre en gras un mot.

## Titres

```md
# H1
## H2
### H3
#### H4
##### H5
###### H6

Version alternative pour les H1 / H2, version "sous-ligné":

Alt-H1
======

Alt-H2
------
```

## Paragraphes

Les paragraphes ont une syntaxe très basique, elle ne requiert aucun balisage.

```markdown
Ceci est un paragraphe pour dire que c'est un paragraphe !
<!-- Pour sauter une ligne  -->
<br>
Ceci est un autre paragraphe!
....
```

## Texte en gras / italique / barré

Écrire en gras et en italique est particulièrement facile avec Markdown. Il suffit d’utiliser les étoiles, appelées aussi astérisques. Une autre option consiste à utiliser les tirets bas.

<br>

```markdown
*Texte en italique*
_Texte en italique_
**Texte en gras**
__Texte en gras__
***Texte en italique et en gras***
___Texte en italique et en gras___
```

## Les listes

Si vous souhaitez établir une liste simple (ou `<ul>` en Html qui signifie ***Unordered List***) avec Markdown, vous avez le choix entre **le signe plus, le tiret ou un astérisque**. Ces trois options donnent le même rendu. La syntaxe la plus utilisée est celle avec **les tirets**.

```markdown
- Liste 1
- Liste 2
- Liste 3

<!-- Autre exemple -->

+ Liste 1
+ Liste 2
+ Liste 3

<!-- Autre exemple -->

* Liste 1
* Liste 2
* Liste 3
```

Pour créer une liste numérotée, il vous suffira d’inscrire un `chiffre suivi d’un point`. Deux écritures différentes qui produisent le même résultat.

```markdown
1. Liste 1
2. Liste 2
3. Liste 3

<!-- Autre exemple -->

1. Liste 1
1. Liste 2
1. Liste 3
```

Les listes peuvent aussi être **imbriquées** voici quelques exemples.

```markdown
- Liste 1
    - Sous-Liste 1
    - Sous-Liste 2
- Liste 2
    - Sous-Liste 1
    - Sous-Liste 2
    1. Sous-Liste numérotée 1
    2. Sous-Liste numérotée 2

<!-- Autre exemple -->

1. Liste numérotée 1
    - Sous-Liste 1
    - Sous-Liste 2
    1. Sous-Liste numérotée 1
    2. Sous-Liste numérotée 2

<!-- Autre exemple -->

- Liste 1
    - Sous-Liste 1
        - Sous Sous-Liste 1
        - Sous Sous-Liste 2
    - Sous-Liste 2
        1. Sous Sous-Liste numérotée 1
        2. Sous Sous-Liste numérotée 2
- Liste 2
    - Sous-Liste 1
    ...
```

## Les tableaux



## Cases cochées / décochées

```md
- [x] Élément 1, coché
- [ ] Élément 2, non-coché
  - [x] Sous-élément 2.1, coché
  - [ ] Sous-élément 2.2, non-coché
- [ ] Élément 3, non-coché
```

## Collapsible Section

Ouverture automatique avec `open`

```md
<details open>
  <summary>Hello</summary>
  World!
</details>
```

Custom balises

```md
<details>
  <summary><i>Wow, so fancy</i></summary>
  <b>WOW, SO BOLD</b>
</details>
```

Imbriqué

```md
<details>
  <summary>Section A</summary>
  <details>
    <summary>Section A.B</summary>
    <details>
      <summary>Section A.B.C</summary>
      <details>
        <summary>Section A.B.C.D</summary>
          Done!
      </details>
    </details>
  </details>
</details>
```