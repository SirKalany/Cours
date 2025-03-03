# Résumé du Cours: Maîtrisez les Translations, Rotations et Opacité

## Optimisez les performances de votre navigateur pour vos animations CSS

* A l'écran, il n'y a pas de véritable mouvement, mais une succession d'images s'enchaînant suffisamment rapidement pour être interprétées par notre cerveau comme du mouvement ;

* Cette succession d'images s'appelle les FPS (Frame Per Second, ce qui signifie images par seconde) ; Plus le FPS est élevé, plus l'animation est fluide ; Le taux d’images par seconde idéal est 60 FPS ;

* Les quatre étapes de la création d’une page web sont : 

* Style : le navigateur comprend la structure HTML du code qu'il reçoit et prépare le style qui sera appliqué,

* Layout (mise en page) : le navigateur détermine la mise en page et la taille des éléments en fonction du style qu'il a reçu,

* Paint : il transforme les éléments en pixels,

* Composition : `il` combine tous les éléments pour composer la page qui s’affiche ;

* Pour assurer la fluidité des animations, il faut se contenter d’animer des propriétés de l’étape composition. Les plus utiles sont  `transform`  et  `opacity`  .

## Créez des animations fluides avec la propriété CSS transform

* La propriété  transform  nous permet de manipuler et animer nos sites de presque toutes les manières, et comme tout se passe pendant l’étape composition, les animations sont bien fluides sur tous les supports ;

* On peut déplacer des éléments avec les fonctions `translate` :   `translate()`,  `translateX()`,  `translateY()`  et  `translate3d()`  ;

* On peut agrandir avec les fonctions `scale` :  `scale()`,  `scaleX()`,  `scaleY()`  et  `scale3d()`  ;

* Et on peut les faire pivoter grâce aux fonctions `rotate` :  `rotate()`,  `rotateX()`,  `rotateY()` et  `rotateZ()`  ;

* Si on ajoute une deuxième propriété  `transform`, elle annule la première. On ne peut donc définir qu’une seule propriété  `transform`  dans un même sélecteur ;

* Pour effectuer plusieurs transformations, on peut les lister dans une même propriété transform comme: transform:translateX(200%) scale(2);

* Une propriété avec plusieurs fonctions exécute les fonctions dans l’ordre, de droite à gauche ;

* Les fonctions de transformations en 3D comme `translate3d()`,  `rotateZ()`  et  `scale3d()`  ont également besoin de la fonction perspective pour indiquer au navigateur la distance à laquelle l'utilisateur se trouve : plus la distance est grande, moins l'animation sera marquée.

## Modifiez le point d’ancrage d’un élément grâce à transform

* `Transform-origin`  permet de repositionner le point d’ancrage, qui se trouve par défaut au centre de l’élément ;

* On peut régler ce point d’origine en utilisant des unités comme `px`, `rem`, `vh`, `etc`. ;

* Il est aussi possible d'utiliser des pourcentages pour X et Y ;

* Ou encore, on peut utiliser des mots clés :  left  et   right  pour l’axe X,  top  et  bottom  pour l’axe Y, et  center  pour les deux ;

* Ol est possible de ne pas indiquer la valeur de l'axe Y ou, quand on utilise des mots clés, de mettre uniquement une valeur : le navigateur comprend de lui-même à quel axe la valeur s'applique ;

* Quand on change le point d’origine en 3D, la valeur de Z doit être exprimée en unités (et non en pourcentages) !

## Analysez la performance de vos animations avec Chrome DevTools

* Chrome DevTools est l'outil de prédilection des développeurs. Il permet d'inspecter le code source d'une page, d'analyser les performances de notre page, de brider la performance de notre machine pour simuler un appareil plus lent. Pour cette dernière option, activez l’option “CPU throttling” ;

* L'outil Performance permet d'analyser les performances d’une page, notamment le taux d’images par seconde d’une animation ;

* On peut utiliser l’onglet Performance pour analyser nos animations, ce qui permet de repérer les problèmes dans notre code qui pourraient causer des problèmes de fluidité sur certains supports ;

* Zoomer sur une image précise d’une animation permet de détailler les calculs effectués par le navigateur, que nous avions vus dans le chapitre sur le fonctionnement du navigateur.

## 	Animez les couleurs de manière performante avec opacity

* Animer la couleur d’une propriété déclenche des calculs de paint ;

* La propriété `opacity`  nous permet de faire des transitions entre des couleurs en évitant ces calculs ;

* La propriété  `opacity`  reçoit une valeur entre 0 et 1, 0 étant complètement transparent et 1 complètement opaque ;

* Pour éviter d’avoir à ajouter des  <div>  supplémentaires, que l'on aurait dû ajouter à chaque fois dans le HTML, on peut utiliser le pseudoélément  `::before`  ou  `::after`  ;

* Pour créer un pseudoélément, ajoutez le nom du pseudoélément à un sélecteur, en utilisant le préfixe double deux-points :  `.selector::after{...}`

* Les pseudo-éléments  ::before  et  ::after  créent un élément qui est respectivement le premier ou le dernier enfant de l’élément sélectionné ; 

* Il est possible de créer des dégradés de couleur. Il suffit d'attribuer un dégradé au background-color de l'élément d'arrière-plan. On fera ensuite disparaître l'élément superposé avec opacity: 0.
