
%LINK-5-CHANGED: Interface GigabitEthernet0/2, changed state to administratively down

SWL3-1(config-if-range)#inter f0/21

SWL3-1(config-if)#exit

SWL3-1(config)#ip routing

SWL3-1(config)#inter f0/21

SWL3-1(config-if)#no switchport

SWL3-1(config-if)#exit

SWL3-1(config)#vlan 10

SWL3-1(config-vlan)#name Estudiantes

SWL3-1(config-vlan)#ip address 192.168.10.254 255.255.255.0

^

% Invalid input detected at '^' marker.

SWL3-1(config-vlan)#exit

SWL3-1(config)#vlan 20

SWL3-1(config-vlan)#name Profesores

SWL3-1(config-vlan)#vlan 30

SWL3-1(config-vlan)#name Invitados

SWL3-1(config-vlan)#vlan 99

SWL3-1(config-vlan)#name Admin&Nativa

SWL3-1(config-vlan)#intere vlan 10

^

% Invalid input detected at '^' marker.

SWL3-1(config-vlan)#inter vlan 10

SWL3-1(config-if)#

%LINK-5-CHANGED: Interface Vlan10, changed state to up

  

SWL3-1(config-if)#ip address 192.168.10.254 255.255.255.0

SWL3-1(config-if)#inter vlan 20

SWL3-1(config-if)#

%LINK-5-CHANGED: Interface Vlan20, changed state to up

  

SWL3-1(config-if)#ip address 192.168.20.254 255.255.255.0

SWL3-1(config-if)#inter vlan 30

SWL3-1(config-if)#

%LINK-5-CHANGED: Interface Vlan30, changed state to up

  

SWL3-1(config-if)#ip address 192.168.30.254 255.255.255.0

SWL3-1(config-if)#inter vlan 99

SWL3-1(config-if)#

%LINK-5-CHANGED: Interface Vlan99, changed state to up

  

SWL3-1(config-if)#ip address 192.168.99.254 255.255.255.0

SWL3-1(config-if)#inter f0/21

SWL3-1(config-if)#switchport

SWL3-1(config-if)#switchport mode trunk

Command rejected: An interface whose trunk encapsulation is "Auto" can not be configured to "trunk" mode.

SWL3-1(config-if)#switchport mode access

SWL3-1(config-if)#switchport mode trunk

SWL3-1(config-if)#switchport trunk vlan 99

^

% Invalid input detected at '^' marker.

SWL3-1(config-if)#switchport trunk native vlan 99

SWL3-1(config-if)#switchport trunk allowed vlan 10,20,30,99

SWL3-1(config-if)#exit

SWL3-1(config)#exit

SWL3-1#

%SYS-5-CONFIG_I: Configured from console by console

  

SWL3-1#copy running-config startup-config

Destination filename [startup-config]?

Building configuration...

[OK]