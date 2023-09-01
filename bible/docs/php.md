# PHP (.php)
## Concepts

**Conditions Ternaires**
```php
// CONCEPT
(Condition) ? (Statement1) : (Statement2);
Variable = (Condition) ? (Statement1) : (Statement2);
// EXEMPLE
<?php
  $a = 10;
  $b = $a > 15 ? 20 : 5;
  print ("Value of b is " . $b);
// Autre exemple
$ad1 = isset($_SESSION["adresse_delegue0"]) ? $_SESSION["adresse_delegue0"] : '';
?>
```
Output
```
Value of b is 5
```

[Lien opérateurs ternaires PHP](https://stacklima.com/php-operateur-ternaire/)

## Fonctions intégrées
  
(PHP 8.2.9)

- `mb_convert_encoding($chaine, 'ISO-8859-1')` : Converti en ISO
- `mb_convert_encoding($chaine, 'UTF-8')` : Converti en UTF-8