## Feuille de triche

| Commande | Fonction | Exemple |
| --- | --- | --- |
| **Configuration & Initialisation** | | |
| `git init` | Initialise un dépôt Git dans le dossier courant | |
| `git clone [url]` | Récupère l'entièreté d'un dépôt distant via URL | `git clone git@github.com:Simplon-hdf/cheats-sheets-git-flow.git` |
| **Index** | | |
| `git status` | Affiche les fichiers modifiés dans le répertoire de travail | |
| `git add [fichier]` | Déplace un fichier dans la zone de stage | `git add example.md` |
| `git reset [fichier]` | Enlève un fichier de l'index tout en gardant les changements dans le répertoire de travail | `git reset example.md` |
| `git diff` | Différence des changements en dehors de l'index | |
| `git diff --staged` | Différence entre l'index et le dernier commit | |
| `git diff [branche locale] [branche distante]` | Compare les différences entre une branche locale et distante | `git diff develop main` |
| `git commit -m [message]` | Effectue le commit contenant les fichiers dans l'index | `git commit -m "Renamed example.md"` |
| **Branches** | | |
| `git branch -av` | Liste les branches. Un * apparaîtra à côté de la branche actuelle | |
| `git branch [branche]` | Crée une nouvelle branche | `git branch main` |
| `git switch [branche]` | Change la branche courante | `git switch develop` |
| `git branch -d [branche]` | Supprime la branche locale | `git branch -d develop` |
| `git checkout --track` | Crée une nouvelle branche locale à partir d'une branche distante, et la suit | |
| `git tag [nom-du-tag]` | Crée un tag sur le commit actuel | `git tag v1.0` |
| **Historique** | | |
| `git log` | Affiche l'historique des commits | |
| `git log -p [fichier]` | Affiche l'historique des commits sur un fichier spécifique | `git log -p example.md` |
| `git blame [fichier]` | Affiche l'historique des modifications, y compris l'auteur sur un fichier spécifique | `git blame example.md` |
| **Mise à jour & Publication** | | |
| `git remote -v` | Liste les remote configurés | |
| `git remote show [remote]` | Affiche les informations de la remote | `git remote show origin` |
| `git remote add [remote] [url]` | Permet de créer une connexion avec un dépôt distant sous un raccourci | `git remote add origin git@github.com:Simplon-hdf/cheats-sheets-git-flow.git` |
| `git fetch [remote]` | Récupère toutes les modifications de la remote sans fusionner les changements | `git fetch origin` |
| `git pull [remote] [branche]` | Récupère les modifications de la branche, et les fusionne | `git pull origin main` |
| `git push [remote] [branche]` | Pousse les commits d'une branche locale vers un dépôt distant | `git push origin main` |
| **Fusionner & Rebaser** | | |
| `git merge [branche]` | Fusionne la branche spécifiée avec la branche actuelle | `git merge main` |
| `git rebase [branche]` | Réapplique l'historique des commits de la branche actuelle au dessus de la branche spécifiée | `git rebase main` |
| `git rebase --abort` | Annule le processus de rebase en cours | |
| `git rebase --continue` | Poursuit le processus de rebase après la résolution des conflits | |
| `git mergetool` | Ouvre un outil de fusion pour résoudre les conflits | |
| **Annuler/Rétablir** | | |
| `git reset --hard HEAD` | Réinitialise l'index et le répertoire de travail au commit référencé par HEAD | `git reset --hard @~1` |
| `git checkout HEAD [fichier]` | Restaure un fichier spécifique dans le répertoire de travail au dernier commit (HEAD) | `git checkout HEAD example.md` |
