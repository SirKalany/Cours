# Exemples de code JavaScript

## Appel d'un API:

```js
async function getData() {
  const answer = await fetch("http://localhost:5000/api/data");
  return answer.json();
}
```

1. async function getWorks() {

    - async : Mot-clé qui rend la fonction asynchrone. Cela signifie que la fonction peut utiliser 'await' à l’intérieur, ce qui permet de mettre en pause l'exécution jusqu'à ce qu’une promesse soit résolue (Voir 2).

    - function getData() : Déclare une fonction nommée getData, qui sera utilisée pour récupérer des données.


2. const answer = await fetch("http://localhost:5000/api/data");

    - const answer = : Crée une constante locale answer qui va contenir la réponse de l’appel à l’API.

    - await : Attend que la promesse retournée par 'fetch(...)' soit résolue. Cela permet de récupérer directement le résultat, sans utiliser '.then().'

    - fetch("http://localhost:5000/api/data") : Appelle l’API située à cette adresse (probablement un serveur local). 'fetch' est une fonction intégrée de JavaScript pour faire des requêtes HTTP (GET par défaut).

3. return answer.json();
   
    - answer.json() : Transforme la réponse HTTP en objet JSON (ou tableau, selon ce que l’API renvoie). Cette méthode retourne aussi une promesse, car la conversion peut prendre un peu de temps.

    - return : La fonction retourne donc la promesse contenant les données converties.
