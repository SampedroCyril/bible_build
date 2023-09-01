# Java (.java)
## Types de Classes et Structures en Java

## Types de Classes et Structures en Java

### Classes

- **Classe Standard**:
  - Définit les attributs et les méthodes que ses objets vont posséder.
```java
  public class MaClasse {
      private int monAttribut;
      public void maMethode() { /* ... */ }
  }
```

- **Classe Abstraite**:
  - Ne peut pas être instanciée directement.
  - Peut contenir des méthodes abstraites (sans corps) qui doivent être implémentées par les sous-classes.
```java
  public abstract class Forme {
      public abstract double aire();
  }
```

### Interfaces

- **Interface**:
  - Définit un contrat que les classes implémentant l'interface doivent suivre.
  - Contient uniquement des méthodes abstraites (dans les versions Java avant Java 8) mais peut contenir des méthodes par défaut ou des méthodes statiques depuis Java 8.
```java
  public interface MonInterface {
      void maMethode();
  }
```

### Enumérations

- **Enum**:
  - Un type spécial de classe qui représente un groupe de constantes (variables qui ne changent pas).
```java
  public enum Jours {
      LUNDI, MARDI, MERCREDI, JEUDI, VENDREDI, SAMEDI, DIMANCHE
  }
```

### Classes internes

- **Classe Interne**:
  - Une classe définie à l'intérieur d'une autre classe.
  - A accès aux membres privés de la classe externe.
```java
  public class Externe {
      private int x = 10;
      class Interne {
          public void afficher() {
              System.out.println(x);
          }
      }
  }
```

- **Classe Interne Statique**:
  - Similaire à une classe interne, mais déclarée avec le mot-clé `static`.
  - N'a pas accès aux membres non statiques de la classe externe.
```java
  public class Externe {
      static class InterneStatique {
          // ...
      }
  }
```

- **Classes Anonymes**:
  - Une classe sans nom, généralement utilisée pour surcharger des méthodes d'interfaces ou de classes abstraites pour des usages ponctuels.
```java
  MonInterface monObjet = new MonInterface() {
      @Override
      public void maMethode() {
          // Implémentation ici
      }
  };
```

Ceci est un aperçu des types de classes et structures les plus couramment utilisés en Java. Il existe d'autres nuances et détails qui peuvent être explorés en profondeur en fonction des besoins.




## Annotations JAVA SPRING

### Lombok

- **`@Getter` / `@Setter`**: 
  - Permet d'éviter d'écrire manuellement les getters et setters, réduisant ainsi le volume de code.
  - **Paramètre `lazy`** : Utilisez-le comme `@Getter(lazy = true)`. Il permet de mettre en cache des données pour éviter de répéter des opérations coûteuses.

- **`@NoArgsConstructor`**: 
  - Génère automatiquement un constructeur sans arguments, évitant ainsi la nécessité de le déclarer manuellement.

- **`@AllArgsConstructor`**: 
  - Génère automatiquement un constructeur avec des arguments pour tous les champs de la classe, ce qui est particulièrement utile pour les classes de données.

- **`@Data`**: 
  - Combinaison de `@Getter`, `@Setter`, `@RequiredArgsConstructor`, `@ToString` et `@EqualsAndHashCode`. Il fournit une représentation complète d'une classe sans avoir à écrire beaucoup de code boilerplate.

- **`@EqualsAndHashCode`**:
  - Génère les méthodes `equals` et `hashCode` basées sur les champs de la classe, assurant une comparaison d'égalité basée sur le contenu plutôt que sur la référence de l'objet.

- **`@Slf4j`**: 
  - Ajoute un logger à la classe sans nécessité de le déclarer manuellement. Très utile pour le logging.

### Spring

- **`@Entity`**: 
  - Indique qu'une classe est une entité. Elle est généralement utilisée avec JPA pour représenter une table de base de données.

- **`@Autowired`**: 
  - Effectue l'injection automatique des dépendances dans les beans Spring. Il permet d'injecter automatiquement les objets dans votre code.

- **`@Service`**: 
  - Indique qu'une classe est un service dans la logique métier de l'application. Elle est généralement utilisée pour opérer sur les entités et interagir avec les bases de données.

- **`@Repository`**: 
  - Marque une classe comme un Repository, indiquant ainsi son rôle de communication avec la base de données.

- **`@Controller`**: 
  - Indique qu'une classe sert de contrôleur dans le modèle MVC de Spring. Elle est responsable de traiter les requêtes entrantes et de renvoyer une réponse.

- **`@RequestMapping`**: 
  - Utilisée pour mapper les requêtes web sur des classes ou des méthodes spécifiques du contrôleur. Elle peut spécifier l'URL, la méthode (GET, POST, etc.) et d'autres attributs de la requête.

- **`@Component`**: 
  - Un indicateur générique qui signifie qu'une classe est un composant Spring. Les classes annotées avec `@Component` sont détectées lors de la scan de classpath et sont enregistrées dans le contexte d'application de Spring.