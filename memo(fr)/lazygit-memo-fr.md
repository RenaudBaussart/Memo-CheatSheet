Voici la traduction du texte en français :

![sectionexplain](res/lazygit/Section-explain.png)

## global
- `flèche haut/bas` : Change la ligne sélectionnée (ne pas sortir de la section).
- `flèche gauche/droite` : Change la section sélectionnée.
- `p` : Effectue un pull depuis l'amont défini.
- `P` : Effectue un push vers l'amont défini.
- `:` : Ouvre une ligne de commande pour exécuter une commande personnalisée.
- `R` : Rafraîchit l'interface utilisateur en mode texte (TUI).
- `z` : Annule la dernière action.
- `q` : Quitte lazygit.
- `esc` : Annule l'action en attente.
- *(personnalisé)* `c-v` : Effectue un commit conventionnel.
- *(personnalisé)* `f2` : Effectue un push vers un dépôt spécifique.

## section 2
- `espace` : Stage/déstage le fichier sélectionné.
- `c` : Effectue un commit du fichier mis en scène sélectionné.
- `e` : Édite le fichier sélectionné (nécessite Vim).
- `s` : Stashe le fichier sélectionné.
- `S` : Affiche les options de stash.
- `f` : Fait un fetch depuis l'amont.
- `o` : Ouvre le fichier dans un visualiseur de fichiers.
- `M` : Ouvre l'outil de fusion externe.
- *(personnalisé)* `f1` : Effectue un pull depuis une branche et un dépôt spécifiques.

## section 3
- `espace` : Checkout vers la branche sélectionnée.
- `M` : Fusionne la branche sélectionnée dans la branche actuelle.
- `d` : Supprime la branche sélectionnée.
- `R` : Renomme la branche sélectionnée.
- `s` : Change l'ordre de tri.
- `u` : Affiche et sélectionne l'option d'amont pour la branche sélectionnée.
- `O` : Change l'option de demande de tirage.
- `o` : Crée une demande de tirage.
- `F` : Checkout forcé.
- `r` : Rebase la branche sélectionnée.

## section 4
- `r` : Revoit le commit sélectionné.
- `t` : Crée un commit de reversion pour le commit sélectionné.
- `C` : Copie le commit sélectionné (cherry-pick).
- `V` : Colle le commit copié (cherry-pick).
- `i` : Démarre le rebase interactif.

## section 5
- `g` : Pop.
- `d` : Drop.
- `n` : Nouvelle branche.
- `r` : Renomme le stash.
- `entrée` : Affiche le fichier.