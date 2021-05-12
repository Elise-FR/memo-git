# memo-git
différence entre Git et GitHub : 
Git = programme ligne de commande. On est sur un repo local. On créé nos commit
Github = site Github : un des principaux fournisseur de repo Git distant. Sur ce site on peut aussi avoir divers renseignements avec l'onglet explore.

Commit = comme une enveloppe où l'on peut mettre en autant de fichiers que l'on veut. 
Git Commit = comme cacheter l'enveloppe 
Git add = ajouter le contenu dans l'enveloppe 
push = envoyer sur le repo distant 

Fork = Sorte de photocopie. On récupère le code source sur notre profil. Il est duppliqué.

Taguer une version = la nommer

repository = fichier + ensemble de l'historique des changements 

Aide 1:
Créer un nouveau dossier sur la ligne de commande GIT :
Mkdir <nom du dossier> (attention les <> sont uniquement là pour dire qu'il faut remplacer par notre nom de dossier, il n'y a pas besoin de les mettre dans notre ligne de commande)

Naviguer dans un dossier existant : 
cd <nom dus dossier>

Lister les éléments dans dossier : 
ls

Activer git pour un répertoire : 
Git init

Aide 2:

Vérifier l'état des modifs dans un dépot:
Git status

Afficher les modifs apportées aux fichiers:
Git diff

Ajouter les modifs d'un fichier à soumettre : 
Git add <nom de mon fichier>

Pour ajouter toutes les modifs d'un seul coup : 
Git add . (Attention, si on a plusieurs fichier dans un répertoire, il prend en compte tous les fichiers, mieux vaut nommer chaque fichier)

Pour soumettre les modifs qu'on a ajoutées avec un message décrivant les modifs : 
git commit -m "mon message"

Aide 3:

Ajoutez nom utilisateur github à la configuration git :
git config --global user.username <UserName>

Vérifier ce qui a été configuré dans git :: 
git config --global user.username

Important : 

Lorsque l'on veut que notre répertoire soit reconnu par Git : 
git init (que l'on fait une seule fois)

Lorsque l'on modifie un ficher : 
git add <nom du fichier> (à refaire à chaque modifs)

On fait ensuite un commit message : 
git commit -m "mon message" (à faire à chaque fois que l'on veut marquer un commit)

Pour pouvoir envoyer nos fichiers sur github : 
git remote add origin git@github.com:....git
git push -u origin master 

(git push à faire au minimum 1x par jour)

Pour pousser un tag : 
git push origin <nom du tag>

Pour pousser plusieurs tags : 
Git push --tags

Pour revenir à commit précis : 
Git checkout <numero commit> 

Pour revenir au master après le HEAD: 
Git switch - 

Pour afficher tous ses commits : 
git log

