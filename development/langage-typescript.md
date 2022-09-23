# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'intéret de TypeScript dans l'IDE ✔️
  -> l'auto-complétion
- les types de bases ✔️
  -> types de données JS (string, boolean, number, void, null ...)
- comment et pourquoi étendre une interface ✔️
  -> une interface permet de définir le typage d'une ou plusieures données et de pouvoir utiliser ce typage partout dans le code (à condition d'exporter l'interface)
- les classes et les decorators ❌

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

```
export interface IWilderProps {
  wilder: IWilder;
  fetchWilders: () => void;
}

const Wilder = ({ wilder: {id, name, skills}, fetchWilders } : IWilderProps) => {
  const deleteOne = async (e : FormEvent) => {
    await deleteWilder(id);
    console.log(id);
    fetchWilders();
  };
```

### Utilisation dans un projet ❌ / ✔️

[https://github.com/elodiedaubie/express-hello-wilders](...)

Description :

### Utilisation en production si applicable❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Doc officielle

- [https://www.typescriptlang.org/]

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- Revoir la notion de classes et les decorators ❌ / ✔️

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌
- J'ai fait une [présentation](...) ❌
