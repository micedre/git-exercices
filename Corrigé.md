# Gérer les dépots distants

```
git remote -v
```

Permet d'afficher les dépots distants configurés localement. Par défaut, lors d'un clone, le dépot distant qui a servi au clone est enregistré avec comme nom `origin`

```
git remote add dossier "<chemin vers copie>"
```

permet de configurer un dépot distant ayant pour nom `dossier` pointant vers le nouveau dossier.

```
git push dossier remote-basic
```

Permettra de pousser les commit vers ce nouveau depot distant