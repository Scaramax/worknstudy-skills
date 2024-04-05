# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage  ✔️
- les normes `ecmascript`  ✔️
- l'utilisation de l'`asynchrone`  ✔️
- les spécifités du mot-clef `this`  ✔️

## 💻 Je code en Javascript

### Un exemple de code commenté  ✔️

Basé sur https://www.codewars.com/kata/52449b062fb80683ec000024
```javascript
// Function that generates Hashtags based on a sentence sent by the user
// Example : "Do we have a Hashtag" => #DoWeHaveAHashtag
function generateHashtag (str) {

//Remove eventual spaces at the beginning or end of the string
  if(str.trim() === "") {
    return false;
  }

//Create a string starting with #, by splitting the words in an array, then capitalizing each word, then joining capitalized words
  let hashTag = "#" + str.split(" ").map( word => {
    return word.charAt(0).toUpperCase() + word.substring(1);
  }).join("");

//Condition in the codewars kata
  if(hashTag.length > 140) {
    return false;
  }
  
  return hashTag;
}
```

### Utilisation dans un projet  ✔️

[[lien github](...)](https://github.com/Scaramax/beerbrowser)

Description : Utilisé dans l'ensemble de mes projets (repo privés)

### J'ai utilisé ce langage en production  ✔️

[lien du projet](...)

Description : Utilisé au quotidien en entreprise (repo privés)

### J'ai utilisé ce langage en environement professionnel  ✔️

Description : Utilisé au quotidien en entreprise (principalement TypeScript, React, Node.js)

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

- J'ai ecrit un [tutoriel](...) ❌
- J'ai fait une [présentation](...) ❌

