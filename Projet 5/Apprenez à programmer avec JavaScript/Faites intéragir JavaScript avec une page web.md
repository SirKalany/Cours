## Récupérez un élément d’une page web

* Une page web est constituée de balises HTML, et repose sur une structure que l’on appelle DOM. Cette structure permet de relier les balises entre elles.

* Pour récupérer un élément du DOM :
  - utilisez defer dans l’inclusion de vos fichiers JS pour retarder leur prise en compte, afin que la variable document ait le temps d’être créée ;
  - partez du point d’entrée du DOM : la variable document ;
  - utilisez les méthodes adaptées : getElementById, querySelector ou querySelectorAll.

## Modifiez un élément d’une page web

* Utilisez des attributs pour configurer les éléments HTML d’une page web.

* Modifiez la valeur des attributs :
  - en utilisant la méthode setAttribute ;
  - en utilisant la syntaxe : elementHtml.nomAttribut = “nouvelle valeur d’attribut”.

## Créez un nouvel élément dans une page web

* Créez un nouvel élément HTML :
  - en utilisant la méthode createElement puis en liant l’élément créé à la page grâce à appendChild ;
  - en utilisant la propriété innerHTML pour insérer directement du HTML sous forme de texte à l’intérieur d’une balise.

* L’interpolation permet de générer facilement des chaînes de caractères complexes en utilisant des backticks.

## Interagissez avec un élément d’une page web grâce aux événements

* La programmation événementielle consiste à écrire du code qui réagit à des événements.

* Un événement est un signal envoyé par l’élément HTML lorsque l’utilisateur effectue une action (clic, frappe au clavier…).

* Pour savoir quand un événement est envoyé, vous devez attacher un écouteur à l’élément HTML.

* Pour gérer un événement, vous devez l’écouter en utilisant la méthode AddEventListener.

* Vous pouvez récupérer des informations sur un événement en utilisant la variable event.
