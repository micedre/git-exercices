# gérer les branches

``` 
git checkout gestion-branche
git checkout -b feat/add-construction-doc
```

On crée la branche `feat/add-constrution-doc` à partir de la branche courante (ici `gestion-branche` )

On peut maintenant rajouter et valider un fichier "construction.md"

---

```
git branch -f issue/fix-typo gestion-branche
```

permet de créer la branche `issue/fix-typo` à partir de la branche `gestion-branche` et non plus à partir de la branche courante.

```
git checkout issue/fix-typo
```
Pour passer HEAD sur cette branche

---

```
git log --oneline --graph --all
```

pour voir les différentes branches et embranchements de l'historique git

Par exemple :

```
* 80bb8db (issue/fix-typo) typo
* 87078fd Typo
| * a6bdbce (feat/add-construction-doc) add construction
|/
* 1c0f5e1 (HEAD -> gestion-branche-corrige, gestion-branche) Enoncé
```