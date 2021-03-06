## Configuration avancé de git

Les alias permettent de donner des noms courts à des lignes de commandes potentiellement complexe.
Ici, une solution possible est 

```
git config --global alias.gl "log --oneline --graph --all"
```
---

Par exemple avec kdiff3 (https://download.kde.org/stable/kdiff3/) : 

```
[merge]
	tool = kdiff3
[mergetool "kdiff3"]
	path = <chemin/vers/kdiff3.exe>
[mergetool]
        prompt = false
        keepBackup = false
        keepTemporaries = false
[diff]
	tool = kdiff3
[difftool "kdiff3"]
	path = <chemin/vers/kdiff3.exe>
[difftool]
        prompt = false
        keepBackup = false
        trustExitCode = false
```



testable par exemple avec : 

```
git difftool HEAD git-config-basique --tool=kdiff3
```
---

Les hooks sont à placer dans le dossier
`.git/hooks`. Il s'agit de renommer le fichier que l'on souhaite et de rajouter le script voulu.

Ici on souhaite valider le message de commit, il faut donc le hook *commit-msg* dans lequel on peut par exemple passer le script : 

```
grep -q -e '\[A-Z\] .*' "$1" || {
	echo >&2 Wrong format for commit message
	exit 1
}
```