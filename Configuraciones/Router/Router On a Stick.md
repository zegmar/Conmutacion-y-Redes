Router>enable

Router#conf ter

	Enter configuration commands, one per line. End with CNTL/Z.

Router(config)#hostname ***NombreHost***

R1(config)#ip domain-name ***NombreDomaminio***

R1(config)#crypto key generate rsa

The name for the keys will be: R1.redes.local

Choose the size of the key modulus in the range of 360 to 4096 for your

General Purpose Keys. Choosing a key modulus greater than 512 may take

a few minutes.

How many bits in the modulus [512]: ??

% Generating 4096 bit RSA keys, keys will be non-exportable...[OK]

```ad-tip
title: Recomendación 
Usar el **Maximo** posible
```

R1(config)#ip shh version 2

	*Mar 1 0:2:9.547: %SSH-5-ENABLED: SSH 1.99 has been enabled


R1(config)#username ***Usuario*** secret ***Contraseña***

R1(config)#banner motd # ***Mensaje*** #

```ad-caution
title: Mensaje
Se recomienda poner un mensaje de advertencia

No colocar una amenaza o algun mensaje que incite a forzar una entrada. Esto para evitar problemas en situaciones legales
```

R1(config)#enable secret ***Contraseña***

R1(config)#line console 0

R1(config-line)#login local

R1(config-line)#logging synchronous

R1(config-line)#lin vty 0 5

R1(config-line)#login local

R1(config-line)#logging synchronous

R1(config-line)#transport input ssh

R1(config-line)#inter f0/***Puerto***

R1(config-if)#shutdown

R1(config-if)#no shutdown

	R1(config-if)#
	
	%LINK-5-CHANGED: Interface FastEthernet0/0, changed state to up
	
	  
	
	%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/0, changed state to up


R1(config-if)#inter f0/***Subinterfaz***

	R1(config-subif)#

	%LINK-3-UPDOWN: Interface FastEthernet0/0.10, changed state to down
	
	%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/0.10, changed state to up

R1(config-subif)#encapsulation dot1q ***vlan***

R1(config-subif)#ip address ***IP mascara***

R1(config-subif)#exit

R1(config)#exit

	R1#
	
	%SYS-5-CONFIG_I: Configured from console by console

R1#copy running-config startup-config

Destination filename [startup-config]?

Building configuration...

[OK]