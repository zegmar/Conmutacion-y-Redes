SWL3-1(config)#ip routing

SWL3-1(config)#inter f0/***Puerto***

SWL3-1(config-if)#switchport trunk encapsulation dot1q

SWL3-1(config-if)#switchport mode trunk

SWL3-1(config-if)#switchport trunk native vlan ***vlan***

SWL3-1(config-if)#switchport trunk allowed vlan ***vlan's***

SWL3-1(config-if)#ex

SWL3-1(config)#ex

SWL3-1#

	%SYS-5-CONFIG_I: Configured from console by console

  

SWL3-1#copy running-config startup-config

	Destination filename [startup-config]?
	
	Building configuration...
	
	[OK]