# Integration continue

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les enjeux de l'integration continue ✔️
- la mise en place d'une github action ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```yml
name: frontend-tests-workflow

on: pull_request # Activated when doing a pull request

jobs:
  test-frontend:
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v2
      - name: Goto frontend and run tests
        run: cd frontend && npm i && npm test # Is executed directly by github for each pull request
```

### Utilisation dans un projet  ✔️

[healthcheck](https://github.com/WildCodeSchool/2024-02-wns-bleu-healthcheck)

Description : 

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description : La CI est utilisée pour exécuter les tests à chaque pull request

### Utilisation en environement professionnel ❌

Description : Pas utilisé actuellement mais j'espère aider à le mettre en place dans le futur

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
