# Résumé du Cours: Réalisez vos premières animations CSS

* vous pouvez créer vos animations CSS sur vos propres éditeurs de code, ou bien sur des outils de code en ligne tels que CodePen ou CodeSandbox ;

* L'animation a été démocratisée auprès du grand public par Disney ; les techniques d'animation web n'ont cessé d'évoluer depuis les débuts du web : GIF, Flash, etc. ; aujourd'hui, il existe de nombreuses techniques d'animation web : JavaScript, SVG, Canvas, WebGL mais surtout CSS ; l'animation permet d'ajouter de la vie à une page web, et ainsi de vraiment impacter l'expérience d'un utilisateur sur cette page.

## Créez des animations simples avec les transitions

* Les 5 éléments nécessaires pour créer une transition sont :

* Une propriété CSS à modifier, une valeur initiale pour votre propriété CSS, une valeur finale pour cette même propriété, une durée et une pseudoclasse pour déclencher l’animation ;

* On applique la valeur initiale à l’élément qu’on veut modifier, et la valeur finale dans la pseudoclasse qui déclenche la transition ;

* La durée peut s’exprimer en secondes : 0.4s, ou en millisecondes : 400ms ;

* Les propriétés d’une transition peuvent être déclarées individuellement : `transition-duration: 400ms`  ;

## Déclenchez vos transitions avec les pseudoclasses

* Les pseudoclasses sont essentielles pour déclencher des transitions en CSS ;

* Les pseudoclasses les plus adaptées pour déclencher des transitions sont celles qui impliquent une interaction avec l’utilisateur ;

* Les pseudoclasses les plus courantes pour déclencher une transition sont  `:hover,  :active,  :focus,  :valid,  :invalid,  :not(),  :checked,  :enabled, `et`  :disabled`

* On peut combiner des pseudoclasses entre elles pour créer des sélecteurs plus précis ;

* Les pseudoclasses peuvent aussi être utilisés pour changer le style d’un élément voisin.

## Appliquez les 12 principes de l’animation au web

* Les 12 principes de l'animation sont :

* Squash and Stretch, pour compresser et étirer un élément ;

* Anticipation, pour préparer l’audience à un mouvement à venir ; 

* Staging (mise en scène), pour guider les yeux de l’utilisateur vers les éléments importants d’une page ;

* Straight Ahead and Pose to Pose (toute l'action d'un coup et partie par partie), qui correspond davantage à l'animation traditionnelle mais fait penser à la différence transitions/keyframes ; 

* Follow Through and Overlapping Action (continuité du mouvement initial et chevauchement de deux mouvements consécutifs), pour faire accélérer et décélérer un élément en fonction de sa masse ; 

* Slow in and slow out (ralentissement en début et en fin de mouvement), basé sur le fait que les objets ne démarrent pas et ne s’arrêtent pas instantanément ;

* Arc, pour créer des mouvements naturels ;

* Secondary Action (action secondaire), pour séparer différentes parties d’une scène dans une animation ;

* Timing, pour faire se déplacer les objets à une vitesse crédible ;

* Exaggeration (exagération), pour donner du caractère et de la personnalité à une animation ; 

* Solid Drawing (notion de volume), pour que les animations correspondent au résultat souhaité ;

* Appeal (charisme), pour rendre les animations plus dynamiques.

## Créez des transitions CSS à propriétés multiples

* il est possible d’animer autant de propriétés que l’on veut avec les transitions ;

* le mot clé   `all`  permet d’appliquer des transitions simultanément à toutes les propriétés ;

* ou bien on peut séparer les animations par des virgules, ce qui permet de leur donner des valeurs différentes. Exemple :  `transition: transform 450ms, background-color 300ms`;

* on peut décaler le départ des transitions avec  `transition-delay` ;

* la valeur de  `transition-delay`  peut également être définie directement dans la propriété  `transition`.

## Créez des animations plus naturelles avec les fonctions de timing

* L’accélération et la décélération des transitions sont contrôlées par la propriété  transition-timing-function ;

* Si aucune fonction de timing n’est indiquée, la transition utilisera la fonction  ease. Elle suit un profil d’accélération plus net, et une rampe de décélération plus prononcée ;

* Parmi les autres mots clés pour les fonctions de temporisation, on peut trouver  `ease-in`,   `ease-out`,   `ease-in-out`, et  `linear` ;

* Quand aucune fonction de timing par défaut ne correspond à l’animation, il est possible de créer ses propres courbes d’animation personnalisée à l’aide de la fonction  cubic-bezier()  ;

* Il existe des outils pour ajuster les effets de timing avec la fonction  `cubic-bezier()`
