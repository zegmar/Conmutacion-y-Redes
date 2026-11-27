ip route [red] [máscara] [siguiente_salto]

Crear una ruta estática manual hacia una red remota.

ip route 0.0.0.0 0.0.0.0 [siguiente_salto]

Ruta por defecto: gateway de último recurso para todo lo desconocido.

ip route [red] [máscara] [salto] [distancia]

Ruta estática flotante: respaldo que solo entra si falla la principal.