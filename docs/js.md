# JavaScipt (.js)
## Liste des Événements

- **`onchange`**: Se déclenche lorsqu'un élément HTML a été modifié.
```javascript
  document.getElementById("monInput").onchange = function() {
      alert("La valeur a été modifiée !");
  };
```

- **`onclick`**: Se déclenche lorsque l'utilisateur clique sur un élément HTML.
```javascript
  document.getElementById("monBouton").onclick = function() {
      alert("Bouton cliqué !");
  };
```

- **`onmouseover`**: Se déclenche lorsque l'utilisateur survole un élément avec sa souris.
```javascript
  document.getElementById("monElement").onmouseover = function() {
      alert("Vous survolez l'élément !");
  };
```

- **`onmouseout`**: Se déclenche lorsque l'utilisateur sort de l'élément HTML avec sa souris.
```javascript
  document.getElementById("monElement").onmouseout = function() {
      alert("Vous avez quitté l'élément !");
  };
```

- **`onkeydown`**: Se déclenche lorsque l'utilisateur appuie sur une touche du clavier.
```javascript
  document.onkeydown = function(event) {
      alert("Touche appuyée: " + event.key);
  };
```

- **`onload`**: Se déclenche lorsque le navigateur a fini de charger la page.
```javascript
  window.onload = function() {
      alert("Page complètement chargée !");
  };
```

- **`onfocus`**: Se déclenche lorsque un élément HTML reçoit le focus (sélectionné ou cliqué).
```javascript
  document.getElementById("monInput").onfocus = function() {
      alert("L'input est maintenant focalisé !");
  };
```

- **`onblur`**: Se déclenche lorsque un élément HTML perd le focus.
```javascript
  document.getElementById("monInput").onblur = function() {
      alert("L'input a perdu le focus !");
  };
```

- **`onsubmit`**: Se déclenche lorsque un formulaire est soumis.
```javascript
  document.getElementById("monFormulaire").onsubmit = function() {
      alert("Formulaire soumis !");
      return false;  // Pour éviter la soumission réelle du formulaire
  };
```

- **Exemple de code**:
```javascript
  // Exemple de code qui ouvre le pdf en target _blanks pour imprimer
  // Une fois sur le nouvel onglet, ouvre automatiquement la fonction d'impression
  // Une fois appuyé sur ok ou entrée, quitte la page avec un délai d'1 sec
  function impression(url) {
      var newWindow = window.open(url, '_blank');  // Petite correction : '_blank' plutôt que '_blanks'
      newWindow.onload = function() {
          newWindow.print();
      }
      setTimeout(function() {
          newWindow.alert("L'impression est terminée. Cliquez sur OK ou appuyez sur Entrée pour fermer cet onglet.");
          newWindow.close();
      }, 1000);
  }
```

---

## Les manipulations de listes

- **Parcourir l'ensemble d'une liste et afficher ses élements**

```js
const names = ['Jack', 'Laura', 'Paul', 'Megan'];
names.forEach((name) => console.log(name));
```

- **`delete`** : Supprime une élement d'une liste.

```js
const names = ['Jack', 'Laura', 'Paul', 'Megan'];
delete names[1];
// => ["Jack", empty, "Paul", "Megan"]
```

- **`length`**
