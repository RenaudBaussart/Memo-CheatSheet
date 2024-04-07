### Navigation dans le système de fichiers
- `ls` : Liste les fichiers et répertoires dans le répertoire actuel.
    - `-l` : Format de liste longue, affichant des informations supplémentaires sur les fichiers.
    - `-a` : Inclure les fichiers cachés (ceux commençant par un point).
    - `-h` : Affiche les tailles de fichiers au format lisible par l'homme.
    - `-t` : Trie les fichiers par heure de modification.
    - `-r` : Inverse l'ordre du tri.
    - `-R` : Liste récursivement les sous-répertoires rencontrés.
- `cd [nom_du_répertoire]` : Change le répertoire de travail.
- `pwd` : Affiche le chemin du répertoire actuel.
- `cat [nom_du_fichier]` : Affiche le contenu du fichier.
- `less [nom_du_fichier]` : Affiche le contenu du fichier une page à la fois.
    - `Barre d'espace` : Avance d'une page.
    - `b` : Recule d'une page.
    - `/motif` : Recherche vers l'avant pour la prochaine occurrence du motif.
    - `?motif` : Recherche vers l'arrière pour l'occurrence précédente du motif.
    - `q` : Quitte less.
- `head [nom_du_fichier]` : Affiche les premières lignes d'un fichier.
    - `-n [num]` : Affiche les [num] premières lignes du fichier.
- `tail [nom_du_fichier]` : Affiche les dernières lignes d'un fichier.
    - `-n [num]` : Affiche les [num] dernières lignes du fichier.
    - `-f` : Affiche les données ajoutées au fur et à mesure que le fichier augmente de taille (tail -f).
- `grep [motif] [nom_du_fichier]` : Recherche un motif dans un fichier.
    - `-i` : Ignore les distinctions de cas dans le motif et les fichiers d'entrée.
    - `-v` : Inverse la correspondance, sélectionnant les lignes non correspondantes.
    - `-n` : Précède chaque ligne de sortie du numéro de ligne basé sur 1 dans son fichier d'entrée.
    - `-r` : Recherche récursivement les sous-répertoires répertoriés.

### Manipulation de fichiers

- `touch [nom_du_fichier]` : Crée un nouveau fichier vide.
- `nano [nom_du_fichier]` : Ouvre le fichier dans l'éditeur de texte Nano.
- `mkdir [nom_du_répertoire]` : Crée un nouveau répertoire.
- `rm [nom_du_fichier]` : Supprime un fichier.
    - `-rf ` : Supprime tous les enfants de ce fichier ou répertoire.
- `rmdir [nom_du_répertoire]` : Supprime un répertoire vide.
- `cp [source] [destination]` : Copie des fichiers ou des répertoires.
    - `-r` : Copie récursivement les répertoires et leurs contenus.
- `mv [source] [destination]` : Déplace ou renomme des fichiers ou des répertoires.

### Gestion des autorisations

- `chmod [permissions] [nom_du_fichier]` : Modifie les autorisations d'un fichier ou d'un répertoire.
    - `-R` : Modifie récursivement les autorisations des répertoires et de leurs contenus.
- `chown [utilisateur:groupe] [nom_du_fichier]` : Modifie le propriétaire et/ou le groupe d'un fichier ou d'un répertoire.
    - `-R` : Modifie récursivement la propriété des répertoires et de leurs contenus.
- `chgrp groupe fichier/répertoire` : Cette commande est utilisée pour changer la propriété de groupe d'un fichier ou d'un répertoire.
    - `-R` : Modifie récursivement la propriété de groupe des répertoires et de leurs contenus.

### Processus et Système

- `ps` : Affiche les processus actifs.
    - `-e` : Affiche des informations sur tous les processus.
    - `-f` : Affiche une liste complète.
    - `-u utilisateur` : Affiche les processus appartenant à un utilisateur spécifique.
    - `aux` : Affiche une liste détaillée de tous les processus.
- `kill [PID]` : Tue un processus en utilisant son identifiant de processus (PID).
    - `9` : Termine de force le processus.
- `top` : Affiche les processus en cours d'exécution et leurs ressources.
    - `q` : Quitte top.
    - `k` : Tue un processus.
    - `u` : Spécifie l'utilisateur.
    - `H` : Basculer l'affichage des threads.
    - `P` : Trier par utilisation CPU.
    - `M` : Trier par utilisation mémoire.
    - `R` : Inverser l'ordre de tri.
- `pgrep motif` : Cette commande est utilisée pour rechercher des processus par nom et autres attributs.
    - `-l` : Affiche les noms des processus ainsi que leurs PID.

### Archives et Compression

- `tar -cvf [nom_archive.tar] [fichiers]` : Crée une archive tar.
    - `-c` : Crée une nouvelle archive.
    - `-v` : Mode verbeux, montre les fichiers archivés.
    - `-f [nom_archive.tar]` : Spécifie le nom de l'archive.
- `tar -xvf [nom_archive.tar]` : Extrait une archive tar.
    - `-x` : Extrait les fichiers d'une archive.
    - `-v` : Mode verbeux, montre les fichiers extraits.
    - `-f [nom_archive.tar]` : Spécifie le nom de l'archive.
- `gzip [nom_du_fichier]` : Compresse un fichier en utilisant gzip.
- `gunzip [nom_du_fichier.gz]` : Décompresse un fichier gzip.

### Réseau

- `ping [adresse_ip_ou_nom_de_domaine]` : Vérifie la connectivité réseau.
- `ifconfig` : Affiche des informations sur les interfaces réseau.
- `ssh [utilisateur@adresse_ip]` : Se connecte à une machine distante via SSH.
    - `-p` : Ajoute un port à l'adresse.
	- `-l` : Nom d'utilisateur de connexion.

### Help and Documentation

- `man [command]` Displays the manual for a specific command.
    - `--help` Add this to a command to display quick help.
