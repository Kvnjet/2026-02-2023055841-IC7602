**Lectura 8 Kevin Espinoza Redes**



**Explique el funcionamiento de ICMP.**



Es un protocolo auxiliar de IP que informa errores y envía mensajes de control entre hosts y gateways. IP no es confiable y no avisa si un datagrama se pierde, así que ICMP notifica al origen cuando algo falla (destino inalcanzable, TTL agotado, problema en el encabezado, congestión). Sus mensajes viajan encapsulados en datagramas IP (protocolo 1) y llevan los campos Type, Code y Checksum, además del encabezado del datagrama original que causó el error. ICMP solo reporta y no garantiza la entrega.







**Comente las aplicaciones de este protocolo en las comunicaciones.**



* **Ping:** verifica si un host es alcanzable y mide el tiempo de ida y vuelta (Echo / Echo Reply).
* **Traceroute:** descubre la ruta salto a salto usando Time Exceeded.
* **Reporte de errores:** informa destinos, puertos o redes inalcanzables.
* **Control de congestión:** Source Quench pide al emisor reducir la velocidad.
* **Optimización de rutas:** Redirect indica una mejor ruta.
* **Monitoreo y diagnóstico:** permite a los administradores detectar fallas y medir latencia.



