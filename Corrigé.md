# Gérer les conflits 

```
git log --oneline --graph --all
```
Permet de voir que les 2 branches ont pour base la branche `conflict-merge` et ont un commit d'avance sur celle ci.

Pour voir les fichiers modifier on peut ajouter l'argument `--name-only` à la ligne précédente : 

```
* 72c69ce (conflict-merge2) merge2
| docs/Installation.md
| docs/contribuer.md
| * a897cc1 (conflict-merge1) merge1
|/
|   docs/Installation.md
|   docs/contribuer.md
* 2c743bb (HEAD -> conflict-merge-corrige, conflict-merge) Enoncé
```

Pour fusionner :

```
git checkout conflict-merge2
git merge conflict-merge1
```

Les modifications impactant les mêmes lignes, git ne sait pas résoudre les conflits tout seul. On peut les gérer avec `git mergetool` ou l'éditeur de votre choix.

