# RedMeshInteligent

# Criterios de asignación para direcciones IPv4 en función de los usos

# Capa pública
Son aquellas que eventualmente tiene sentido que se publiquen más allá de la propia zona o comunidad sin utilizar ningún tipo de NAT. Corresponden por tanto a usuarios, servidores, aplicaciones o lo que sea que tenga sentido que disponga de una dirección única de nivel 3 alcanzando el número máximo de redes abiertas.
Para estos usos se prevé el uso del rango de direcciones 10.0.0.0 - 10.255.255.255

# Capa de gestioń
Son aquellas direcciones que una red necesita para funcionar, pero que no se quiere que traspasen diferentes redes o comunidades. Por ejemplo, las que se utilizan para dispositivos internos, encaminadores (routers), enlaces, funcionamiento interno de protocolos (BATMAN, OLSR...). Estas direcciones se pueden reutilizar entre áreas o zonas diferentes que se gestionen de forma separada. En aquellos puntos donde se conecten se tienen que hacer los filtros oportunos que impidan que este tipo de direcciones se propaguen a las tablas de rutas que publica cada red.
Para estos usos se prevé el uso del rango de direcciones 172.16.0.0 - 172.31.255.255.

# Capa privada
Son las que corresponden a las redes locales privadas que pueden estar conectadas, normalmente trás una NAT, a las redes abiertas. El uso típico es la red privada que hay tras un cortafuegos.
Para este uso se prevé el uso del rango de direcciones 192.168.0.0 - 192.168.255.255.
