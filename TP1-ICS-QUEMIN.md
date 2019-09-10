# TP1 Admin Systeme Remi Quemin

<br>
<br>


## Manuel

<br>
<br>


#### 1. A l’aide du manuel, identifiez le rôle de la commande which
Which renvoie le chemin des fichiers qui sont executables. 
Par exemple quand on fait "which ls" il va donner le chemin ou le fichier est executable.
<br/>
#### 2. Quand on consulte cette page, comment peut-on rechercher, par exemple, le mot option? 
Une fois avoir fait man which , nous cherchons un mot, 
par exemple le mot "option" pour cela il faut taper "/" et rentrer le mot que l'on souhaite ainsi quand on rentre `"/option"`, 
il surligne les mots options présents.
<br/>
#### 3. Comment quitte-t-on le manuel? 
Pour quitter le manuel, il suffit d'appuyer sur la touche "q"
<br/>
#### 4. Chaque section du manuel a une première page, qui présent
Pour afficher la premiere page de la section 6, j'ai fais `"man 6 intro"`, 
cette section affiche tout ce qui est en rapport avec les jeux, gadgets, economiseur d'ecran.
<br/>
<br/>
## Navigation dans l’arborescence des fichiers
<br/>

#### 1. Allez dans le dossier /var/log 
Pour aller dans /var/log, je fais `cd /var/log`.
<br/>
#### 2. Remontez dans le dossier parent (/var) en utilisant un chemin relatif 
Pour retourner dans le dossier parent (donc /var) il suffit de taper `"cd .."` ainsi nous sommes passés du dossier /log au dossier /var.
<br/>
#### 3. Retournez dans le dossier personnel 
Pour retourner dans le dossier personnel il suffit de rentrer `"cd"`.
<br/>
#### 4. Revenez au dossier précédent (/var)
Pour retourner dans le dossier precedent il suffit de faire `cd -`.
<br/>
#### 5. Essayez d’accéder au dossier /root; que se passe-t-il?
Quand on essaye d'acceder au dossier root, l'accès est refusé.
<br/>
#### 6. Essayez la commande sudo cd /root; que se passe-t-il? Expliquez 
On ne peut pas utliser à la fois la commande sudo et la commande cd.
<br/>
#### 7. A partir de votre dossier personnel, créez l’arborescence suivante :
Maintenant je dois créer une arborescence en créant des fichiers ainsi que des dossiers : Pour cela : `mkdir` pour créer un dossier suivi du nom du dossier. Exemple : `mkdir Dossier1 Dossier 2` <br/>
Pour créer un fichier : `touch fichier1 fichier 2`.
<br/>
#### 8. Revenez dans votre dossier personnel ; à l’aide de la commande rm, essayez de supprimer Fichier1, puis Dossier1 ; que se passe-t-il ?
Pour revenir au dossier personnel il suffit de faire: `cd`
Pour supprimer le Fichier1 : `rm Dossier1/Fichier1`
la commande `rm Dossier1` renvoie une erreur :
_cannot remove Dossier1: Is a directory_
Il faut modifier la commande `rm` afin de supprimer un dossier.
<br/>
#### 9. Quelle commande permet de supprimer un dossier ?
La commande qui permet de supprimer un dossier est : `rmdir`.
<br/>
#### 10. Que se passe-t-il quand on applique cette commande à Dossier2 ?
Quand on essaye de supprimer le Dossier2 : `rmdir Dossier2` , <br/> 
> rmdir: failed to remove 'Dossier2': Directory not empty <br/>
Il ne peut pas supprimer le dossier le dossier n'est pas vide, en effet il y a plusieurs fichiers.
<br/>
#### 11. Comment supprimer en une seule commande Dossier2 et son contenu ?
Pour supprimer le Dossier2 et son contenu il suffit de faire : `rm -r Dossier2`.
<br/>
<br/>

## Commandes importantes
<br/>

#### 1. Quelle commande permet d’afficher l’heure ? A quoi sert la commande time ?
la commande qui permet d'afficher l'heure est la commande : `date`
la commande time sert à determiner le temps d'execution d'une commande choisie.
Par exemple time ls -l : <br/>
>real   0m0, 002s <br/>
>user   0m0, 002s  <br/>
>sys    0m0, 002s  <br/>
<br/>

#### 2. Dans votre dossier personnel, tapez successivement les commandes ls puis la ; que peut-on en déduire sur les fichiers commençant par un point ?
Quand on fait ls rien n'apparait tandis qu'avec la commande la des fichiers commçant par un point apparaissent, ce sont des fichiers cachés.

#### 3. Où se situe le programme ls ?
Grace a la commande which ls on sait que le programme se situe : `/usr/bin/ls`.

#### 4. Que fait la commande ll ? (indice : la commande alias peut vous aider)
La commande ll affiche des informations des fichiers et/ou des dossiers nous avons par exemple les droits, le poids, la date.

