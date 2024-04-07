## memo

| Commande | Fonction | Exemple |
| --- | --- | --- |
| **Configuration & Initialisation** | | |
| `git flow init` | Initialise un dossier .git vide dans le dépôt courant et bascule l'utilisateur sur la branche develop | |
| **Branches** | | |
| `git flow feature start [branche]` | Crée une branche de fonctionnalité et la définie comme branche courante | `git flow feature start header` |
| `git flow feature finish [branche]` | Fusionne la branche de fonctionnalité dans la branche develop et supprime la branche de fonctionnalité | `git flow feature finish header` |
| `git flow hotfix start [branche]` | Crée une branche de correctif et la définie comme branche courante | `git flow hotfix start fix-api-url` |
| `git flow hotfix finish [branche]` | Fusionne la branche de correctif dans les branches main et develop, et supprime la branche de correctif | `git flow hotfix finish fix-api-url` |
| `git flow release start [numéro de version]` | Crée une nouvelle branche de release à partir de la branche develop | `git flow release start 1.0.0` |
| `git flow release finish [numéro de version]` | Fusionne la branche de release dans la branche main et supprime la branche de release | `git flow release finish 1.0.0` |
| **Partage de Branche** | | |
| `git flow feature publish [branche]` | Pousse la branche de fonctionnalité vers le dépôt distant | `git flow feature publish header` |
| `git flow feature pull [remote] [branche]` | Récupère une branche d'un dépôt distant | `git flow feature pull origin menu` |