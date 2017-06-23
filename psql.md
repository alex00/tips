Postgres
==

Erreur "roles does not exist"
-

`sudo -u postgres -i`

Se connecter à psql avec un utilisateur
-

`psql -U postgres -h localhost -W`

Commande psql
-

* Quitter

`\q`

* Afficher les tables

`\dt`

* Afficher les utilisateurs

`\du`

Bug

current transaction is aborted commands ignored until end of transaction block

-> Update schema.rb
