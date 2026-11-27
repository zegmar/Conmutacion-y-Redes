#ConfiguracionPractica4

Se aplicaron las [[Configuración Básica | Configuraciones Basicas]]

Se Realizo la [[VLAN y Seguridad de puertos|| Configuración de Vlan's ]] y de [[Enlace Troncal || Enlaces Troncales]]

Datos Utilizados: 
- **Hostname:** SW2
- **Nombre del dominio:** redes.local
- **bits en la key:** 4096
- **Mensaje:** Solo Personal Autorizado!!!
- **Usuario:** admin **Contraseña:** cisco
- **Puertos apagados:** f0/2-5,f0/7-10,f0/12-20, f0/21, f0/23
- **Puertos Troncales:** f0/21-24
- **Vlans:**
	- **Vlan:** 10
		- **IP:** 192.168.10.2
		- **Mascara:** 255.255.255.0
		- **Nombre:** Estudiantes
		- **Puertos:** f0/1-5
	- **Vlan:** 20
		- **IP:** 192.168.20.2
		- **Mascara:** 255.255.255.0
		- **Nombre:** Profesores
		- **Puertos:** f0/6-10
	- **Vlan:** 30
		- **IP:** 192.168.30.2
		- **Mascara:** 255.255.255.0
		- **Nombre:** Invitados
		- **Puertos:** f0/11-15
	- **Vlan:** 99
		- **IP:** 192.168.99.2
		- **Mascara:** 255.255.255.0
		- **Nombre:** Admin&Nativa
		- **Puertos:** f0/21-24
	- **Vlan:** 100
		- **Nombre:** SinUso
		- **Puertos:** f0/16-20