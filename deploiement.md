Déploiement
==

Foward agent (Connection refused - connect(2) for http://exemple.com )
-

    Host exemple.www
    Hostname 000.00.000.000
    ForwardAgent yes
    User <user>


    set :ssh_options, {
      forward_agent: true, 
      user: '<user>',
      proxy: Net::SSH::Proxy::Command.new('ssh exemple.www nc %h %p')
    }

Foward agent (scp: /tmp/exemple/git-ssh.sh: Permission denied)
- 

Ajouter dans deploy.rb
 
    set :tmp_dir, "/home/<user>/tmp"

Commandes capistrano
-

Premier déploiement

    cap <env> deploy:setup
    
Vérifier avant de déployer

    cap <env> deploy:check

Déployer

    cap <env> deploy
    
Revenir à l'ancienne version

    cap <env> deploy:rollback
