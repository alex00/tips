Lancer Fitnext-ng
-

Afficher les commandes

```
./bin/console
```

Reseter la BDD

```
./bin/reset-database.sh 
```

Créer user

```
./bin/console fitnext:user:create --email=alex@test.fr --password=0000
```

Add user in program

```
 ./bin/console fitnext:engine:userprogram:add 1 1 --start-at=2017-01-06
```

Generate program for a one user

```
./bin/console fitnext:engine:user:plan 1 1 --period=2017-01-06_2017-01-14 -vvv
```

Create an admin

```
./bin/console fitnext:user:role:add --email=alex@test.fr --role=ROLE_ADMIN
```
