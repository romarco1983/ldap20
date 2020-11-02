@edt ASIX M06: LDAP server
--------------------------
Repositori que conté els fitxers per a crear un ldap server amb un container docker mitjançant la imatge ldap20:schema

Podem descarregar-la al repositori de github https://hub.docker.com/repository/docker/isx43457566/ldap20

Definim atributs i objectClass a l'schema futbolistes.schema

La imatge pot funcionar en mode detach i interactiu. S'executa amb la següent comanda:

      detach:     docker run --rm --name ldap.edt.org -h ldap.edt.org --net 2hisix -p 389:389 -d isx43457566/ldap20:schema
      interactiu: docker run --rm --name ldap.edt.org -h ldap.edt.org --net 2hisix -p 389:389 -it isx43457566/ldap20:schema /bin/bash

