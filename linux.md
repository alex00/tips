LINUX
==

Rechercher un fichier à partir du contenu
--

    grep -rn "contenu_a_chercher" /var/www/

r: Recursif
n: Donne le numero de ligne


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
