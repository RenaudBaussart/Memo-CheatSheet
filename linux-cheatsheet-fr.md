Navigation dans le système de fichiers :

    ls : Liste les fichiers et répertoires dans le répertoire actuel.
    cd [nom_du_répertoire] : Change le répertoire de travail.
    pwd : Affiche le chemin du répertoire actuel.
    mkdir [nom_du_répertoire] : Crée un nouveau répertoire.
    rm [nom_du_fichier] : Supprime un fichier.
        -rf : suprime tout les fichier/dossier enfant de celuit indiquée
    rmdir [nom_du_répertoire] : Supprime un répertoire vide.
    cp [source] [destination] : Copie des fichiers ou des répertoires.
    mv [source] [destination] : Déplace ou renomme des fichiers ou des répertoires.
    cat [nom_du_fichier] : Affiche le contenu d'un fichier.

Manipulation de fichiers :

    touch [nom_du_fichier] : Crée un nouveau fichier vide.
    nano [nom_du_fichier] : Ouvre le fichier dans l'éditeur de texte Nano.
Gestion des permissions :

    chmod [permissions] [nom_du_fichier] : Change les permissions d'un fichier ou d'un répertoire.
    chown [utilisateur:groupe] [nom_du_fichier] : Change le propriétaire et/ou le groupe d'un fichier ou d'un répertoire.

Processus et système :

    ps : Affiche les processus actifs.
    kill [PID] : Tue un processus en utilisant son identifiant de processus (PID).
    top : Affiche les processus en cours d'exécution et leurs ressources.

Archives et compression :

    tar -cvf [nom_archive.tar] [fichiers] : Crée une archive tar.
    tar -xvf [nom_archive.tar] : Extrait une archive tar.
    gzip [nom_fichier] : Compresse un fichier avec gzip.
    gunzip [nom_fichier.gz] : Décompresse un fichier gzip.

Réseau :

    ping [adresse_ip_ou_nom_de_domaine] : Vérifie la connectivité réseau.
    ifconfig : Affiche les informations sur les interfaces réseau.
    ssh [utilisateur@adresse_ip] : Se connecte à une machine distante via SSH.
        -p : indique le port
	    -l : indique le nom de login
    scp [fichier] [utilisateur@adresse_ip:destination] : Copie des fichiers via SSH.

Aide et documentation :

    man [commande] : Affiche le manuel pour une commande spécifique.
    --help : Ajoutez ceci à une commande pour afficher une aide rapide.