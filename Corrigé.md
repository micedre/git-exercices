# Premier commit

Une fois les fichiers créés:

```
git add docs/installation.md
git commit
```

Pour ne commiter que le fichier `installation.md` (on commence par l'ajouter à l'index puis on commit ce qui se trouve dans l'index)

```
git add docs/utilisation.md
```

Pour ajouter le fichier `utilisation.md` à l'index

```
git diff --staged
```

Pour voir les différences entre l'état du dépot au dernier commit et l'index.

```
git commit --amend
```

Pour modifier le dernier commit