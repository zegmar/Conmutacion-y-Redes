access-list [1-99] [permit|deny] [origen] [wildcard]

ACL estándar numerada: filtra solo por IP de origen.

ip access-list extended [NOMBRE]

Crear una ACL extendida con nombre (filtra origen, destino, protocolo y puerto).

[permit|deny] [protocolo] [origen] [wc] [destino] [wc] eq [puerto]

Regla detallada de ACL extendida (eq 80 es HTTP, eq 22 es SSH).

permit ip any any

Permitir el resto del tráfico. Sin esto, el deny implícito final bloquea todo.

ip access-group [nombre_o_num] [in|out]

Aplicar la ACL en una interfaz, de entrada (in) o de salida (out).