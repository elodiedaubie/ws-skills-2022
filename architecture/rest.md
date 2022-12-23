# REST API

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les verbes HTTP ✔️
  -> les verbes http sont des méthodes de requêtes utilisant le protocole http. Chaque méthode permet une action spécifique, par exemple GET pour les requêtes, POST pour envoyer des données vers le serveur, DELETE pour supprimer les ressources ...

- les statuts HTTP ✔️
  -> les statuts http sont des codes de réponses http permettant d'identifier le résultat de la requête. Ceux-ci sont composés de 3 chiffres, sont divisés en 5 catégories avec un prefixe signifiant:
  1xx = Informationnel / 2xx = Succès / 3xx = redirection / 4xx = erreur du client // 5xx = erreur du serveur

- les endpoints ✔️
  -> ils fournissent l'emplacement d'une donnée sur le serveur via une URI afin que le client puisse interagir avec le serveur.
- CORS ✔️
  -> Le Cross Origin Ressource Sharing : permet le partage de ressource entre des origines différentes, via les en têtes HTTPS. Par exemple : des requêtes faites depuis le localHost en local vers une API Rest qui se trouve sur une autre machine.
- la nomenclature recommandée pour les routes ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

#### Exemple de nomenclature de route ✔️

```sh
app.use(cors({ origin: "http://localhost:3000" }));

app.post("/wilders", wildersController.create);
app.get("/wilders", wildersController.read);
app.get("/wilders/:id", wildersController.readOne);
app.patch("/wilders/:id", wildersController.update);
app.delete("/wilders/:id", wildersController.delete);
app.post("/wilders/:wilderId/skills", wildersController.addSkill);
app.delete("/wilders/:wilderId/skills/:skillId", wildersController.removeSkill);
app.patch("/wilders/:wilderId/skills/:skillId", wildersController.updateGrade);
```

### Utilisation dans un projet ❌

[lien github](...)

Description :

### Utilisation en production si applicable ❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- [Axios] (https://axios-http.com/fr/docs/intro)
- Client Http basé sur les promesses et compatible avec Node.js, permettnt de construire des API Rest

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
