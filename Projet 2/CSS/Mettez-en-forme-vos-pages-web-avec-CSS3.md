# Résumé du Cours: Mettez en forme vos pages web avec CSS3

## Intégrez le CSS dans la page HTML

* CSS est un autre langage qui vient compléter le HTML. Son rôle est de mettre en forme votre page web.

* Pour écrire le code CSS, on crée un fichier séparé portant l'extension `.css`  comme `style.css`.

* Pour lier les fichiers CSS et HTML, on rajoute une ligne dans la balise `<head> </head>` du fichier HTML :  `<link href="style.css" rel="stylesheet">`

* En CSS, on sélectionne les portions de la page HTML qu'on veut modifier, et on change leur présentation avec des propriétés CSS :

balise1
{
    propriete1: valeur1;
    propriete2: valeur2;
}

* Il existe plusieurs façons de sélectionner la portion de page que l'on veut mettre en forme. Par exemple, on peut viser :

* toutes les balises d'un même type, en écrivant simplement leur nom (`h1` par exemple) ;

* certaines balises spécifiques, auxquelles on a donné des noms à l'aide des attributs `class` ou `id` (`.nom-classe` ou `#nom-id`) ;

* uniquement les balises qui se trouvent à l'intérieur d'autres balises (`h3`,`em`).

## Changez l'apparence du texte

* On modifie la taille du texte avec la propriété CSS `font-size`.

* On peut indiquer la taille en pixels, comme `16px` ; ou encore en “em”, comme `1.3em`.

* On indique la police du texte avec la propriété CSS  `font-family` . 

* De nombreuses propriétés de mise en forme du texte existent : font-style pour l'italique, font-weight pour la mise en gras, text-decoration pour le soulignement.

* Le texte peut être aligné avec la propriété CSS `text-align`  .

## Ajoutez de la couleur et un fond

* On change la couleur du texte avec la propriété  color  et la couleur de fond avec la propriété `background-color`.

* On peut indiquer une couleur en écrivant son nom en anglais, `black` par exemple, sous forme hexadécimale, comme  `#FFC8D3`, ou en notation RGB, comme `rgb(250,25,118)`.

* On peut ajouter une image de fond avec la propriété `background-image`. On peut choisir de fixer l'image de fond, ou encore de la positionner où on veut sur la page.

* On peut rendre une portion de la page transparente avec la propriété  `opacity`  ou avec la notation  RGBA  (une extension de la notation RGB, où la quatrième valeur indique le niveau de transparence).

## Créez des bordures et des ombres

* On peut appliquer une bordure à un élément avec la super-propriété CSS  `border`. Il faut indiquer la largeur de la bordure, sa couleur et son type (simple, double, pointillés, tirets).

* On peut arrondir les bordures avec la propriété CSS  `border-radius`.

* On peut ajouter une ombre aux blocs de texte avec  `box-shadow`. On doit indiquer le décalage vertical et horizontal de l'ombre, son niveau d'adoucissement et sa couleur.

* Le texte peut lui aussi avoir une ombre avec  `text-shadow`.

## Créez des apparences dynamiques

* En CSS, on peut modifier l'apparence de certaines sections dynamiquement, après le chargement de la page, lorsque certaines interactions se produisent. On utilise pour cela les pseudo-classes.

* La pseudo-classe  `:hover`   modifie l'apparence d'un élément au survol (par exemple : `a:hover`  modifie l'apparence des liens hypertextes lorsque la souris pointe dessus).

* La pseudo-classe  `:active`  modifie l'apparence des liens hypertextes au moment du clic.

* La pseudo-classe `:visited` modifie l'apparence des liens hypertextes lorsqu'un lien a déjà été visité.

* La pseudo-classe  `:focus`  modifie l'apparence d'un élément sélectionné via la touche "tab".

* Encore aujourd'hui, certaines propriétés ne sont pas totalement reconnues par tous les navigateurs.
