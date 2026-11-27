
switchport nonegotiate

Desactivar DTP en el troncal para evitar ataques de salto de VLAN (VLAN hopping).

ip dhcp snooping trust

Marcar el puerto como confiable para que pasen respuestas de servidores DHCP legítimos.

ip dhcp snooping limit rate 6

Limitar DHCP a 6 paquetes por segundo para evitar saturación (DoS).

ip dhcp snooping vlan [lista]

Activar la inspección DHCP en esas VLANs: bloquea servidores DHCP falsos en puertos de acceso.

ip arp inspection validate src-mac dst-mac ip

Validar que las MAC e IP de los paquetes ARP coincidan con la tabla de DHCP snooping.

ip arp inspection vlan [lista]

Activar la Inspección Dinámica de ARP (DAI): bloquea ARP spoofing / Man-in-the-Middle.

spanning-tree portfast default

Activar PortFast de forma global en los puertos de usuario para conexión inmediata.

spanning-tree portfast bpduguard default

Activar BPDU Guard global: bloquea el puerto si alguien conecta un switch no autorizado.

spanning-tree portfast

Forzar PortFast en los puertos seleccionados.

spanning-tree bpduguard enable

Forzar BPDU Guard en los puertos seleccionados.