# Résumé du Cours: Réalisez des animations dynamiques avec les @keyframes

## Créez des animations plus complexes avec la règle CSS @keyframes

* Les animations @keyframes nous permettent de construire des animations plus complexes en créant plusieurs étapes pour les propriétés tout au long de l'animation ;

* Les keyframes CSS sont instanciées à l'aide de la règle @keyframes suivie d'un nom pour l'ensemble des keyframes : `@keyframes example-frames {...}` ;

* Chaque keyframe peut être établi en utilisant comme valeur le pourcentage d'animation réalisé : 33% {...} ;

* Si vous n'avez besoin que d'un keyframe de début et de fin, les mots clés « from » et « to » peuvent être utilisés à la place de 0 % et 100 % respectivement ;

* Si aucun keyframe de début ou de fin n'est fourni, l'animation commence et/ou se termine avec les valeurs de propriété assignées au sélecteur. Si aucune valeur n'est explicitement assignée dans le sélecteur, c'est la valeur par défaut qui est choisie ;

* Une animation définie par la règle @keyframes peut contenir différents keyframes avec des propriétés distinctes ;

* Plusieurs pourcentages peuvent être assignés à un seul keyframe. Les valeurs définies dans ce keyframe seront appliquées à ces pourcentages dans l'animation ;

* Les propriétés et valeurs d'un ensemble de keyframes remplaceront les valeurs de propriétés attribuées à un sélecteur au cours de l'animation.

## Utilisez les propriétés de l'animation CSS

* Les animations CSS @keyframes peuvent être déclenchées en utilisant des pseudoclasses telles que  `:hover`, tout comme les transitions ;

* Les @keyframes CSS peuvent également être déclenchés par le chargement des éléments auxquels ils sont assignés, comme un sélecteur. Par exemple, dès le chargement d'une page ; 

* Nous pouvons retarder le démarrage des animations avec keyframes en utilisant la propriété  `animation-delay`, avec un délai exprimé en secondes ou en millisecondes, tout comme les transitions ;

* Nous pouvons étendre ces valeurs du début à la fin de ces animations en utilisant la propriété  `animation-fill-mode` :

* Le mot clé `« backwards »` prolonge les valeurs de départ d'une animation avant son lancement, couvrant la durée du délai assigné avant que l'animation elle-même ne commence,

* Le mot clé `« forwards »` prolonge les valeurs finales d'une animation jusqu'à ce que la page soit rechargée ou que le navigateur soit fermé,

* Le mot clé `« both »` prolonge l'animation dans les deux sens ;

* Nous pouvons définir une fonction de timing des @keyframes en utilisant la fonction animation-timing-function sur le sélecteur où l'animation a été assignée ;

* Nous pouvons également définir un timing spécifique keyframe par `keyframe`, en assignant la propriété  `animation-timing-function`  aux keyframes en question.

## Manipulez et réutilisez les animations CSS

* Nous pouvons répéter un ensemble de keyframes autant de fois que nous le souhaitons en utilisant la propriété  `animation-iteration-count`, avec le nombre de cycles comme valeur ;

* Nous pouvons régler nos keyframes pour qu'ils se répètent à l'infini en utilisant la propriété  `animation-iteration-count`  avec le mot clé « infinite » ;

* La propriété  `animation-direction`  nous permet de lire un ensemble de keyframes normalement, avec le mot clé « normal » ;

* La propriété  `animation-direction`  nous permet de lire un ensemble de keyframes vers l'arrière avec le mot clé « reverse » ;

* La propriété  `animation-direction`  nous permet de lire un ensemble de keyframes avec des allers-retours avec le mot clé « alternate » ;

* Et enfin, la propriété  animation-direction  nous permet de lire un ensemble de keyframes avec des allers-retours, mais en commençant par la fin avec le mot clé « alternate-reverse » ;

* Nous pouvons mettre en pause une animation avec `keyframe` en assignant à la propriété  `animation-play-state`  la valeur réglée sur « paused » ;

* Nous pouvons reprendre la lecture d'une animation avec keyframe en assignant la propriété  `animation-play-state`  avec la valeur réglée sur « running ».

## Affinez vos animations CSS avec DevTools

* Itérer, c’est le secret d'une bonne animation. Le simple fait d'ajouter quelques chiffres et d'appuyer sur Enregistrer est rarement suffisant ;

* Notre expérience nous donne une bonne intuition quant aux valeurs de départ qui paraissent bien pour nos propriétés d'animation ;

* Le panneau Animations de DevTools nous permet d'affiner rapidement les animations, d'improviser et d'expérimenter jusqu'à ce que nous trouvions la bonne durée ou le bon délai pour un élément ;

* Le panneau Changes (Modifications) nous permet de voir les propriétés que nous avons modifiées ainsi que leurs nouvelles valeurs, de façon à mettre à jour notre code source en conséquence. 
