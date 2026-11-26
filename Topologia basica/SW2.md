```
Switch>enable

Switch#configure terminal

Enter configuration commands, one per line. End with CNTL/Z.

Switch(config)#hostname SW2

SW1(config)#ip domain-name redes.local

SW1(config)#crypto key generate rsa

The name for the keys will be: SW2.redes.local

	Choose the size of the key modulus in the range of 360 to 4096 for your
	
	General Purpose Keys. Choosing a key modulus greater than 512 may take
	
	a few minutes.
	
	  
	
	How many bits in the modulus [512]: 4046
	
	% Generating 4046 bit RSA keys, keys will be non-exportable...[OK]
	

SW1(config)#ip ssh version 2

	*Mar 1 1:50:5.299: %SSH-5-ENABLED: SSH 1.99 has been enabled

SW1(config)#username admin secret cisco

SW1(config)#line console 0

SW1(config-line)#login local

SW1(config-line)#logging synchronous

SW1(config-line)#exit

SW1(config)#line vty 0 15

SW1(config-line)#login local

SW1(config-line)#logging synchronous

SW1(config-line)#transport input ssh

SW1(config-line)#banner motd # Solo Personal Autorizado!!!#

SW1(config)#enable secret cisco

SW1(config)#interface vlan 1

SW1(config-if)#ip address 192.168.1.250 255.255.255.0

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

```

```
Username: admin
Password: 

SW1>enable
Password: 
SW1#configure terminal

Enter configuration commands, one per line.  End with CNTL/Z.

SW1(config)#interface fastethernet0/1

SW1(config-if)#switchport mode access

SW1(config-if)#switchport port-security

SW1(config-if)#switchport port-security mac-address sticky

SW1(config-if)#switchport port-security maximum 1

SW1(config-if)#switchport port-security violation shutdown

SW1(config-if)#exit

SW1(config)#interface range fastethernet0/2-20 

SW1(config-if-range)#switchport mode access

SW1(config-if-range)#switchport port-security

SW1(config-if-range)#switchport port-security mac-address sticky

SW1(config-if-range)#switchport port-security maximum 1

SW1(config-if-range)#switchport port-security violation shutdown

SW1(config-if-range)#exit

SW1(config)#interface range f0/2-5,f0/7-10,f0/12-20 

SW1(config-if-range)#shutdown

	%LINK-5-CHANGED: Interface FastEthernet0/2, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/3, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/4, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/5, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down
	
	%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

SW1(config-if-range)#exit

SW1(config)#exit

	SW1#
	%SYS-5-CONFIG_I: Configured from console by console

SW1#copy running-config startup-config

	Destination filename [startup-config]? 
	Building configuration...
	[OK]

```
