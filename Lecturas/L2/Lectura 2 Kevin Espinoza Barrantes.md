**Lectura 2 Kevin Espinoza Barrantes 2023055841**



**1.Explique la diferencia entre una WAN y una MAN.**



&#x20;

MAN: una MAN puede llegar a cubrir hasta 100 km, básicamente conectando solo una área local



WAN: las WAN pueden expandirse de manera geográfica pero no tiene una delimitación en tamaño, el internet es la WAN más grande del mundo, pueden contener millones de computadoras conectadas por subnets.



Está diferencia en su tamaño es el diferenciante entre las MAN y WAN.





**2.Explique las diferencias entre una red orientada a conexión y una red no orientada a conexión**



Red orientada a conexión: Se garantiza una camino por cada conexión por el cual la data llegue en su totalidad y en orden, sucede el apretón de mano que es que el receptor y el remitente intercambian información de control antes de empezar la conexión.



Red no orientada a conexión: No hay un apretón de mano, sin eso el proceso es más rápido y se puede mandar la información de un punto a otro, todo paquete debe tener una dirección a cual enviarse para así saber su destinatario



orientada a conexiones nos permite mandar la información en orden y asegurar la conexión antes que la información que quería ser compartida empiece a trasmitirse mientras que las no orientadas en conexiones al no asegurar la conexión de manera previa son más rápidas pero no se puede asegurar el orden o la totalidad de la información.

&#x20;



**3.¿Qué es una red punto a punto? Explique cómo implementarla de acuerdo con la lectura.**



Es una conexión formada atravez de múltiples nodos en donde la información viaja por muchísimos nodos, un packet tiene que visitar uno o más nodos intermediarios, debido a que existen múltiples rutas es siempre importante encontrar la mejor ruta.



Existen 2 maneras de implementar una red punto a punto: circuit-switched y packet-switched



circuit-switched: creada entre 2 nodos de manera dedicada, una conexión end-to-end se crea entre 2 nodos y la conexión dura mientras haya una transferencia de datos.



packet-switched: los mensajes se dividen en paquetes, los paquetes viajan entre el origen y el destino pasando por packet switches, con buffers en cada switch, cada link tiene buffers de entrada y salida, internet es el mayor ejemplo de una red de este estilo





**4.Explique los conceptos de FDM y TDM**





FDM: El espectro de frecuencias de un enlace que se divide entre múltiples conexiones, asignando una banda de frecuencia distinta a cada conexión durante toda la sesión. Cada conexión transmite simultáneamente pero en su propia frecuencia.





TDM: El tiempo se divide en frames de duración fija, y cada trama se divide a su vez en un número fijo de time slots. Cuando se establece una conexión, se le asigna una ranura específica en cada trama, la cual no se comparte con otras conexiones, el sistema solo puede transmitir datos durante su ranura asignada.



