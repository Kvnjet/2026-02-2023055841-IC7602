**Lectura 4 Kevin Espinoza**



**¿En qué consiste ARP?**



Es un protocolo que permite mapear una dirección IP a la dirección física MAC correspondiente dentro de una red local. Es necesario porque aunque los dispositivos se identifican lógicamente por IP, la entrega real de frames en una LAN requiere la dirección MAC del destinatario.





**¿Cómo funciona ARP?**



1. El emisor conoce la IP del destino.
2. IP le pide a ARP crear un mensaje de solicitud con la IP y dirección física del emisor, la IP del destino y el campo de dirección física del destino en ceros.
3. El mensaje se encapsula en un frame usando la dirección física del emisor como origen y la dirección de broadcast como destino.
4. Todos los hosts reciben el frame solo la máquina cuya IP coincide reconoce la solicitud, las demás la descartan.
5. La máquina destino responde con un mensaje ARP reply que contiene su dirección física, enviado de forma unicast.
6. El emisor recibe la respuesta y ya conoce la dirección física del destino.
7. El datagrama IP se encapsula en un frame y se envía de forma unicast al destino.





**¿Cuáles considera son las ventajas y desventajas de Static y Dynamic Mapping?**



Static Mapping: se crea una tabla que asocia cada dirección lógica con su dirección física en cada máquina. Las direcciones físicas pueden cambiar, por lo que la tabla debe actualizarse periódicamente, lo cual genera overhead y afecta el rendimiento de la red, al ya tener las direcciones físicas guardadas en la tabla, no es necesario enviar solicitudes por la red cada vez que una máquina necesita conocer una dirección



Dynamic Mapping: cada vez que una máquina conoce la dirección lógica de otra, puede usar un protocolo (ARP) para encontrar la dirección física automáticamente. No requiere mantenimiento manual de tablas, se adapta a los cambios de dirección física sin overhead administrativo, cada resolución requiere enviar una solicitud ARP en broadcast a toda la red, lo que genera tráfico adicional





**¿Cuáles son las aplicaciones de un Proxy ARP?**



Un Proxy ARP es un router que actúa en nombre de un conjunto de hosts, creando un efecto de subnetting. Cuando el router recibe una solicitud ARP buscando la IP de uno de esos hosts, responde con su propia dirección física al recibir el paquete IP real, lo reenvía al host o router correspondiente. Se usa para crear una subred sin necesidad de reconfigurar todo el sistema para reconocer direcciones subneteadas, el router administra las solicitudes ARP de los hosts protegidos en la subred añadida.







**¿Cómo funciona el ARP spoofing? Puede usar otros recursos para dar respuesta a esta pregunta.**



El ARP spoofing aprovecha que ARP no fue diseñado con seguridad, no verifica que una respuesta provenga realmente de la parte autorizada y los hosts aceptan respuestas ARP incluso sin haberlas solicitado. Un atacante envía mensajes ARP falsificados para asociar su propia dirección MAC con la IP de otro host, logrando que el tráfico destinado a esa IP se le envíe a él en lugar del destino legítimo. Esto le permite realizar un ataque de intermediario: interceptar, espiar, modificar o bloquear el tráfico entre las víctimas.



