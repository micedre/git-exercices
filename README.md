# Exercices git : dépôt de tests

Ce dépôt contient des exercices sur git sur les différents concepts de l'outils. 
Il est préférable de créer un fork de ce dépôt pour ne pas être bloqué pour certains exercices utilisant les remotes. Pour cela vous pouvez généralement cliquer sur un bouton `fork` en haut à droite.

Ce dépôt permet de manipuler l'outil de façon un peu guidée, mais n'a pas vocation à aborder l'ensemble des fonctionnalité de `git`; la lecture du livre [Pro Git](https://git-scm.com/book) est fortement conseillée. 

## Contexte des exercices

Vous avez été missionné pour rétro documenter une application existante avec votre équipe. Il vous est demandé de documenter en format markdown et utiliser l'outil git pour garder un historique des modifications complet.

## Exercices 

On suppose pour toutes la suite que vous avez déjà installé et configurer l'outil `git`. Si ce n'est pas le cas,  Vous pouvez le [télécharger](https://git-scm.com/downloads).

Chaque exercice se trouve dans une branche dédiée (fournie entre parenthèse dans la liste ci dessous), pour y accéder il faudra donc taper la commande suivante :

```
git checkout nom-de-la-branche
```

Pour chaque exercice le README décrit l'énoncé de l'exercice et les taches à effectuer.

### Configuration de git

* Configuration basique de git (`git-config-basique`)
* Configuration avancée de (`git-config-avance`)

### Premieres commandes git

* Création d'un dépôt (`clone-init`)
* Mon premier commit (`premier-commit`)
* Voir les logs (`git-log`)
* Ignorer des fichiers (`git-ignore`)
* Gérer des dépôts distants (`remote-basic`)
* Revenir en arrière sur un commit (`git-oups`)
* Créer un tag (`git-tag`)

### Gestion des branches

* Création, suppression de branche git (`gestion-branche`)
* Fusionner des branches (fast-forward) (`ff-merge`)
* Fusionner des branches (3-way) (`3-way-merge`)
* Fusionner des branches (conflit) (`conflict-merge`)
* Rebaser (`git-rebase`)
* gérer les branches distantes (`remote-branches`) test test

### Commandes avancées

* Ne valider qu'une partie d'un fichier (`git-add-p`)
* Rebasage intéractif (`git-rebase-i`)
* Bisection (`git-bisect`)

