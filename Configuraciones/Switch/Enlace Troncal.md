SW1(config-if-range)#inter range f0/***Puertos troncales***

SW1(config-if-range)#switchport mode trunk
	Mensajes de cambio a Trunk Mode

SW1(config-if-range)#switchport trunk native vlan ***Vlan Dedicada***
	Mensajes de cambio
  
SW1(config-if-range)#switchport trunk allowed vlan ***Vlan's aceptadas***

SW1(config-if-range)#exit

SW1(config)#exit

SW1#coppy running-config startup-config
	
	^
	
	% Invalid input detected at '^' marker.
	
	SW1#copy running-config startup-config
	
	Destination filename [startup-config]?
	
	Building configuration...
	
	[OK]