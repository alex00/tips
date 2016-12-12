LINUX
==

Rechercher un fichier à partir du contenu
--

    grep -rn "contenu_a_chercher" /var/www/

r: Recursif
n: Donne le numero de ligne

Rechercher un fichier à partir de plusieur strings
--

    grep -e "contenu_1" -e "contenu_2" -e "contenu_3" /var/www/


Rechercher un fichier à partir de son nom
--

    find /var/www -type d -name index.html

type: type de données
name: nom de l'élément recherché


Changer d'utilisateur
--

    sudo -u postgres -i

Changer de mot de passe
--

    passwd

Afficher les connections internet actives
--

    netstat -tupan

Chmod
--

    chmod 740 <file>    
    chmod -R 740 <folder>
    
"4" pour le droit de lecture (read)

"2" pour le droit d'écriture (write )

"1" pour le droit d'exécution (execute)
