@edt ASIX M06: LDAP server
--------------------------
Repositori que conté els fitxers per a crear un ldap server amb un container docker mitjançant la imatge ldap20:entrypoint

Imatge amb varies opcions d'arrencada segons l'argument que passem: start, initdb, initdbedt.


   - initdbedt: crea tota la base de dades edt (esborra tot el que hi havia prèviament). Hi posa la xixa.
   - initdb: esborra tot el que hi havia i crea la base de dades sense xixa.
   - start: engega el servidor


Podem descarregar-la al repositori de github https://hub.docker.com/repository/docker/isx43457566/ldap20

La imatge pot funcionar en mode detach i interactiu. S'executa amb la següent comanda:

      detach:     docker run --rm --name ldap.edt.org -h ldap.edt.org --net 2hisix -p 389:389 -v ldap-config:/etc/openldap/slapd.d -v ldap-data:/var/lib/ldap isx43457566/ldap20:entrypoint initdbedt

