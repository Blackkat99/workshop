# workshop
man
Équivalent Windows : help
Signification : manual
Affiche les pages du manuel système.
Chaque argument donné à man est généralement le nom d'un programme, d'un utilitaire, d'une fonction ou d'un fichier spécial.
Exemples d'utilisation :
man man
affiche les informations pour l'utilisation de man
man exports
décrit le contenu et la syntaxe du fichier /etc/exports pour les partages NFS
'q' pour quitter.
Voir aussi la page man
ls
Équivalent Windows : dir
Signification : list
Permet de lister un répertoire
Options les plus fréquentes :
-l : Permet un affichage détaillé du répertoire (permissions d'accès, le nombre de liens physiques, le nom du propriétaire et du groupe, la taille en octets, et l'horodatage)
-h : Associé avec -l affiche la taille des fichiers avec un suffixe correspondant à l'unité (K, M, G)
-a : Permet l'affichage des fichiers et répertoires cachés (ceux qui commencent par un . (point))
-lct : Permet de trier les fichiers et répertoires par date de modification décroissante
Exemples d'utilisation :
ls -a
affiche tous les fichiers et répertoires y compris les cachés du répertoire courant
ls /etc/
affiche le contenu du répertoire /etc/
lspci ou lsusb
affiche les périphériques PCI ou USB connectés.
lshw affiche les caractéristiques de tout le matériel physique, non-logiciel (hardware).
Voir aussi ls en couleur
Remarque :
Il existe également une commande dir quasi identique à la commande ls. Elle s'utilise de la même façon, avec les mêmes options, et les pages man (manuel) les 2 commandes sont d'ailleurs identiques. Seul l'affichage par défaut de la sortie est différent avec dir :

par défaut la sortie n'est pas en couleur (il faut utiliser l'option --color pour obtenir une sortie en couleur avec dir) ;
les caractères spéciaux tels que les espaces dans les noms des fichiers et dossiers sont précédés d'un caractère \ (backslash).
La commande « ls -C -b » produira une sortie identique à la commande dir employée sans options.

cd
Équivalent Windows : cd
Signification : change directory
Permet de se promener dans les répertoires
Exemples d'utilisation :
cd
permet de revenir au répertoire /home/utilisateur (identique à cd ~)
cd -
permet de revenir au répertoire précédent
cd ..
permet de remonter au répertoire parent (ne pas oublier l'espace contrairement à windows)
cd /
permet de remonter à la racine de l'ensemble du système de fichiers
cd /usr/bin/ ou usr/bin
se place dans le répertoire /usr/bin/
mv
Équivalent Windows : move / ren
Signification : move
Permet de déplacer ou renommer des fichiers et des répertoires
Options les plus fréquentes :
-f : Écrase les fichiers de destination sans confirmation
-i : Demande confirmation avant d'écraser
-u : N'écrase pas le fichier de destination si celui-ci est plus récent
Exemples d'utilisation :
mv monFichier unRep/
Déplace monFichier dans le répertoire unRep
mv unRep/monFichier .
Déplace le fichier monFichier du répertoire unRep là où on se trouve
mv unRep monRep
Renomme unRep en monRep
cp
Équivalent Windows : copy / xcopy
Signification : copy
Permet de copier des fichiers ou des répertoires
Options les plus fréquentes :
-a : Archive. Copie en gardant les droits, dates, propriétaires, groupes, etc.
-i : Demande une confirmation avant d'écraser
-f : Si le fichier de destination existe et ne peut être ouvert alors le détruire et essayer à nouveau
-R ou -r : Copie un répertoire et tout son contenu, y compris les éventuels sous-répertoires
-u : Ne copie que les fichiers plus récents ou qui n'existent pas
-v : permet de suivre les copies réalisées en temps réel
Exemples d'utilisation :
cp monFichier sousrep/
Copie monFichier dans sousrep
cp -r monRep/ ailleurs/
Copie le répertoire monRep (et ses éventuels sous-répertoires) vers ailleurs en créant le répertoire ailleurs/monRep s'il n'existe pas.
cp monRep/{*.cpp,*.h,MakeFile,Session.vim} ailleurs/
Copie les fichiers spécifiés dans {} contenus dans le répertoire monRep vers ailleurs. Notez bien qu'il n'y a pas d'espace entre ces noms de fichiers.
