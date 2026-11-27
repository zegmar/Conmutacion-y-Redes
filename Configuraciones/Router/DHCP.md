ip dhcp excluded-address [inicio] [fin]

Reservar IPs que DHCP no debe repartir (gateways, servidores).

ip dhcp pool [nombre]

Crear un ámbito (pool) de direcciones DHCP.

network [red] [máscara]

Dentro del pool, definir la red de la que se reparten IPs (con máscara normal).

default-router [IP_gateway]

Decir a los clientes DHCP cuál es su puerta de enlace.

dns-server [IP_dns]

Decir a los clientes DHCP cuál es su servidor DNS.

ip helper-address [IP_servidor_dhcp]

Reenviar las solicitudes DHCP hacia un servidor que está en otra subred.

show ip dhcp binding

Ver qué IP se asignó a cada MAC.