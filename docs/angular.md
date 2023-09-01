# Angular
## TUTO ANGULAR

<details>
  <summary>Autre</summary>
  <ul>
    <li><a href="https://openclassrooms.com/fr/courses/7471261-debutez-avec-angular">OpenClassrooms</a></li>
    <li><a href="https://www.w3schools.com/angular/">W3C Schools</a></li>
  </ul>
</details>

<details>
  <summary>Angular Websites</summary>
  <b>Always download the starting code</b>
  <ul>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-01">Lesson 1 : Hello world</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-02">Lesson 2 : Create Home component</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-03">Lesson 3 : Create the application’s HousingLocation component</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-04">Lesson 4 : Creating an interface</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-05">Lesson 5 : Add an input parameter to the component</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-06">Lesson 6 : Add a property binding to a component’s template</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-07">Lesson 7 : Add an interpolation to a component's template</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-08">Lesson 8 : Use *ngFor to list objects in component</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-09">Lesson 9 : Angular services</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-10">Lesson 10 : Add routes to the application</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-11">Lesson 11 : Integrate details page into application</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-12">Lesson 12 : Adding a form to your Angular app</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-13">Lesson 13 : Add the search feature to your app</a></li>
   <li><a href="https://angular.io/tutorial/first-app/first-app-lesson-14">Lesson 14 : Add HTTP communication to your app</a></li>
  </ul>
</details>

## Commandes Utiles Angulars CLI & NPM

<details>
   <summary><strong>Commandes Angular CLI</strong></summary>

   <ol>
   <li><strong>Créer un nouveau projet</strong>
      <ul>
         <li>Commande : <code>ng new [project-name]</code></li>
         <li>Description : Crée un nouveau projet Angular.</li>
         <li>Exemple : <code>ng new mon-application</code></li>
      </ul>
   </li>

   <li><strong>Servir l'application localement</strong>
      <ul>
         <li>Commande : <code>ng serve</code></li>
         <li>Description : Construit et sert votre application localement, la rendant généralement accessible via <code>http://localhost:4200/</code>.</li>
      </ul>
   </li>

   <li><strong>Générer du code</strong>
      <ul>
         <li>Commande : <code>ng generate [type] [name]</code> ou <code>ng g [type] [name]</code></li>
         <li>Description : Génère du code (comme des composants, des services, des modules, etc.).</li>
         <li>Exemple : <code>ng generate component mon-composant</code> ou <code>ng g c mon-composant</code></li>
      </ul>
   </li>

   <li><strong>Construire l'application pour la production</strong>
      <ul>
         <li>Commande : <code>ng build</code></li>
         <li>Description : Construit votre application et la stocke dans le répertoire <code>dist/</code>.</li>
      </ul>
   </li>

   <li><strong>Exécuter les tests unitaires</strong>
      <ul>
         <li>Commande : <code>ng test</code></li>
         <li>Description : Exécute les tests unitaires de votre application.</li>
      </ul>
   </li>

   <li><strong>Exécuter les tests de bout en bout</strong>
      <ul>
         <li>Commande : <code>ng e2e</code></li>
         <li>Description : Exécute les tests de bout en bout de votre application.</li>
      </ul>
   </li>

   <li><strong>Vérifier la qualité du code</strong>
      <ul>
         <li>Commande : <code>ng lint</code></li>
         <li>Description : Vérifie la qualité de votre code en utilisant TSLint.</li>
      </ul>
   </li>

   <li><strong>Mettre à jour les packages et le code</strong>
      <ul>
         <li>Commande : <code>ng update</code></li>
         <li>Description : Met à jour les packages et le code de votre application.</li>
      </ul>
   </li>

   <li><strong>Ajouter le support pour une bibliothèque externe</strong>
      <ul>
         <li>Commande : <code>ng add [package-name]</code></li>
         <li>Description : Ajoute le support pour une bibliothèque externe à votre projet (par exemple, Angular Material).</li>
         <li>Exemple : <code>ng add @angular/material</code></li>
      </ul>
   </li>

   <li><strong>Consulter la documentation officielle</strong>
      <ul>
         <li>Commande : <code>ng doc [keyword]</code></li>
         <li>Description : Ouvre la documentation officielle Angular pour un mot-clé donné.</li>
         <li>Exemple : <code>ng doc component</code></li>
      </ul>
   </li>
   </ol>
