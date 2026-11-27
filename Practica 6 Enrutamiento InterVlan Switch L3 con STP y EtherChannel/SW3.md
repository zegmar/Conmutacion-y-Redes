#ConfiguracionPractica4

Se aplicaron las [[Configuración Básica | Configuraciones Básicas]]

Se Realizo la [[VLAN || Configuración de Vlan's ]] y de [[Enlace Troncal || Enlaces Troncales]]

Se asigno  vlan 30 como root prymary para [[Spanning Tree Protocol || STP]]

Se configuraron los [[EtherChannel || ChannelGroup]]


Datos Utilizados: 
- **Hostname:** SW3
- **Nombre del dominio:** redes.local
- **bits en la key:** 4096
- **Mensaje:** Solo Personal Autorizado!!!
- **Usuario:** admin **Contraseña:** cisco
- **Contraseña:** cisco
- **Puertos apagados:** f0/2-5,f0/7-10,f0/12-20, f0/21, f0/24
- **Puertos Troncales:** f0/21-24
- ***EtherChannel:*** 
	- ***ChannelGroup:*** 1
		- ***Puertos:*** f0/23,f0/24
	- ***ChannelGroup:*** 2
		- ***Puertos:*** f0/21,f0/22
- **Vlans:**
	- **Vlan:** 10
		- **IP:** 192.168.10.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Estudiantes
		- **Puertos:** f0/1-5
	- **Vlan:** 20
		- **IP:** 192.168.20.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Profesores
		- **Puertos:** f0/6-10
	- **Vlan:** 30
		- **IP:** 192.168.30.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Invitados
		- **Puertos:** f0/11-15
	- **Vlan:** 99
		- **IP:** 192.168.99.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Admin&Nativa
		- **Puertos:** f0/21-24
	- **Vlan:** 100
		- **Nombre:** SinUso
		- **Puertos:** f0/16-20