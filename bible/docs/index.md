# La Bible du dev (L'évangile selon CS)

:warning: Ce site est en construction, il contient des éléments pouvant êtres utiles mais ce n'est pas la version finale de celui-ci. Il ne sera probablement jamais "terminé" mais là c'est loin d'être fini !

## Présentation

Cette documentation utilise la technologie MkDocs / MkDocs material. Le langage utilisé est le **MarkDown**. Cette doc est spécialement faite pour les développeurs, donc si tu n'as pas les bases, check internet first!

## Installation Mkdocs

Mkdocs requiert python ainsi que pip.
Pour installer mkdocs, ouvrez votre terminal utilisez la commande `pip install mkdocs`.
Déplacez vous dans votre projet avec `cd mon_projet/`.

## Commandes MkDocs

* `mkdocs new [ma-doc]` - Créer le projet.
* `mkdocs serve` - Lancer le serveur.
* `mkdocs build` - Build le projet.
* `mkdocs -h` - Affiche l'aide.

Si les commandes ci-dessus ne fonctionnent pas, préfixez les avec `python -m`

## Structure du projet avec mkdocs.yml

```yml
mkdocs.yml    # Le fichier de configuration.
docs/
    index.md  # Page d'accueil de la documentation.
    ...       # Autres pages de la documentation.
```


Exemple de nav plus complet :

```yml
nav:
    - Home: 'index.md'
    - lien: 'fichier.md'
    - sous-menu:
        - 'lien1 sous-menu': 'fichier.md'
        - 'lien2 sous-menu': 'fichier.md'
    - lien dans menu re normal: 'fichier.md'
```