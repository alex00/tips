Delayed Job
==

Executer une tâche spécifique
-

### Sans la supprimer #

    Delayed::Job.find(x).invoke_job

### Et la supprimer #

    Delayed::Worker.new.run(Delayed::Job.last)

### Lancer delayed job (Rails 4) #

    bundle exec bin/delayed_job start
    
### Stoper delayed job (Rails 4) #

    bundle exec bin/delayed_job stop

### Créer un fichier de log

Ajouter le fichier config/initializers/delayed_job.rb

    Delayed::Worker.logger = Logger.new(File.join(Rails.root, 'log', 'dj.log'))