#### 5. Quelle commande permet d’afficher les fichiers contenus dans le dossier /bin ?
la commande `ls /bin`.

#### 6. Que fait la commande ls .. ?
La commande `ls ..` permet de lister le dossier père dans l'arborescence.

#### 7. Quelle commande donne le chemin complet du dossier courant ?
La commande qui permet de donner le chemin complet du dossier courant est : `pwd`. Dans mon cas elle m'affiche :  <br/>
> home/serveur <br/>

#### 8. Que fait la commande echo 'yo' > plop exécutée 2 fois ?
Cette commande permet de créer un fichier plop avec écrit:
> yo <br/>

#### 9. Que fait la commande echo 'yo' >> plop exécutée 2 fois ?
cette commande permet de créer un fichier plop avec écrit:
> yo <br/>
> yo <br/>

#### 10. A quoi sert la commande file ? Essayez la sur des fichiers de types différents.
La commande file retourne le type de données contenue dans une fichier par exemple dans le fichier1 : <br/>
> empty. <br/>
Tandis que le fichier plop : <br/> 
> ASCII text <br/>

#### 11. Créez un fichier toto qui contient la chaîne Hello Toto ! ; créer ensuite un lien titi vers ce fichier avec la commande ln toto titi. Modifiez à présent le contenu de toto et affichez le contenu de titi :qu’observe-t-on ? Supprimez le fichier toto ; quelle conséquence cela a-t-il sur titi ?
Lorque l'on modifie le fichier toto, le fichier titi est modifiée également. Quand on supprime le fichier toto le fichier titi devient un simple fichier unique et garde le contenu de toto.

#### 12. Créez à présent un lien symbolique tutu sur titi avec la commande ln -s titi tutu. Modifiez le contenu de titi ; quelle conséquence pour tutu ? Et inversement ? Supprimez le fichier titi ; quelle conséquence cela a-t-il sur tutu ?
Quand on modifie le contenu de titi le contenu de tutu est modifié aussi. Et inversement. Cependant quand on supprime le fichier titi et que l'on souhaite voir le contenu du fichier tutu : `No such file or directory`. Le fichier est donc corompu, on remarque quand on fait ls, le fichier tutu est rouge.

#### 13. Affichez à l’écran le fichier /var/log/syslog. Quels raccourcis clavier permettent d’interrompre et reprendre le défilement à l’écran ?
En faisant `cat /var/log/syslog` nous affichons le fichier. Pour arreter le defilement et pouvoir voir les lignes une par une il est possible grace à la commande : `cat /var/log/syslog | less`.

#### 14. Affichez les 5 premières lignes du fichier /var/log/syslog, puis les 15 dernières, puis seulement les lignes 10 à 20.
La commande `head -5 /var/log/syslog` permet de voir les 5 première lignes du fichier la commande `tail -15 /var/log/syslog` permet de voir les 15 dernières lignes et la commande `head -n 10 20 /var/log/syslog` permet de voir entre les lignes 10 et 20.

#### 15. Que fait la commande dmesg | less ?
La commande dmesg  permet de voir l'historique des messages du noyaux. la commande lee permet comme dit precedemment d'interrompre le defilement afin de pouvoir naviguer librement dnas le fichier.

#### 16. Affichez à l’écran le fichier /etc/passwd ; que contient-il ? Quelle commande permet d’afficher la page de manuel de ce fichier ?
Pour afficher le fichier : `cat /etc/passwd/`, il contient différentes informations sur les utilisateurs systèmes.
La commande qui permet d'afficher la page de manuel est : `man 5 passwd`.

#### 17. Affichez seulement la première colonne triée par ordre alphabétique inverse

#### 18. Quelle commande nous donne le nombre d’utilisateurs ?
La commande qui nous donne le nombre d'utilisateur est : `who`.

#### 19. Combien de pages de manuel comportent le mot-clé conversion dans leur description ?
Avec la commande `man -k conversion` , je constate qu'il y a 4 pages.

#### 20. A l’aide de la commande find, recherchez tous les fichiers se nommant passwd présents sur la machine.
La commande find : `find / -name 'passwd'`.

#### 21. Modifiez la commande précédente pour que la liste des fichiers trouvés soit enregistrée dans le fichier ~/list_passwd_files.txt et que les erreurs soient redirigées vers le fichier spécial /dev/null.

#### 22. Dans votre dossier personnel, utilisez la commande grep pour chercher où est défini l’alias ll vu précédemment.

#### 23. Utilisez la commande locate pour trouver le fichier history.log.
En rentrant la commande `locate history.log`, on constate que le fichier situe dans /var/log/apt.

#### 24. Créer un fichier dans votre dossier personnel puis utilisez locate pour le trouver. Apparaît-il ? Pourquoi ?
La commande locate utilise une base de données. Ce fichier vient d'etre crée il y a peu de temps, il faudra attendre 24h pour que la base se mette a jour pour que l'on puisse locate notre fichier.










