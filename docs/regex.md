# Regex

## Qu'est ce qu'est regex ?
Regex, ou expressions régulières, est comme un outil de recherche avancé pour du texte. Ça te permet de matcher, chercher, ou remplacer du texte en suivant des règles spécifiques.

## Exemple de contexte
Dans le code, tu utilises des fonctions qui acceptent des expressions régulières comme arguments. Par exemple, en PHP, tu pourrais utiliser la fonction preg_match().

Imaginons que tu as une grande chaîne de texte et tu veux vérifier si un numéro de téléphone français y est caché. Ton code ressemblerait à ça :

```php
$text = "Mon numéro est 0123456789, appelez-moi !";
$pattern = "/0[1-9][0-9]{8}/";

if (preg_match($pattern, $text, $matches)) {
  echo "Numéro trouvé : " . $matches[0];
} else {
  echo "Pas de numéro trouvé.";
}
```

Dans cet exemple, **preg_match** cherche le pattern de la regex dans la chaîne $text. Si ça trouve, ça remplit $matches avec ce qu'il a trouvé.