# Formation GIT

## Initialisation du dépôt:

'''bash
git init
'''

## Ajouter remote

'''bash
git remote add origin https://github.com/SamS709/formation_git.git
'''
## Observer le statut du git
'''bash
git status 
'''

## Ajouter des fichiers à un commit dans son état actuel

'''bash
git add NomDuFichier1 NomDuFichier2
'''

## Enlever des fichiers d'un commit:
'''bash
git restore --staged NomDuFichier1 NomDuFichier2
'''

## Pour tout ajouter au commit: (prend tous les fichiers à partir de la racine où le git a été initialisé)
'''bash
git add .
'''

## Possibilités pour un commit :

### 1:

#### Commit pour figer l'état du fichier
'''bash
git commit
'''

#### Pour rentrer le commentaire de commit
i => insérer du texte => mon_commit
echap =>commande linuw pour appliquer les modifs => 
:wq     (write and quit)
:q!     (forcer de quitter sans faire de modifs)

### 2:
'''bash
git commit -m "mon_commit"
'''

## Fixer la branch (ici main)
'''bash
git branch -M main
'''

## push from origin to branch
''' bash
git push -u origin main

## Historique des commit
'''bash
git log
'''
ou
'''bash
git show
''' (donne plus d'infos que git log)

## Ecrire un bon commit

