
Switch>enable

Switch#configure terminal

Enter configuration commands, one per line. End with CNTL/Z.

Switch(config)#hostname ***NombreHost***

SW1(config)#ip domain-name ***NombreDominio***

SW1(config)#crypto key generate rsa

The name for the keys will be: ***NombreHost.NombreDominio***

	Choose the size of the key modulus in the range of 360 to 4096 for your
	
	General Purpose Keys. Choosing a key modulus greater than 512 may take
	
	a few minutes.
	
	  
	
	How many bits in the modulus [512]: ***??***
	
	% Generating 4046 bit RSA keys, keys will be non-exportable...[OK]

```ad-tip
title: Recomendación 
Usar el **Maximo** posible
```

SW1(config)#ip ssh version 2

	*Mar 1 1:50:5.299: %SSH-5-ENABLED: SSH 1.99 has been enabled

SW1(config)#username ***Usuario*** secret ***Contraseña***

SW1(config)#line console 0

SW1(config-line)#login local

SW1(config-line)#logging synchronous

SW1(config-line)#exit

SW1(config)#line vty 0 15

SW1(config-line)#login local

SW1(config-line)#logging synchronous

SW1(config-line)#transport input ssh

SW1(config-line)#banner motd # ***Mensaje*** #

```ad-caution
title: Mensaje
Se recomienda poner un mensaje de advertencia

No colocar una amenaza o algun mensaje que incite a forzar una entrada. Esto para evitar problemas en situaciones legales
```

SW1(config)#enable secret ***contraseña***

SW1(config)#interface vlan 1

SW1(config-if)#ip address ***IP Mascara***

SW1(config-if)#no shutdown
  
	SW1(config-if)#
	
	%LINK-3-UPDOWN: Interface Vlan1, changed state to down

SW1(config-if)#exit

SW1(config)#exit

	SW1#
	
	%SYS-5-CONFIG_I: Configured from console by console


SW1#copy running-config startup-config

Destination filename [startup-config]?

Building configuration...

[OK]

SW1#configure terminal

Enter configuration commands, one per line.  End with CNTL/Z.

SW1(config)#interface range fastethernet0/1-20 

SW1(config-if-range)#switchport mode access

SW1(config-if-range)#switchport port-security

SW1(config-if-range)#switchport port-security mac-address sticky

SW1(config-if-range)#switchport port-security maximum 1

SW1(config-if-range)#switchport port-security violation shutdown

SW1(config-if-range)#exit

SW1(config)#interface range f0/***Puertos que no se están utilizando***

SW1(config-if-range)#shutdown
	***Mensaje de puertos apagados***

SW1(config-if-range)#exit

SW1(config)#exit

	SW1#
	%SYS-5-CONFIG_I: Configured from console by console

SW1#copy running-config startup-config

	Destination filename [startup-config]? 
	Building configuration...
	[OK]
