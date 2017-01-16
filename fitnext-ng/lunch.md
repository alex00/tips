Lancer Fitnext-ng
-

Start mysql

```
mysql.server start
```

Lunch nginx_local

```
sudo nginx -c /usr/local/etc/nginx/nginx.conf 
sudo nginx -c /usr/local/etc/nginx/nginx.conf -s stop
``` 

Start php with fpm

```
sudo /usr/local/opt/php70/sbin/php70-fpm start
```

Display commands

```
./bin/console
```

Reset BDD

```
./bin/reset-database.sh 
```

Create user

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
