## gérer les branches (3-way-merge)

* chacune des branches 3-way-merge1 et 3-way-merge2 est partie dela branche 3-way-merge et ont 2 commit d'avance sur celle ci

```
git checkout 3-way-merge2
git merge 3-way-merge1
```
Pour fusionner 3-way-merge1 dans 3-way-merge2
Point notable, meme si 2 commit différents concernaient le meme fichier (Enoncé). Ces modifications étaient suffisamment espacées pour que git sache les gérer tout seul sans générer de conflits.
```
Auto-merging Enoncé.md
Merge made by the 'recursive' strategy.
 "Enonc\303\251.md" | 8 +++++++-
 merge1             | 1 +
 2 files changed, 8 insertions(+), 1 deletion(-)
 create mode 100644 merge1
```

On obtient ensuite :

```
*   b7a8b8a (HEAD -> 3-way-merge2) Merge branch '3-way-merge1' into 3-way-merge2
|\
| * 0148d61 (3-way-merge1) README
| * 8f4330a fichier merge1
* | 5cfe3f5 Enoncé merge2
* | 6c61491 merge2
|/
* e02d9c0 (3-way-merge)  Enoncé
```