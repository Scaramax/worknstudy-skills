# Tester son application

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les tests unitaires ✔️
- les mocks ✔️
- les tests d'integration ✔️
- les tests de bout en bout (end to end) ✔️
- le TDD ✔️
- les tests par snapshot ❌

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

Exemple de test de rendering simple :
```tsx
import { render, screen } from "@testing-library/react";
import "@testing-library/jest-dom";
import Home from "../pages/home/Home";
import { test, expect } from "vitest";

import { MockedProvider } from "@apollo/client/testing";
import { TEST_URL } from "@/common/graphql/queries";

const mocks = [
  {
    request: {
      query: TEST_URL,
      variables: {},
    },
    result: {
      data: {
        testUrl: {
          url: "http://example.com",
          lastStatus: {
            date: "2024-01-01",
            response_time: 200,
            status: 2,
            status_code: 200,
            status_message: "Success",
          },
        },
      },
    },
  },
];

test("renders the main title", () => {
  render(
    <MockedProvider mocks={mocks} addTypename={false}>
      <Home />
    </MockedProvider>
  );
  const titleElement = screen.getByText(/LA NOUVELLE ÈRE DU DASHBOARDING/i);
  expect(titleElement).toBeInTheDocument();
});
```

### Utilisation dans un projet ✔️

[healthcheck](https://github.com/WildCodeSchool/2024-02-wns-bleu-healthcheck)

Description :

### Utilisation en production si applicable❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description : Malheureusement pas mis en place dans mon entreprise actuelle, mais j'espère améliorer ceci. En revanche, j'ai 4 ans d'expérience dans un poste de Lead Assurance Qualité Logicielle (mais je ne développais pas de tests).

## 🌐 J'utilise des ressources

### Titre

- lien
- description

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
