## Voir les logs

```
git log -1 -p
```

Permet d'afficher uniquement le dernier commit. `-p` inidque d'afficher aussi le différentiel par rapport au commit parent.

```
git log grep="docs"
```

affichera l'ensemble des commit dont le message contient le mot docs

```
git log --author=Mystere
```

Voir les commit de Mystere
