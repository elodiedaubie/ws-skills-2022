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
- les classes et les decorators ✔️ les decorators sont une syntaxe spécifique qui peuvent d'appliquer à des paramètres ou des classes

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```sh
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

### Utilisation dans un projet ✔️

[Lien GitHub](https://github.com/WildCodeSchool/2209-wns-adleman-citycompass)

Description :

### Utilisation en production si applicable ❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

- [Doc-Officielle-TypeScript] (https://www.typescriptlang.org/)

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- Action 1 ❌ / ✔️
- Action 2 ❌ / ✔️

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌
- J'ai fait une [présentation](...) ❌
