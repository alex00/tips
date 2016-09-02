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
