# Revenir en arrière sur un commit

```
git add docs/contribuer.md
git commit -m "Ajout contribuer"
```

pour valider le fichier

```
git add docs/contribuer.md
git commit --amend
```
pour modifier le dernier commit et ajouter ce qu'il y a dans l'index (en plus des précédentes modifications).

```
git reset --soft HEAD~
```

Pour revenir au commit précedent tout en gardant l'index du commit annulé.