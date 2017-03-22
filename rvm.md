Problème de certificat ssl


Afficher la liste (update)
-

    ruby -ropenssl -e 'p OpenSSL::X509::DEFAULT_CERT_FILE'
 

that outputs 
-

    "/usr/local/etc/openssl/cert.pem"

Et

-

    mv /usr/local/etc/openssl/cert.pem /usr/local/etc/openssl/cert.pem.old
