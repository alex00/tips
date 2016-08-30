NGINX
==

Configurer Nginx
-

    sudo nano /etc/nginx/sites-available/default

Configuration basique
-

    server {

    listen 80;

    # Pointer le dossier public de votre app
    root RAILS/public;
    passenger_enabled on;

    server_name localhost votredomaine.com;
    }

Redémarrer Nginx
-

    sudo service nginx restart
    
Lien symbolique site available - site enab
-

    sudo ln -s /etc/nginx/sites-available/example.com /etc/nginx/sites-enabled/example.com
