# Gérer les branche (Fast Forward Merge)

```
git log --oneline --graph --all
```
Pour afficher l'arbre de l'historique. On observe que ff-merge2 a 2 commit d'avance sur ff-merge

```
git checkout ff-merge
git merge ff-merge2
```

pour fusionner la branche ff-merge2 dans la branche courante (ici ff-merge). Comme aucun commit nouveau n'avait été ajouté depuis la création de la branche ff-merge2, git a simplement repris les commit pour les ajouter sur la branche ff-merge.

