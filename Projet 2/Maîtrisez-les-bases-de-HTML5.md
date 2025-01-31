# Résumé du Cours: Découvrez les métiers de développeur

## Comprenez la différence entre HTML et CSS

* Le HTML constitue la structure d'une page web.

* Le CSS permet d'ajouter du style.

* Les deux langages se complètent avec un rôle bien défini pour chacun.

* Le navigateur est un logiciel qui permet de lire les langages du Web : HTML et CSS.

* Tous les navigateurs embarquent des outils de développement, dont l'outil d'inspection qui permet d'accéder au HTML et au CSS d'une page.

## Comprenez la différence entre HTML et CSS

* Pour créer une page web, on crée un fichier ayant l'extension  `.html`  , qui pourra être ouvert dans le navigateur web simplement en faisant un double-clic dessus.

* Chaque fichier HTML est constitué de balises.

* Les balises peuvent avoir plusieurs formes :

* `<balise> </balise>`  : balises en paires, elles s'ouvrent et se ferment pour délimiter le contenu (début et fin d'un titre, par exemple) ;

* `<balise>`  : balises orphelines (on ne les insère qu'en un seul exemplaire), elles permettent d'insérer un élément à un endroit précis (par exemple une image).

* Les balises sont parfois accompagnées d'attributs pour donner des indications supplémentaires, ou paramétrer un élément (exemple :  `<img src="photo.jpg">`  ).

* Une page web est constituée de deux sections principales : l'en-tête `<head> </head>`  dont le contenu n'apparaît pas dans l'affichage de la page et le corps `<body> </body>`  qui, lui, apparaît.

## Organisez votre texte

* Le HTML comporte de nombreuses balises qui nous permettent d'organiser le texte de notre page. Ces balises donnent des indications comme “Ceci est un paragraphe”, “Ceci est un titre”, etc.

* Les paragraphes sont définis par la balise  `<p> </p>`  , et les sauts de ligne par la balise orpheline `<br>`.

* Il existe six niveaux de titre, de  `<h1> </h1>`  à  `<h6> </h6>`, à utiliser selon l'importance du titre.

* On peut mettre en valeur certains mots avec les balises  `<strong>`,  `<em>`  et  `<mark>`.

* Pour créer des listes, on doit utiliser la balise  `<ul>`  (liste à puces, non ordonnée) ou  `<ol>`  (liste ordonnée). À l'intérieur, on insère les éléments avec une balise  `<li>`  pour chaque item.

## Créez un lien hypertexte en HTML

* Un lien hypertexte (ou hyperlien) permet de changer de page. Par défaut, il est en bleu et souligné dans le navigateur mais on peut modifier ce style en CSS.

* Pour faire un lien hypertexte vers un site web existant, on utilise la balise  `<a>`  avec l'attribut  href pour indiquer l'adresse de la page web cible. Il s'agit d'un lien absolu. Exemple :  `<a href="https://openclassrooms.com">` .

* Pour faire un lien hypertexte vers une autre page de son site, on utilise la balise `<a>`  avec l'attribut  href pour indiquer le nom du fichier en local. Il s'agit d'un lien relatif. Exemple :  `<a href="page2.html">` .

* Un lien hypertexte peut aussi permettre d'amener vers un endroit précis d'une page. Il faut créer une ancre avec l'attribut  `id`  pour “marquer” cet endroit dans la page, puis faire un lien vers l'ancre comme ceci :  `<a href="#ancre">` .

## Créez un lien hypertexte en HTML

* Il existe plusieurs formats d'images adaptés au Web : PNG, JPG…

* On insère une image avec la balise `<img>`  .

* `<img>` doit obligatoirement comporter au moins ces deux attributs : `src` (source de l'image) et   `alt` (courte description de l'image).

* Il est possible d'afficher une autre version d'une image grâce à un lien qui entoure l’image.
