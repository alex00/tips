Delayed Job
==

Executer une tâche spécifique
-

### Sans la supprimer #

    Delayed::Job.find(x).invoke_job

### Et la supprimer #

    Delayed::Worker.new.run(Delayed::Job.last)
