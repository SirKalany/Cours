# Résumé du Cours: Créez un formulaire de saisie de données

## Récupérez la valeur d’un champ de formulaire

* Utilisez les formulaires pour permettre à l'utilisateur de saisir des informations. 

* Vous pouvez utiliser différent types de champs pour saisir ces informations :

  - input de différents types (texte, numérique, radio, case à cocher…)
  - textarea
  - select.

* Pour récupérer la valeur d’un champ, utilisez différentes options en fonction de votre contexte :

  - pour la plupart des champs : utilisez la propriété value
  - pour les cases à cocher : utilisez la propriété checked
  - pour récupérer la valeur des boutons radio, parcourez-les jusqu’à trouver celui qui est coché, puis utilisez la propriété value sur ce bouton.
 
## Soumettez votre formulaire

* Un navigateur est un client HTTP. Il fait appel au serveur pour récupérer les informations sur la page qu’il veut afficher.

* Lorsqu’un utilisateur valide un formulaire, l’événement submit est envoyé.

* Lorsqu'un événement submit est envoyé, par défaut, il provoque un appel au serveur. Cela génère un rechargement de la page qui empêche l'exécution du code.

* Pour éviter ce comportement par défaut :

  - écoutez l’événement submit ;
  - empêchez le comportement avec la méthode preventDefault.
 
## Mettez en place des règles de validation 

* Mettez en place des règles de validation pour vous assurer que l’utilisateur a correctement saisi ses données :

  - vérifiez la valeur d’un champ pour les cas simples ;
  - définissez des expressions régulières pour les cas plus complexes.
 
* Vous pouvez tester vos champs :

  - à l’envoi du formulaire grâce à l’événement submit ;
  - à la saisie d’un champ du formulaire grâce aux événements input ou change.
 
* Définissez vos expressions régulières étape par étape en vous aidant des sites ci-dessous : 

  - regex101.com pour tester votre expression ;
  - Regexper pour visualiser votre expression.
 
## Affichez un message d’erreur

* En tant que développeur, veillez à traiter toutes les erreurs qui pourraient survenir dans le code : 

  - grâce à if / else pour les erreurs courantes ;
  - en centralisation la gestion des erreurs grâce aux exceptions try, catch et throw pour les situations plus complexes.
 
* Le bloc try catch fonctionne en deux parties :

  - un bloc try qui essaie d’exécuter une portion de code ;
  - un bloc catch qui est lancé si jamais un élément du bloc try a lancé une exception.
 
* Vous pouvez utiliser throw new Error(message) pour lancer vous-même vos exceptions.
