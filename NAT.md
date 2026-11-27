ip nat inside

Marcar la interfaz como interna (lado de la red privada).

ip nat outside

Marcar la interfaz como externa (salida a Internet).

access-list [número] permit [red] [wildcard]

Identificar qué redes internas tendrán salida por NAT.

ip nat inside source list [acl] interface [wan] overload

PAT: traducir muchas IP privadas con una sola IP pública.

ip nat inside source static [privada] [pública]

NAT estático 1 a 1, por ejemplo para publicar un servidor.

show ip nat translations

Ver la tabla activa de traducciones NAT.