Kevin Alonso Espinoza Barrantess

2023055841



Preguntas:

&#x20;

1\. Explique cómo se originó el Internet.



Las primeras veces que se hablo acerca de interacciones sociales mediante redes fueron escritos en memos de J.C.R Licklider del MIT en 1962 que hablo de crear una "Galatic Network" que en la practica es muy parecido al internet actual, en 1961 Kleinrock publico su primera teoría del packet switching después sacando un libro en 1964, Licklider fue la cabeza del proyecto DARPA que inicio en 1962, se inicio practicando las conexiones con líneas telefónicas y en 1965 se logro conectar por primera vez a 2 computadoras y estás pudieron comunicarse, 1966 se inicio con el plan de ARPANET, el MIT, RAND y NPL empezaron a hacer trabajos sobre el tema en paralelo sin saberlo, el Network Measumerent Center de Kleinrock en UCLA fue el primer nodo de ARPANET, en 1969 se puso el primer host en UCLA y el SRI se volvió el segundo nodo, para los finales de 1969 4 computadoras host estaban conectadas en ARPANET.



En 1970 el NWG termino el protocoto Host-to-Host inicial de ARPANET, el NCP, durante 1971-1972 los usuarios de la red pudieron empezar a desarrollar aplicaciones, En 1972 ARPANET fue presentado al publico y pronto después salió la primera gran aplicación de la red: el email, desde ese punto el ARPANET creció hasta ser el internet que conocemos hoy en día   	 





2\. De acuerdo con la lectura, ¿Qué es circuit switching y packet switching?



Packet switching: usar paquetes para comunicarse en vez de circuitos, separa la información en paquetes pequeños que viajan por separado y se juntan al llegar al destino, se enruta de manera independiente 



Circuit Switching: Las redes se conectan mediante circuitos, mandando bits de manera sincronizada y reservada junto con una parte de un circuito end-to-end, todo esto entre un par de localizaciones 



3\. Qué tanto impacto causó las “Four ground rules” en el Desarrollo de las comunicaciones actuales? Base su respuesta en su conocimiento actual de cómo funcionan las redes, comunicaciones y el Internet.



Fueron de una gran importancia, sin cada red teniendo que mantenerse por si sola no podríamos convivir con tantos tipos de redes al mismo tiempo (Wi-fi, fibra óptica, satelital etc...), sin gateways y routers que no guardaran información no podríamos haber escalado el internet de manera sencilla e ilimitada.

Confiar solamente desde el punto base de donde vino la información nos permite confiar en los routers los cuales no pueden retrasmitir un mensaje ya que eso es responsabilidad de la fuente y esto está fuertemente relacionado con el TCP y los principios end-to-end y la libertad que se vive en el apartado operativo de las redes al no haber una autoridad central.



4\. Explique el rol de la documentación en las redes.



Al contrario que la documentación científica o formal en las redes se ocupa informar de manera rápida y concisa, por eso se creo el RFC que son fácilmente accesibles desde la web, también se popularizo el uso de emails personalizado, los RFC tenían el objetivo de crear un loop de criticas positivas que transformara la tecnología, la primera información que las redes se concentraron en trasmitir era la información de su propio diseño.



5\. En la lectura se mencionan múltiples dispositivos de red, así como protocolos, por ejemplo satélites, ethernet y routers (pero no se limita solo a estos), extraiga todos estos nombres de dispositivos y mediante alguna herramienta de Inteligencia artificial generativa (que se debe especificar), proporcione una definición de cada dispositivos en el ámbito de redes además pregunte ¿A que capa del modelo de referencia OSI pertenece el dispositivo o protocolo?



Los dispositivos y protocolos fueron extraídos del texto fuente y definidos con apoyo de Claude Anthropic, modelo Sonnet 4.5 en eficacia media.





1\. SNMP (Simple Network Management Protocol)

Protocolo diseñado para la gestión y monitoreo de dispositivos en una red IP (routers, switches, servidores, impresoras, etc.), permitiendo consultar y modificar variables de estado (como tráfico, errores, temperatura de un dispositivo) desde una estación de gestión central.

Capa OSI: Capa 7 (Aplicación) — opera sobre UDP y es un protocolo de aplicación usado por software de administración de red.



2\. CMIP (Common Management Information Protocol)

Protocolo de gestión de red alternativo a SNMP, desarrollado bajo el estándar OSI. Ofrecía funciones más robustas (orientado a objetos, con mejor seguridad y manejo de eventos), pero fue mucho más complejo de implementar, razón por la cual el mercado terminó prefiriendo SNMP como solución "de corto plazo" que se volvió dominante.

Capa OSI: Capa 7 (Aplicación) — al igual que SNMP, es un protocolo de gestión que opera en el nivel de aplicación.



3\. Router

Dispositivo de red que interconecta redes distintas (o segmentos de red) y decide, mediante tablas de enrutamiento, el mejor camino para reenviar paquetes de datos entre origen y destino. Es el dispositivo central en la arquitectura de "gateways" descrita por las cuatro reglas de Kahn.

Capa OSI: Capa 3 (Red) — toma decisiones de reenvío basadas en direcciones IP.



4\. Packet Satellite Network (Red de Paquetes por Satélite / SATNET)

Tecnología de red que usaba enlaces satelitales para transmitir paquetes de datos entre estaciones terrestres muy distantes geográficamente (por ejemplo, entre EE.UU. y Europa), permitiendo interconectar redes que no podían enlazarse por cable. Fue una de las redes originales que se integró a la arquitectura de Internet, validando que el diseño de Kahn/Cerf pudiera funcionar sobre medios heterogéneos.

Capa OSI: Capa 1 y 2 (Física y Enlace de Datos) — el satélite provee el medio de transmisión física y el enlace punto a punto/broadcast.



5\. Packet Radio Network

Red experimental de DARPA que transmitía paquetes de datos mediante señales de radio en lugar de líneas físicas, pensada originalmente para comunicaciones móviles/militares. Al igual que Packet Satellite, fue clave para demostrar que el protocolo TCP/IP podía operar sobre medios de transmisión muy distintos entre sí (la motivación original detrás del diseño "internetworking" de Cerf y Kahn).

Capa OSI: Capa 1 y 2 (Física y Enlace de Datos) — la radio es el medio físico y define cómo se accede al canal compartido.



6\. World Wide Web / Browsers

Software de aplicación (no un protocolo de red por sí mismo) que permite a los usuarios acceder e interactuar con información distribuida globalmente mediante hipertexto, utilizando protocolos como HTTP. Su adopción masiva fue lo que aceleró la comercialización de Internet descrita en el texto.

Capa OSI: Capa 7 (Aplicación) — es la interfaz de usuario final que consume el protocolo HTTP.

