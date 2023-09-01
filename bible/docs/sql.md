# SQL

### Insérer les données d'un CSV dans une table

Permet de lire un fichier csv et de l'insérer dans une table

```sql
LOAD DATA LOCAL INFILE '~/mon_fichier.csv'
INTO TABLE ma_table
FIELDS 
    TERMINATED BY '\t'
    ENCLOSED BY '"'
    ESCAPED BY '\\'
LINES
    TERMINATED BY '\n';
```

### Commandes SQL

Permet d'afficher la description d'une table
`DESCRIBE my_table`