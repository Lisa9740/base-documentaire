# Pattern Design 

## Qu'est-ce qu'un pattern design?
Un patron de conception (souvent appelé design pattern) est un arrangement caractéristique de modules, reconnu comme bonne pratique en réponse à un problème de conception d'un logiciel.

## Pourquoi utiliser un pattern design?
*     Pour accélérer le processus de développement en fournissant des paradigmes de développement éprouvés.
*     Pour anticiper des problématiques qui peuvent ne devenir visibles que plus tard dans la mise en œuvre.
*     Pour améliorer la lisibilité du code en fournissant une standardisation.

## Type de design pattern 
###    Patron de conception de création ou Creational pattern design en anglais :
Les patrons de création fournissent des mécanismes de création d’objets qui augmentent la flexibilité et la réutilisation du code.
###    Patron de conception de structure ou Strutural design pattern :
Ces patrons vous guident pour assembler des objets et des classes en de plus grandes structures tout en gardant celles-ci flexibles et efficaces.

###    Patron de conception de comportement ou Behavioral  design pattern :
Ces patrons s’occupent des algorithmes et de la répartition des responsabilités entre les objets.

## Exemple de design pattern

### Patron de conception de comportement : Observer
Pourquoi l'utiliser ?
On utilise le pattern Observer quand on doit gérer des évenements.

Dans une classe qui doit déclencher des évenements, on ajoute:

En attribut : une liste d'Observateurs
Une méthode permettant d'ajouter un Observateur dans la liste
Une méthode permettant d'envoyer un signal a tous ses obsevateurs.
"Observateur" est une classe abstraite avec une méthode signal, dont héritent des observateurs "concrets" qui implémentent cette méthode.

Quand l'état de la classe change elle doit envoyer un signal a tout ses observateurs qui doivent effectuer l'action nécessaire en fonction du nouvel état de la classe.

### Patron de conception de création : Factory Method / Fabrique

La "Factory Method" définit une interface pour créer des objets dans une classe mère, mais délègue le choix des types d’objets à créer aux sous-classes.

Pourquoi l'utiliser ? 

Pour permettre l'évolution des composant interne : dans le cas où on ne connaît pas à l'avance les types et dépendances précisent des objets utilisé dans le code. Mais aussi pour étendre les composant interne en redéfinissant la méthode fabrique.

### Patron de conception structurel : 

- Chaîne de responsabilité :

La Chaîne de responsabilité est un patron de conception comportemental qui permet de faire circuler des demandes dans une chaîne de handlers. Lorsqu’un handler reçoit une demande, il décide de la traiter ou de l’envoyer au handler suivant de la chaîne.

Le patron vous propose de relier ces handlers par une chaîne. Chaque handler stocke une référence vers le prochain handler de la chaîne dans l’un de ses attributs. En plus de traiter la demande, les handlers la font passer plus loin dans la chaîne. La demande fait le tour de la chaîne jusqu’à ce que tous les handlers aient eu l’occasion de la traiter.

 - Design Pattern Decorator :
 
 Décorateur est un patron de conception structurel qui permet d’affecter dynamiquement de nouveaux comportements à des objets en les plaçant dans des emballeurs qui implémentent ces comportements.



