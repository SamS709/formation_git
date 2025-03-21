# Formation GIT

## Initialisation du dépôt:

```bash
git init
```

## Ajouter remote

```bash
git remote add origin https://github.com/SamS709/formation_git.git
```
## Observer le statut du git
```bash
git status 
```

## Ajouter des fichiers à un commit dans son état actuel

```bash
git add NomDuFichier1 NomDuFichier2
```

## Enlever des fichier déjà add:

```bash
git rm --cached NomDuFichier1 NomDuFichier2
```

## Enlever tous les fichier déja add:

```bash
git rm -r --cached .
```

forcer:

```bash
git rm -r -f --cached .
```


## Enlever des fichiers d'un commit:
```bash
git restore --staged NomDuFichier1 NomDuFichier2
```

## Pour tout ajouter au commit: (prend tous les fichiers à partir de la racine où le git a été initialisé)
```bash
git add .
```

## Possibilités pour un commit :

### 1:

#### Commit pour figer l'état du fichier
```bash
git commit
```

#### Pour rentrer le commentaire de commit
<p>i => insérer du texte => mon_commit</p>
<p>echap =>commande linuw pour appliquer les modifs =></p> 
<p>:wq     (write and quit)</p>
<p>:q!     (forcer de quitter sans faire de modifs)</p>

### 2:
```bash
git commit -m "mon_commit"
```

## Fixer la branch (ici main)
```bash
git branch -M main
```

## push from origin to main
``` bash
git push -u origin main
```
## Historique des commit
<p>Permet aussi de savoit si on a juste commit (Head -> main) ou si on a commit et push (origin/main)</p>
```bash
git log
```
ou
```bash
git show
``` 
(donne plus d'infos que git log)

## Ecrire un bon commit
```bash
git commmit
PRESS i
titreCommit
Sauter une ligne
texte dans le commit
PRESS echap
    -> :wq! pour write and quit
    -> :q! pour forcer quit sans commit
```

## Les branches

### Visualiser les branches
```bash
git branch
```

### Créer une branche (par convention la première branche dérivée de main est appelée developp)
```bash
git checkout -b developp
```
<p>Il y a une étoile devant la branche dans laquelle on se trouve (v. git branch)</p>

### Push de origin vers new_branch
```bash
git push -u origin new_branch
```

### Merger de new_branch vers main
#### Possibilité 1
<p>Se déplacer dans la branche main</p>
```bash
git checkout main
```
<p>Merger à martir de developp</p>
```bash
git merge developp
```

<p>Pousser sur gitHub</p>
```bash
git push -u origin main
```

#### Possibilité 2
<p>1/  Pull request de developp sur merge à partir de GitHub</p>
<p>2/  Accepter en mergant developp sur main</p>


# Pull request
```bash
git push
```