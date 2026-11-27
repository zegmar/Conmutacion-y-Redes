no ip domain-lookup

Evitar que el router intente resolver por DNS un comando mal escrito.

line vty 0 4

Entrar a las 5 sesiones remotas del router.

exec-timeout 5 30

Cerrar la sesión tras 5 minutos y 30 segundos sin actividad.

interface gigabitethernet [0/0]

Entrar a la interfaz de red local (LAN) del router.

interface serial [0/0/0]

Entrar a la interfaz serial, el enlace WAN entre routers.

description [texto]

Documentar hacia dónde va el cable de esa interfaz.

clock rate [valor]

Dar la sincronización en el extremo DCE del cable serial.

show ip interface brief

Verificar que las interfaces tengan IP y estén up/up.

show ip route

Ver la tabla de enrutamiento: conectadas (C), locales (L) y aprendidas.