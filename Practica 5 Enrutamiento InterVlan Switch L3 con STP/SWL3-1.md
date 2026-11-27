#ConfiguracionPractica4 

Se aplicaron las [[Configuración Básica | Configuraciones Básicas]]

Se Realizo la [[VLAN || Configuración de Vlan's ]] y se configuro como [[Configurar como capa 3 || Switch de capa 3]] 

Datos Utilizados: 
- **Hostname:** SWL3-1
- **Nombre del dominio:** redes.local
- **bits en la key:** 2048
- **Mensaje:** Solo Personal Autorizado!!!
- **Usuario:** admin **Contraseña:** cisco
- **Contraseña:** cisco
- **Puertos apagados:** f0/1-20, f0/22-24
- **Puertos Troncales:** f0/21
- **Vlans:**
	- **Vlan:** 10
		- **IP:** 192.168.10.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Estudiantes
	- **Vlan:** 20
		- **IP:** 192.168.20.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Profesores
	- **Vlan:** 30
		- **IP:** 192.168.30.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Invitados
	- **Vlan:** 99
		- **IP:** 192.168.99.3
		- **Mascara:** 255.255.255.0
		- **Nombre:** Admin&Nativa
	- **Vlan:** 100
		- **Nombre:** SinUso
		- **Puertos:** f0/1-20,f0/22-24