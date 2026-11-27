SW1#conf ter

	Enter configuration commands, one per line. End with CNTL/Z.

SW1(config)#vlan ***NumeroX***

SW1(config-vlan)#name ***NombreVlan***

SW1(config-vlan)#exit

SW1(config)#vlan ***NumeroX***

SW1(config-vlan)#name Profesores

SW1(config-vlan)#exit

SW1(config)#inter range f0/***Puertos que tendran accesos a la Vlan***

SW1(config-if-range)#switchport access vlan ***Numero de la Vlan***

```ad-attention
title: Recomendacion
Se recomienda tener una **Vlan** dedicada para los puertos sin uso y una para la administracion 
```

SW1(config-if-range)#exit

SW1(config)#exit

SW1#coppy running-config startup-config
	^
	
	% Invalid input detected at '^' marker.
	
	SW1#copy running-config startup-config
	
	Destination filename [startup-config]?
	
	Building configuration...
	
	[OK]

