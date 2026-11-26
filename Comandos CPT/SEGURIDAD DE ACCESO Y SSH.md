- enable secret cisco: Configurar contraseña para el modo privilegiado.

- service password-encryption: Cifra las contraseñas en texto plano.

- username name secret password: Asigna nombre de usuario y contraseña.

- ip domain-name name: Asigna nombre al dominio.

- crypto key generate rsa: Hace claves criptográficas.

- ip ssh version 2: Habilita y fuerza el uso de la versión 2 del protocolo SSH para mayor seguridad en las conexiones remotas.

- Line vty 0 15: Se configura de forma simultanea las 16 líneas remotas que puede soportar el switch.

- transport input ssh: Obliga a que el switch solamente acepte transmisiones por ssh.

- Login local: Autentica al usuario mediante usuario y contraseña.

```ad-warning
title: Importante
Es preferible usar username name secret password en VTY para el reconocimiento login local

```

- ip ssh -l username ip address: Acceso remoto desde una pc a x dispositivo.


