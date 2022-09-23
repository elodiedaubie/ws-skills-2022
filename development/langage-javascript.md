# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage ✔️
  -> structures conditionnelles (if ..else ou ternaire)
  -> créer une fonction (mot clé function, fonction flechée, callback)
  -> boucles (for, while)
  -> utilisation des functions natives de JS sur tableau (.filer, .map, .foreach), string (.lenght, .repeat, .search)
- les normes `ecmascript` ✔️
  -> la dernière version majeure est ES6, il s'agit de définir les normes du lanagages. A chaque nouvelle version (tous les ans), des nouvelles fonctionnalités, mot clé ou structures sont apportées. Ex : var qui est devenu let/const ou les fonction fléchées au lieu de l'utilisation du mot clé function
- l'utilisation de l'`asynchrone` ❌
  -> J'ai utilisé l'async/await mais n'ai pas tout à fait compris la notion de promise
- les spécifités du mot-clef `this` ✔️
  -> Le mot clé this est utilisé à l'intérieur d'une classe, pour faire référence à l'objet qui sera instancié avec celle-ci

## 💻 Je code en Javascript

### Un exemple de code commenté ✔️

```javascript
// L'objectif est de créer une fonction qui prend un tableau et une callback en paramètre.
// La callback doit se charger de modifier les prénoms du tableau, pour les formater : John au lieu de JoHn
const people = [
  "JoHn",
  "ChrISTiana",
  "anThoNY",
  "MARia",
  "jaMeS",
  "MIChaEl",
  "jeNNIFeR",
];

const pascalCase = (string) => {
  return string[0].toUpperCase() + string.slice(1).toLowerCase();
};

const refactorArray = (array, callback) => {
  return array.map(callback);
};

console.log(refactorArray(people, pascalCase));
```

### Utilisation dans un projet ✔️

[https://github.com/elodiedaubie/express-hello-wilders](...)

Description :

### J'ai utilisé ce langage en production ❌

[lien du projet](...)

Description :

### J'ai utilisé ce langage en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Doc Javascript

[https://developer.mozilla.org/fr/docs/Web/JavaScript]
[https://devdocs.io/javascript/]

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- Faire une App React en JS à partir d'une API ❌ / ✔️
- Faire 10 code wars 7 kyu mini ❌ / ✔️

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
