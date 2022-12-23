# Tester son application

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les tests unitaires ✔️
  -> ils servent à tester une fonction ou une classe en particulier, avec différents cas (succès, échecs, cas limites) en respectant les principes de responsabilité unique ou d'encapsulation.
- les mocks ✔️
  -> les mocks simulent des données ou reproduisent le comportement d'objets afin de passer des tests sans accéder à des données réelles (plus performant et garantissent une uniformité des tests auprès de toute l'équipe)
- les tests d'integration ✔️
  -> l'objectif des tests d'intégration est de vérifier une partie du code (ex une fonctionnalité) dans son ensemble avec l'interraction de plusieures fonctions ou classe spar exemple. Ils font généralement suite aux tests unitaires.
- les tests de bout en bout (end to end) ✔️
  -> ils permettent de simuler les interractions utilisateurs sur un ou plusieurs clients (ex : différents naviguateurs) avec l'application.
- le TDD ✔️
  -> le Test Driven Developpement est une méthode de développement qui s'appuie fortement sur les tests : ceux-ci sont rédigés avant l'écritude du code qui s'éxécutera. L'intérêt est double : d'une part, cela oblige à prévoir les cas d'échecs dès le départ ce qui permet d'écrire un code plus solide, d'autre part cela évite les regressions lorsque le code est retouché/refactorisé.
- les tests par snapshot ✔️
  -> le principe d'un snapshort est de sauvegarder dans un fichier le résultat attendu suite à l'éxecution de code et de comparer celui-ci avec le résultat réel à chaque fois que cette fonction est appelée dans le jeu de test. Cela permet de se prémunir contre une régression qui pourrait intervenir sur une autre fonctionnalité que celle qui a été modifiée ou de tester le rendu d'un composant React automatiquement.

## 💻 J'utilise

### Un exemple personnel commenté ✔️

#### Exemple de test unitaire

```sh
// fonction to test // getDisplayName.ts
const getDisplayName = (
firstName: string,
lastName: string,
city: string = "?",
curriculum = ""
) => {
if (curriculum != "workstudy") return `[${city}] ${firstName} ${lastName}`;
return `[${city}] ${firstName} ${lastName} - Wns`;
};

export default getDisplayName;
```

```sh
// set of tests - getDisplayName.test.ts
describe("getDisplayName", () => {
  it("Should display [city] before first name and last name if city is specified", () => {
    expect(getDisplayName("Jane", "Doe", "Lyon")).toBe("[Lyon] Jane Doe");
  });
  it("Should display [?] before first name and last name if city is not specified", () => {
    expect(getDisplayName("Jane", "Doe")).toBe("[?] Jane Doe");
  });
  it("Should display - Wns after the lastname if study curiculum is workstudy", () => {
    expect(getDisplayName("John", "Doe", "Paris", "workstudy")).toBe(
      "[Paris] John Doe - Wns"
    );
  });
  it("Should display nothing after the lastname if study curiculum is something else than workstudy", () => {
    expect(getDisplayName("John", "Doe", "Paris")).toBe("[Paris] John Doe");
    expect(getDisplayName("John", "Doe", "Paris", "regular")).toBe(
      "[Paris] John Doe"
    );
    expect(getDisplayName("John", "Doe", "Paris", "")).toBe("[Paris] John Doe");
  });
});
```

#### Exemple de test end to end

```sh
import { test, expect } from "@playwright/test";

// test on a free online calculator
test("calculate 6 x 2 = 12 correctly", async ({ page }) => {
  await page.goto("https://www.desmos.com/scientific?lang=fr/");
  await page.getByRole("button", { name: "6" }).click();
  await page.getByRole("button", { name: "Times" }).click();
  await page.getByRole("button", { name: "2" }).click();
  await page
    .getByRole("group", { name: "keypad" })
    .getByRole("button", { name: "Enter" })
    .click();
  await expect(page.getByText("equals 12=12", { exact: true })).toBeVisible();
});
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2209-wns-adleman-citycompass)

Description : projet d'étude de mon alternance à la WCS

### Utilisation en production si applicable ❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- [Jest] (https://jestjs.io/fr/)
- Framework de test JavaScript, pour tests unitaires ou d'intégration (TypeScript, Node, React ...)

- [Playwright] (https://playwright.dev/)
- Bibliothèque Node opur tests end to end

- [PHPUnit] (https://phpunit.de/)
- Framework de test unbitaires pour PHP

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
