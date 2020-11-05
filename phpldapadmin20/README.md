@edt ASIX M06: LDAP server
--------------------------
Repositori que conté els fitxers per a crear un ldap server amb un container docker mitjançant la imatge phpldapamin:20

Servidor phpldapadmin que es connecta al servidor ldap.edt.org. 

Podem descarregar-la al repositori de github https://hub.docker.com/repository/docker/isx43457566/phpldapadmin:20

La imatge pot funcionar en mode detach i interactiu. S'executa amb la següent comanda:

    detach:     docker run --rm --name phpldapadmin.edt.org -h phpldapadmin.edt.org --net 2hisix -p 80:80 -d isx43457566/phpldapadmin:20
    interactiu: docker run --rm --name phpldapadmin.edt.org -h phpldapadmin.edt.org --net 2hisix -p 80:80 -it isx43457566/phpldapadmin:20 /bin/bash


 
    
