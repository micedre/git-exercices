## Configuration basique de git

Il existe trois catégories de configuration dans git : 
* système: lié à l'installation de git (donc au poste de travail)
* global : lié à l'utilisateur
* local: lié au depot git en cours

On peut voir l'ensemble de cette configuration ainsi que les fichiers où les trouver avec la commande

```sh
git config --list --show-origin
```

---

Pour effectuer un commit avec git il est nécéssaire de renseigner son nom et un email. Si on ne le fait pas manuellement, git essaye de le deviner a partir de l'environnement et affiche le message suivant :
> Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
>You can suppress this message by setting them explicitly:
>
>   git config --global user.name "Your Name"
> 
>    git config --global user.email you@example.com

---

L'éditeur par défaut est utilisé quand on utilise git en ligne de commande, par exemple pour écrire le message de commit. Par défaut, il s'agit de l'éditeur vim qui n'est pas forcément facile à utiliser. 
Cette valeur se change par la commande : 

```sh
git config --global core.editor "<chemin vers un executable>"
```

Par exemple pour utiliser le bloc note, on utilisera la commande :

```
git config --global core.editor notepad.exe
```

(Notez le flag `--global` pour que cette configuration soit valable pour tous vos depot sans impacter les autres utilisateurs du poste de travail)

