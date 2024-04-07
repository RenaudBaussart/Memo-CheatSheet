## Cheat Sheet

---

| Commande | Fonction | Exemple |
| --- | --- | --- |
| **Configuration & Initialisation** | | |
| `git flow init` | Initialise un dossier .git vide, dans le dépôt courant et déplace l'utilisateur sur la branche develop | |
| **Branches** | | |
| `git flow feature start [branche]` | Crée une branche de feature et en fait la branche courante | `git flow feature start header` |
| `git flow feature finish [branche]` | Fusionne la branche de feature sur la branche develop, et supprime la branche feature | `git flow feature finish header` |
| `git flow hotfix start [branche]` | Crée une branche de déboggage et en fait la branche courante | `git flow hotfix start fix-api-url` |
| `git flow hotfix finish [branche]` | Fusionne la branche hotfix à la branche main et develop, et supprime la branche hotfix | `git flow hotfix finish fix-api-url` |
| `git flow release start [numero de version]` | Crée une nouvelle branche de release à partir de la branche develop | `git flow release start 1.0.0` |
| `git flow release finish [numero de version]` | Fusionne la branche release sur la branche main et supprime la branche release | `git flow release finish 1.0.0` |
| **Partage de branche** | | |
| `git flow feature publish [branche]` | Pousse la branche feature sur le dépôt distant | `git flow feature publish header` |
| `git flow feature pull [remote] [branche]` | Récupère une branche d'un dépôt distant | `git flow feature pull origin menu` |