A CA file has been bootstrapped using certificates from the system
keychain. To add additional certificates, place .pem files in
  /usr/local/etc/openssl@1.1/certs

and run
  /usr/local/opt/openssl@1.1/bin/c_rehash

This formula is keg-only, which means it was not symlinked into /usr/local.

Apple has deprecated use of OpenSSL in favor of its own TLS and crypto libraries

Generally there are no consequences of this for you. If you build your
own software and it requires this formula, you'll need to add to your
build variables:

    LDFLAGS:  -L/usr/local/opt/openssl@1.1/lib
    CPPFLAGS: -I/usr/local/opt/openssl@1.1/include
    PKG_CONFIG_PATH: /usr/local/opt/openssl@1.1/lib/pkgconfig

==> Summary
🍺  /usr/local/Cellar/openssl@1.1/1.1.0c: 6,225 files, 15.3M
==> Installing nginx 
==> Downloading https://homebrew.bintray.com/bottles/nginx-1.10.2_1.yosemite.bottle.1.tar.gz
######################################################################## 100,0%
==> Pouring nginx-1.10.2_1.yosemite.bottle.1.tar.gz
==> Caveats
Docroot is: /usr/local/var/www

The default port has been set in /usr/local/etc/nginx/nginx.conf to 8080 so that
nginx can run without sudo.

nginx will load all files in /usr/local/etc/nginx/servers/.

To have launchd start nginx now and restart at login:
  brew services start nginx
Or, if you don't want/need a background service you can just run:
  nginx
  
  
```bash  
sudo nginx -c /usr/local/etc/nginx/nginx.conf -s stop
sudo nginx -c /usr/local/etc/nginx/nginx.conf
```
