Rails
==

Tester page erreur 404, 500 en local
-

Remplacer dans config/developement.rb

  `config.consider_all_requests_local = true`
  
  par
  
  `config.consider_all_requests_local = false`

Arreter un process PID
-

    lsof -wni tcp:<port>
    kill -9 <pid>

Lancer rake db:seed sur un fichier
-

    rake db:seed:single SEED=<seed_name_without_.seeds.rb>
    rake db:seed:single SEED=my_custom_seed

Erreur rails console
-

    Library not loaded: /usr/local/opt/readline/lib/libreadline.6.dylib (LoadError)
    
Lancer la commande :

    ln -s /usr/local/opt/readline/lib/libreadline.7.0.dylib /usr/local/opt/readline/lib/libreadline.6.dylib
  
