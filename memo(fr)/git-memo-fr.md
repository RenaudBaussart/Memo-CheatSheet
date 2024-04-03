## Commandes de base :
`git init` - Initialiser un dépôt  
`git clone <repository_url>` - Cloner un dépôt  
`git add <file(s)>` - Ajouter des modifications  
`git commit -m "Message de commit"` - Effectuer un commit  
`git push <remote> <branch_name>` - Pousser les modifications vers un dépôt distant  
`git pull <remote> <branch_name>` - Tirer les modifications d'un dépôt distant  
`git status` - Vérifier l'état du dépôt  

## Branches et Fusion :
`git branch` - Lister toutes les branches du dépôt local  
`git branch <branch_name>` - Créer une nouvelle branche  
`git switch <branch_name>` - Basculer vers une branche  
`git switch -b <branch_name>` - Créer une nouvelle branche et basculer vers elle  
`git merge <branch_name>` - Fusionner des branches dans la branche actuelle  
`git branch -d <branch_name>` - Supprimer une branche  

## Journalisation et Historique :
- `git log` - Afficher l'historique des commits  
    - `--oneline` : Affiche chaque commit sur une seule ligne.
    - `--graph` : Affiche une représentation graphique de l'historique des commits.  
    - `--decorate` : Affiche les noms de branches et les étiquettes associées à chaque commit.  
    - `--author=<pattern>` : Filtre les commits pour afficher uniquement ceux de l'auteur spécifié.  
    - `--since=<date>` : Filtre les commits pour afficher ceux effectués après une certaine date.  
    - `--until=<date>` : Filtre les commits pour afficher ceux effectués avant une certaine date.  
    - `--grep=<pattern>` : Filtre les commits pour afficher ceux dont le message de commit contient le motif spécifié.  
    - `-<n>` ou `--max-count=<n>` : Limite le nombre de commits affichés à `<n>`.  
- `git diff <branch1> <branch2>` - Voir les différences entre les branches
    - `--stat` : Affiche un résumé statistique des modifications apportées par le commit.
    - `--patch` ou `-p` : Affiche les différences entre les fichiers du commit et les fichiers de la version précédente.
    - `-name-only` : Affiche uniquement les noms des fichiers modifiés par le commit.
    - `--name-status` : Affiche les noms des fichiers modifiés et le type de modification (ajouté, modifié, supprimé, etc.).
    - `--decorate` : Affiche les noms de branches et les étiquettes associées au commit.
    - `--oneline` : Affiche le commit sur une seule ligne, avec un résumé du message de commit.
- `git show <commit_id>` - Voir les modifications effectuées dans un commit  
- `git diff`montre les difference exacten entre le active dir et la staging areas  
    - `--staged` la meme que diff mais entre la staging et le dernier commit

## Dépôts distants :
`git remote add <name> <repository_url>` - Ajouter un dépôt distant  
`git remote -v` - Lister les dépôts distants  
`git remote remove <name>` - Supprimer un dépôt distant  

## Annuler des modifications :
`git reset HEAD~1` - Annuler le dernier commit (en conservant les modifications)  
`git checkout -- <file(s)>` - Annuler les modifications dans le répertoire de travail  
`git reset --hard HEAD~1` - Annuler le dernier commit et les modifications  
`git commit --amend` change le message du dernier commit
`git revert [numero du commit]` revien aux commit indique    

## Divers :
Pour ignorer des fichiers, créez un fichier `.gitignore` et répertoriez les fichiers/dossiers à ignorer.  
`git config --list` - Afficher la configuration Git  
`git diff > patch_name.patch`  
`git apply patch_name.patch` - Créer et appliquer un patch  
`git stash` - Mettre en réserve des modifications  
`git stash apply` - Appliquer les modifications mises en réserve  

****que faire quand on a fait une bourde****
```
git reflog
# tu vas voir la list des truc que tu
# a fait dans git sur tout t'est branch
# chacune a un index HEAD@{index}
# trouve celuit avant que tu ais casser le code
git reset HEAD@{index}
# machine a remonter dans le temps magic
```