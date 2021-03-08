# Exercices git : depot de tests

Ce dépôt contient des exercices sur git sur les différents concepts de l'outils. 
Il est préférable de forker ce dépot pour ne pas être bloqué pour certains exercices utilisant les remotes. Pour cela vous pouvez généralement cliquer sur un bouton `fork` en haut à droite.

## Contexte des exercices

Vous avez été missionné pour rétro documenter une application existante avec votre équipe. Il vous est demandé de documenter en format markdown et utiliser l'outil git pour garder un historique des modifications complet.

## Exercices 

On suppose ici que vous avez déjà installé et configurer l'outil git (si ce n'est pas le cas, voir ici : https://gitlab.insee.fr/animation-developpement/outils-de-dev/-/wikis/Outils/Git_Fiche ).

Chaque exercice se trouve dans une branche dédiée (fournie entre parenthèse dans la liste ci dessous), pour y accéder il faudra donc taper la commande suivante :

```
git checkout nom-de-la-branche
```

Pour chaque exercice le README décrit l'énoncé de l'exercice et les taches à effectuer.

### Configuration de git

* Configuration basique de git (`git-config-basique`)
* Configuration avancée de (`git-config-avance`)

### Premieres commandes git

* Création d'un dépot (`clone-init`)
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
* gérer les branches distantes (`remote-branches`) test-conflit

### Commandes avancées

* Ne valider qu'une partie d'un fichier (`git-add-p`)
* Rebasage intéractif (`git-rebase-i`)
* Bisection (`git-bisect`)

