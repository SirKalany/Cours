# Exemples de code JavaScript

## Création d'élément de façon dynamique

```js
const workContainer = document.querySelector(".gallery");
function createFigure(work) {
  const figure = document.createElement("figure");
  const figureCaption = document.createElement("figurecaption");
  const figureImage = document.createElement("img");

  // Assignation des sources de contenu

  figureImage.src = work.imageUrl;
  figureImage.alt = work.title;
  figureCaption.innerHTML = work.title;

  // Assignation des parents/enfants

  figure.appendChild(figureImage);
  figure.appendChild(figureCaption);
  workContainer.appendChild(figure);

  return figure;
}
```

1. **Sélection du conteneur:**

- const workContainer = document.querySelector(".gallery");

    - document.querySelector(".gallery") : Sélectionne le premier élément HTML ayant la classe 'gallery'.

    - const workContainer : Crée une constante qui contiendra cette référence DOM. Ce sera le conteneur dans lequel on va insérer les œuvres (figure).
 
2. **Déclaration d'une fonction**

- function createFigure(work) {;

    - createFigure(work) : Crée une fonction prenant un objet 'work' (œuvre récupérée via l'API, avoir API) comme paramètre.
 
3. **Création des éléments HTML**

-   const figure = document.createElement("figure");
-   const figureCaption = document.createElement("figurecaption");
-   const figureImage = document.createElement("img");

    - document.createElement(...) : Crée dynamiquement des éléments HTML
 
4. **Remplissage des données**

- figureImage.src = work.imageUrl;

    - Lien vers l’image de l’œuvre.
  
- figureImage.alt = work.title;

    - Texte alternatif en cas de problème de chargement, utile pour l’accessibilité.
 
- figureCaption.innerHTML = work.title;

    - Le titre de l’œuvre s’affiche comme légende sous l’image.

5. **Construction et insertion dans la page**

- figure.appendChild(figureImage);

- figure.appendChild(figureCaption);

    - figure.appendChild(...) : Ajoute l’image et la légende dans l’élément <figure>.
  
- workContainer.appendChild(figure);

    - Insère le <figure> complet dans le conteneur .gallery sur la page HTML.
 
5. **Retour de l’élément**

-   return figure;

    - La fonction retourne l’élément <figure> créé. Cela peut être utile si tu veux manipuler ou stocker cet élément ensuite.
