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


#### 1. allez dans le dossier /var/log 
Pour aller dans /var/log, je fais cd /var/log

#### 2. remontez dans le dossier parent (/var) en utilisant un chemin relatif 
Pour retourner dans le dossier parent (donc /var) il suffit de taper "cd .." ainsi nous sommes passés du dossier /log au dossier /var.

#### 3. retournez dans le dossier personnel 
Pour retourner dans le dossier personnel il suffit de rentrer "cd" pour retourner au dossier personnel.

#### 4. revenez au dossier précédent (/var)
Pour retourner dans le dossier precedent il suffit de faire cd -

#### 5. essayez d’accéder au dossier /root; que se passe-t-il?
Quand on essaye d'acceder au dossier root, l'accès est refusé.

#### 6. essayez la commande sudo cd /root; que se passe-t-il? Expliquez 
On ne peut pas utliser a la fois la commande sudo et la commande cd

#### 7. à partir de votre dossier personnel, créez l’arborescence suivante :
Maintenant je dois créer une arborescence en créant des fichiers ainsi que des dossiers : Pour cela : mkdir pour créer un dossier sui vi du nom du dossier. Exemple : mkdir Dossier1 Dossier 2
Pour créer un fichier : touch fichier1 fichier 2
