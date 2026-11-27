SW3(config)#interface port-channel ***NumeroDeChannel***

SW3(config-if)#switchport mode trunk

SW3(config-if)#switchport trunk native vlan ***Vlan***

SW3(config-if)#switchport trunk allowed vlan ***Vlan/vlan's***

SW1(config-if)#interface range f0/***Puertos***

SW1(config-if-range)#channel-group ***NumeroDelChannel*** mode active