#ConfiguracionPractica2

Se aplicaron las [[Configuración Básica | Configuraciones Basicas]]

Se Realizo la [[VLAN y Seguridad de puertos|| Configuración de Vlan's ]] y de [[Enlace Troncal || Enlaces Troncales]]

Datos Utilizados: 
- **Hostname:** SW3
- **Nombre del dominio:** redes.local
- **bits en la key:** 4096
- **Mensaje:** Solo Personal Autorizado!!!
- **Usuario:** admin **Contraseña:** cisco
- **Contraseña:** cisco
- **Puertos apagados:** f0/2-5,f0/7-10,f0/12-20, f0/21, f0/24
- **Puertos Troncales:** f0/21-24
- **Vlans:**
	- **Vlan:** 1
		- **IP:** 192.168.1.250
		- **Mascara:** 255.255.255.0
	- **Vlan:** 10
		- **Nombre:** Estudiantes			
		- **Puertos:** f0/1-5
	- **Vlan:** 20
		- **Nombre:** Profesores
		- **Puertos:** f0/6-10
	- **Vlan:** 30
		- **Nombre:** Invitados
		- **Puertos:** f0/11-15
	- **Vlan:** 99
		- **Nombre:** Admin&Nativa
		- **Puertos:** f0/21-24
	- **Vlan:** 100
		- **Nombre:** SinUso
		- **Puertos:** f0/16-20
