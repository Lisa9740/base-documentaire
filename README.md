# Pattern Design 

## Qu'est-ce qu'un pattern design?
Un patron de conception (souvent appelé design pattern) est un arrangement caractéristique de modules, reconnu comme bonne pratique en réponse à un problème de conception d'un logiciel.

## Pourquoi utiliser un pattern design?
*     Pour accélérer le processus de développement en fournissant des paradigmes de développement éprouvés.
*     Pour anticiper des problématiques qui peuvent ne devenir visibles que plus tard dans la mise en œuvre.
*     Pour améliorer la lisibilité du code en fournissant une standardisation.

## Exemple de design pattern


### Observer
Pourquoi l'utiliser ?
On utilise le pattern Observer quand on doit gérer des évenements.

Dans une classe qui doit déclencher des évenements, on ajoute:

En attribut : une liste d'Observateurs
Une méthode permettant d'ajouter un Observateur dans la liste
Une méthode permettant d'envoyer un signal a tous ses obsevateurs.
"Observateur" est une classe abstraite avec une méthode signal, dont héritent des observateurs "concrets" qui implémentent cette méthode.

Quand l'état de la classe change elle doit envoyer un signal a tout ses observateurs qui doivent effectuer l'action nécessaire en fonction du nouvel état de la classe.
