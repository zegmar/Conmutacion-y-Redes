vlan [id]

Crear una VLAN para separar la red en segmentos lógicos.

name [nombre]

Dar un nombre descriptivo a la VLAN.

interface range [puertos]

Seleccionar varios puertos y configurarlos al mismo tiempo.

switchport mode access

Definir el puerto como de acceso, para dispositivos finales (PC, impresora).

switchport access vlan [id]

Meter el puerto de acceso a una VLAN.

switchport mode trunk

Convertir el puerto en troncal para que pasen varias VLANs entre switches (o hacia el router).

switchport trunk native vlan [id]

Cambiar la VLAN nativa del troncal (la que viaja sin etiqueta).

switchport trunk allowed vlan [lista]

Filtrar qué VLANs pueden cruzar el troncal.

switchport port-security

Activar la seguridad de puerto, que controla qué MACs se conectan.

switchport port-security mac-address sticky

Aprender automáticamente las MAC que se conecten y guardarlas.

switchport port-security maximum [num]

Limitar cuántas MAC se permiten en el puerto.

switchport port-security violation shutdown

Apagar el puerto si se conecta un equipo no autorizado.

show vlan brief

Verificar qué VLANs existen y qué puertos tiene cada una.

show interfaces trunk

Verificar los enlaces troncales activos y sus VLANs permitidas.