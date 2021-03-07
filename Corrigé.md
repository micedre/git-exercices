# Créer un tag

```
git tag 2.0
```

Pour creer le tag `2.0` relatif au dernier commit

```
git tag 2.0 -m "Version 2.0" -a -f
```

Pour recréer le tag 2.0 avec la description "Version 2.0" 

```
git checkout 1.0
git switch -c release-1
<modify>
git add .
git commit -m "Bug fix"
git tag 1.1 -a -m "Version 1.1"
```

Pour récuperer le tag 1.0. Il faut ensuite créer une branche à partir de ce tag, pour garder les commit. Enfin, on fait les modifications necessaires puis on retag.
