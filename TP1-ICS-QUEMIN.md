# tp1-admin-systeme-RemiQuemin
tp1-admin-systeme-RemiQuemin created by GitHub Classroom



### Manuel


#### 1. A l’aide du manuel, identifiez le rôle de la commande which 
Which renvoie le chemin des fichiers qui sont executables. 
Par exemple quand on fait "which ls" il va donner le chemin ou le fichier est executable.

#### 2. Quand on consulte cette page, comment peut-on rechercher, par exemple, le mot option? 
Une fois avoir fait man which, nous cherchons un mot, 
par exemple le mot "option" pour cela il faut taper "/" et rentrer le mot que l'on souhaite ainsi quand on rentre "/option", 
il surligne les mots options présents.
#### 3. Comment quitte-t-on le manuel? 
Pour quitter le manuel, il suffit d'appuyer sur la touche "q"

#### 4. Chaque section du manuel a une première page, qui présent
Pour afficher la premiere page de la section 6, j'ai fais "man 6 intro", 
cette section affiche tout ce qui est en rapport avec les jeux, gadgets, economiseur d'ecran


### Navigation dans l’arborescence des fichiers


#### 1. Allez dans le dossier /var/log 
Pour aller dans /var/log, je fais cd /var/log

#### 2. Remontez dans le dossier parent (/var) en utilisant un chemin relatif 
Pour retourner dans le dossier parent (donc /var) il suffit de taper "cd .." ainsi nous sommes passés du dossier /log au dossier /var.

#### 3. Retournez dans le dossier personnel 
Pour retourner dans le dossier personnel il suffit de rentrer "cd" pour retourner au dossier personnel.

#### 4. Revenez au dossier précédent (/var)
Pour retourner dans le dossier precedent il suffit de faire cd -

#### 5. Essayez d’accéder au dossier /root; que se passe-t-il?
Quand on essaye d'acceder au dossier root, l'accès est refusé.

#### 6. Essayez la commande sudo cd /root; que se passe-t-il? Expliquez 
On ne peut pas utliser a la fois la commande sudo et la commande cd

#### 7. A partir de votre dossier personnel, créez l’arborescence suivante :
Maintenant je dois créer une arborescence en créant des fichiers ainsi que des dossiers : Pour cela : mkdir pour créer un dossier sui vi du nom du dossier. Exemple : mkdir Dossier1 Dossier 2
Pour créer un fichier : touch fichier1 fichier 2

#### 8. Revenez dans votre dossier personnel ; à l’aide de la commande rm, essayez de supprimer Fichier1, puis Dossier1 ; que se passe-t-il ?

Pour revenir au dossier personnel il suffit de faire: `cd`
pour supprimer le Fichier1 : `rm Dossier1/Fichier1`

la commande `rm Dossier1` renvoie une erreur : <br>
_cannot remove Dossier1: Is a directory_

Il faut modifier la commande `rm` afin de supprimer un dossier.

#### 9. Quelle commande permet de supprimer un dossier ?

La commande qui permet de supprimer un dossier est : rmdir

#### 10. Que se passe-t-il quand on applique cette commande à Dossier2 ?

Quand on essaye de supprimer le Dossier2 : rmdir Dossier2 , rmdir: failed to remove 'Dossier2': Directory not empty
Il ne peut pas supprimer le dossier le dossier n'est pas vide, en effet il y a plusieurs fichiers.

#### 11. Comment supprimer en une seule commande Dossier2 et son contenu ?

Pour supprimer le Dossier2 et son contenu il suffit de faire : rm -r Dossier2

### Commandes importantes


#### 1. Quelle commande permet d’afficher l’heure ? A quoi sert la commande time ?

la commande qui permet d'afficher l'heure est la commande : date
la commande time sert à determiner le temps d'execution d'une commande choisie.
Par exemple time ls -l : 
real   0m0, 002s
user   0m0, 002s 
sys    0m0, 002s 












