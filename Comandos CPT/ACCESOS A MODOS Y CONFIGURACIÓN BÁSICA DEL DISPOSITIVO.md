- Enable: Se entra al modo privilegiado.

- Configure terminal: Se entra al modo de configuración global.

- line console 0: Se entra al modo de configuración del puerto físico.

- hostname name: Cambiar el nombre del switch. (Solo en configuración global).

- banner motd # mensaje#: Coloca un warning en determinada parte del switch.

- Logging synchronous: Evita que los warning aparezcan al teclear comandos.

- interface range f0/2-20: Configuración de iface para el rango de puertos elegidos.

- shutdown: Apagar los puertos.

- no shutdown: Enciende la interfaz de red del switch.

- copy running-config startup-config: Guarda los cambios de configuración del switch.
