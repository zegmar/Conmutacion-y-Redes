
 ```ad-example
title: enable (ena)
 Entrar al modo privilegiado. Es el primer paso para cualquier configuración.
 ```

```ad-example
title: configure terminal (conf t)
Entrar al modo de configuración global, donde se hacen casi todos los cambios.
```

```ad-example
title: exit (ex)
Retroceder un solo nivel (de interfaz a config global, por ejemplo).
```

```ad-example
title: end
Salir de golpe hasta el modo privilegiado desde cualquier submodo.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: do wr
Guardar la configuración sin salir del modo de configuración (forma corta).
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```

```ad-example
title: copy running-config startup-config
Guardar la configuración en la NVRAM para que no se pierda al reiniciar.
```




- hostname [nombre]

- Asignar nombre al equipo para identificarlo en la topología.

- banner motd #[mensaje]#

- Mostrar un mensaje de advertencia a quien se conecte.

- enable secret [clave]

- Proteger el modo privilegiado con una contraseña cifrada.

- service password-encryption

- Cifrar las contraseñas que estén en texto plano en la configuración.

- ip domain-name [dominio]

- Configurar el dominio. Es requisito para generar las llaves de SSH.

- crypto key generate rsa

- Generar las llaves criptográficas RSA que usa SSH.

- ip ssh version 2

- Activar SSH versión 2, la más segura.

- username [usuario] secret [clave]

- Crear un usuario local con contraseña cifrada (lo usa login local).

- line console 0

- Entrar a la línea de consola (acceso físico por cable).

- line vty 0 15

- Entrar a las 16 líneas de acceso remoto del switch (Telnet/SSH).

- login local

- Exigir usuario y contraseña locales para entrar por esa línea.

- transport input ssh

- Permitir acceso remoto solo por SSH (bloquea Telnet).

- logging synchronous

- Evitar que los mensajes del sistema interrumpan lo que estás escribiendo.

- interface vlan 1

- Entrar a la interfaz virtual de administración del switch.

- ip address [IP] [máscara]

- Asignar una dirección IP a la interfaz (aquí, la IP de gestión del switch).

- ip default-gateway [IP]

- Dar al switch su puerta de enlace para administrarlo desde otra red.

- no shutdown

- Encender la interfaz.

- shutdown

- Apagar la interfaz (por ejemplo, puertos sin usar).