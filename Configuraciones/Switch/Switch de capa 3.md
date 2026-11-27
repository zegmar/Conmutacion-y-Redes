ip routing

Habilitar el enrutamiento en un switch multicapa (L3).

interface vlan [id]

Crear la SVI: interfaz virtual enrutada que sirve de gateway de la VLAN.

no switchport

Convertir un puerto del switch L3 en puerto enrutado (capa 3) para conectarlo a un router.

switchport trunk encapsulation dot1q

Definir el protocolo de etiquetado. En switch L3 va antes de switchport mode trunk.