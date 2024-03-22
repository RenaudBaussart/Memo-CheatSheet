git commande	
	
	git init [dossier local] (permet de crée un repositori avec un dossier local)
	  git init (dans un dossier directement)
	  
	git clone[url] (clone dans le dossier actuelle un repo a partir d'un url)
	
	git status (permet de voir les diff entre les fichier local et ceux qui sont dans le staging)

	git add * (ajout un ficher dans le staging area pour pouvoir le commit plus tard)
	
	git commit -m "le message pour expliquer se que tu a fait"(perme d'initialiser les log pour le repo)
	  -git commit -a (commit les fichier dans le staging area)

	git diff (permet de voir la difference entre les fichier local et le repo
	  git diff -staged (permet de voir la difference entre les fichier dans la staging area et le repo)
	  git diff [fist branch] [second branche] (permet de voir la les diff entre les 2 banche mantioné)
	
	git reset [fichier] (permet de retiré un ficher dans le staging area sans suprimé les modif)
	  git reset [commits] (reset tout les commits apres celui mentionée mais les garde localement)
	  git reset -hard [commits] (comme au desus mais sa les suprime)
	
	git status (te montre se qui est dans le staging area)
	
	git rm (permet de suprimer un ficher dans un repo)
	
	git log (te donne les info sur les differente branche actuel)
	  -git log –follow[file] (te donne les log d'un ficher en particulier)
	
	git show [commit] (te montre ton commit)
	
	git branch [nomdebranch] (crée une branche dans ton local)
	
	git checkout [nomdebranch] (se place dans la branch du meme nom)
	
	git remote add [le nom du remote] [url] (crée un remote pour facilité les push vers un repo)
	  git remote -v (te montre la liste de t'est remote)

    git push [origine ou ...] [la branche actuel]
