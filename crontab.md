crontab
==

    *    *    *    *    *    *
    -    -    -    -    -    -
    |    |    |    |    |    |
    |    |    |    |    |    + year [optional]
    |    |    |    |    +----- day of week (0 - 7) (Sunday=0 or 7)
    |    |    |    +---------- month (1 - 12)
    |    |    +--------------- day of month (1 - 31)
    |    +-------------------- hour (0 - 23)
    +------------------------- min (0 - 59)

Afficher la liste
-

    crontab -l

Afficher la liste (update)
-

    crontab -e`

Supprimer les taches cron
-

    crontab -r`

Gem whenever
==

Mettre à jour crontab
-

    whenever --update-crontab`

