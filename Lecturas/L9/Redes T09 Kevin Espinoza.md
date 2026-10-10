**Redes T09 Kevin Espinoza**

**Preguntas:**



**¿Qué es un firewall? Comente los tipos existentes en capa 3/4**



Un firewall es un sistema puede ser un programa o un equipo que controla el tráfico que entra y sale de una red. Funciona como un guardia de seguridad que revisa cada paquete y, según unas reglas, decide si lo deja pasar o lo bloquea. Su objetivo es proteger la red de accesos no autorizados.



* Filtrado de paquetes (packet filtering): El más básico el cual revisa cada paquete de forma individual y mira la IP de origen, la IP de destino, el protocolo y el puerto. Si coincide con la regla, lo permite si no lo bloquea. Es rápido pero no recuerda nada de conexiones anteriores.
* Firewall con estado (stateful): Además de revisar el paquete, recuerda el estado de la conexión. Por ejemplo: solo deja entrar una respuesta si antes alguien de adentro hizo la petición. Es más seguro que el filtrado simple.
* Gateway a nivel de circuitos (circuit-level): Trabaja en capa 4. Verifica que el establecimiento de la conexión TCP sea válido y una vez aprobado, deja pasar el tráfico sin revisar el contenido.



**¿Qué es un bastion host?**



Es un computador que se coloca en un punto expuesto de la red, normalmente de cara a internet, y que está muy bien protegido porque se espera que reciba ataques. Solo tiene instalados los servicios estrictamente necesarios, se mantiene actualizado y se vigila de cerca. Sirve como puerta de entrada controlada a la red interna, y si alguien lo ataca, el daño queda limitado a ese equipo y no a toda la red.





**¿En qué consiste un DMZ?**



DMZ significa zona desmilitarizada. Es una red intermedia que queda entre internet y la red interna de una organización. Ahí se colocan los servidores que necesitan ser accesibles desde afuera, como el servidor web, el de correo o el de DNS.



La idea es que, si un atacante logra entrar a uno de esos servidores, solo llegue a la DMZ y no a la red interna con la información más importante. Normalmente se separa con firewalls uno entre internet y la DMZ y otro entre la DMZ y la red interna.





**¿Qué es un Proxy server?**



Es un servidor que actúa como intermediario entre los usuarios y internet. En lugar de que la computadora se conecte directamente a una página se hace la petición al proxy y este la hace por él devolviendo la respuesta luego.



Nos sirve para:



* Ocultar la IP real de los usuarios.
* Filtrar o bloquear sitios web.
* Guardar copias de páginas visitadas (la caché) para que carguen más rápido.
* Registrar y controlar qué hace cada usuario.





**Explique los diferentes protocolos de VPN**





Una VPN crea un camino cifrado a través de internet de forma que los datos viajan protegidos como si fuera una red privada. Los protocolos son las distintas formas de construir ese túnel, son los siguientes:





* PPTP: Es de los más antiguos. Es fácil de configurar y rápido, pero tiene un cifrado débil y hoy se considera inseguro.
* L2TP/IPsec: L2TP crea el túnel y IPsec se encarga de cifrarlo. Es más seguro que PPTP, pero es un poco más lento porque encapsula los datos dos veces.
* IPsec: Es un conjunto de reglas que cifra y autentica los paquetes en la capa de red. Se usa mucho para conectar oficinas entre sí (VPN sitio a sitio).
* SSL/TLS (por ejemplo, OpenVPN): Usa el mismo cifrado que usan las páginas web seguras (HTTPS). OpenVPN es muy seguro, flexible y de código abierto, aunque requiere instalar un programa.
* SSTP: Es un protocolo de Microsoft que usa SSL/TLS por el puerto 443, por lo que pasa fácilmente por firewalls. Funciona sobre todo en Windows.
* IKEv2/IPsec: Es rápido y estable, y se recupera bien si se pierde la conexión, por ejemplo al cambiar de WiFi a datos móviles. Por eso es muy usado en celulares.
* WireGuard: Es el más nuevo. Es muy rápido, simple y seguro, y usa cifrado moderno.

