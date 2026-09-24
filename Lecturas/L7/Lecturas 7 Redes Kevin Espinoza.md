**Lecturas 7 Redes Kevin Espinoza**



**Comente de acuerdo a la lectura las principales características de WEP, WAP y WAP2:**



WEP: Fue el primer protocolo de seguridad inalámbrica, su objetivo era darle cifrado a los datos que viajan por la red. El problema es que la manera en que lo hacía era bastante débil, todos los equipos compartían la misma clave y esa clave era tan corta y predecible que, con el equipo correcto, alguien podía capturar el tráfico y sacarla sin mucho esfuerzo, en la práctica esto terminó siendo una protección casi simbólica.



WPA: Apareció en 2003 como una mejora de WEP, impulsada por la Wi-Fi Alliance para corregir sus problemas de autenticación e integridad de datos. Conserva una base parecida a WEP pero le agrega TKIP, un mecanismo que envuelve al cifrado original y va cambiando las claves periódicamente, lo que hace mucho más difícil romper la seguridad. También suma un código de integridad de mensajes (MIC) para detectar si un paquete fue alterado. Aun así, con el tiempo aparecieron ataques (como el de Beck y Tews) capaces de aprovechar debilidades de TKIP.



WPA2: Es la evolución de WPA, publicada en 2004 como una apuesta por el AES. Su cambio principal es dejar atrás TKIP y usar este cifrado AES que es mucho más robusto y es todavía vigente hoy. Permite autenticarse tanto con una clave precompartida (que es típico en redes domésticas), como con un servidor de autenticación (esto es lo usual en empresas). Es el más seguro de los tres, aunque su punto débil sigue siendo la fortaleza de la clave precompartida que elija el usuario, ya que puede quedar expuesta a ataques de diccionario o de fuerza bruta.