</details>

<details>
   <summary><strong>Commandes npm pour ANGULAR</strong></summary>

   <ol>
   <li><strong>Initialiser un nouveau projet npm</strong>
      <ul>
         <li>Commande : <code>npm init</code></li>
         <li>Description : Crée un nouveau fichier <code>package.json</code> pour votre projet.</li>
      </ul>
   </li>

   <li><strong>Installer les dépendances d'un projet</strong>
      <ul>
         <li>Commande : <code>npm install</code></li>
         <li>Description : Installe toutes les dépendances listées dans <code>package.json</code>.</li>
      </ul>
   </li>

   <li><strong>Installer une bibliothèque ou un paquet spécifique</strong>
      <ul>
         <li>Commande : <code>npm install [package-name]</code></li>
         <li>Description : Installe un paquet spécifique et l'ajoute à <code>node_modules</code>.</li>
         <li>Exemple : <code>npm install @angular/core</code></li>
      </ul>
   </li>

   <li><strong>Installer une bibliothèque ou un paquet comme dépendance de développement</strong>
      <ul>
         <li>Commande : <code>npm install [package-name] --save-dev</code></li>
         <li>Description : Installe un paquet spécifique comme dépendance de développement (souvent utilisé pour les outils de test ou de build).</li>
         <li>Exemple : <code>npm install typescript --save-dev</code></li>
      </ul>
   </li>

   <li><strong>Désinstaller une bibliothèque ou un paquet</strong>
      <ul>
         <li>Commande : <code>npm uninstall [package-name]</code></li>
         <li>Description : Désinstalle un paquet et le supprime de <code>node_modules</code> et <code>package.json</code>.</li>
      </ul>
   </li>

   <li><strong>Mettre à jour les paquets</strong>
      <ul>
         <li>Commande : <code>npm update</code></li>
         <li>Description : Met à jour tous les paquets à leurs dernières versions compatibles, en fonction des règles définies dans <code>package.json</code>.</li>
      </ul>
   </li>

   <li><strong>Exécuter un script défini dans <code>package.json</code></strong>
      <ul>
         <li>Commande : <code>npm run [script-name]</code></li>
         <li>Description : Exécute un script spécifique défini dans la section "scripts" de <code>package.json</code>.</li>
         <li>Exemple : <code>npm run build</code></li>
      </ul>
   </li>

   <li><strong>Vérifier les paquets obsolètes</strong>
      <ul>
         <li>Commande : <code>npm outdated</code></li>
         <li>Description : Affiche une liste des paquets qui ont des versions plus récentes disponibles.</li>
      </ul>
   </li>

   <li><strong>Vérifier la sécurité des paquets</strong>
      <ul>
         <li>Commande : <code>npm audit</code></li>
         <li>Description : Vérifie les dépendances du projet pour les vulnérabilités de sécurité connues et affiche des recommandations pour y remédier.</li>
      </ul>
   </li>

   <li><strong>Lancer l'application Angular en mode développement</strong>
      <ul>
         <li>Commande : <code>npm start</code></li>
         <li>Description : Une commande couramment utilisée pour démarrer une application Angular en mode développement, généralement définie dans la section "scripts" de <code>package.json</code> pour exécuter <code>ng serve</code>.</li>
      </ul>
   </li>

   <li><strong>Configurer le serveur JSON</strong>
      <ul>
         <li>Commande : <code>npm install -g json-server</code></li>
         <li>Description : Installe <code>json-server</code> globalement pour créer un faux serveur REST à partir d'un fichier JSON.</li>
      </ul>
   </li>

   <li><strong>Lancer le serveur de la db stockée en json</strong>
      <ul>
         <li>Commande : <code>json-server --watch db.json</code></li>
         <li>Description : Démarre <code>json-server</code> et surveille les modifications du fichier <code>db.json</code> pour simuler une base de données en temps réel.</li>
      </ul>
   </li>
   </ol>
</details>
