# Docker

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la création d'une image docker ✔️
- l'éxécution d'un container ✔️
- l'orchestration de containers avec docker-compose ✔️


## 💻 J'utilise

### Un exemple personnel commenté ✔️

Exemple de docker compose :
```
services:
    server:
        build: ./server #Builds the image from the server folder
        ports:
            - 5050:5000 #Links the port 5050 from the local machine to the port 5000 of the container
        command: npm run dev #Defines the command to be used to run the service
        volumes:
            - ./server/src/:/app/src/ #Links the src folder from the local machine to the container src folder, allows hot reloading
    client:
        build: ./client
        ports:
            - 8080:3000
        volumes:
            - ./client/src/:/app/src/
    mongodb:
        image: mongo #Builds the image directly from the mongo image available online
        volumes:
            - ./data:/data/db
```

Exemple de Dockerfile :
```
FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app

COPY package*.json ./
RUN npm i

COPY src src

CMD npm start
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/Scaramax/tgc-frontend) [lien github](https://github.com/Scaramax/tgc-backend)

Description : Utilisé pour le projet "the good corner". Note : il faut que je refasse un repo avec front et back ensemble pour que ça soit visible

### Utilisation en production si applicable❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- https://docs.docker.com/
- Docker doc

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
