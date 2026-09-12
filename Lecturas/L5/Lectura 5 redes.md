**Lectura 5 redes**



**Kevin Alonso Espinoza Barrantes**



**¿Cómo funciona el Port-Based Authentication?**



Cotrola el acceso a la red a nivel del puerto físico o lógico de un switch o punto de acceso. Cuando un dispositivo (lo que se llama supplicant) intenta conectarse, el puerto permanece en estado "no autorizado" y solo permite tráfico de autenticación, bloqueando cualquier otro tipo de tráfico como DHCP o navegación. El authenticator (switch/AP) reenvía las credenciales del supplicant a un servidor de autenticación, el cual valida la identidad. Si la autenticación es exitosa, el puerto pasa a estado autorizado y el dispositivo obtiene acceso normal a la red, si falla, el puerto permanece bloqueado.





**Defina los componentes principales de 802-1x.**



* Supplicant: el dispositivo cliente que solicita acceso a la red 
* Authenticator: el dispositivo de red (switch o access point) que controla el acceso al puerto y actúa como intermediario entre el supplicant y el servidor de autenticación.
* Authentication Server: típicamente un servidor RADIUS, encargado de verificar las credenciales del supplicant y decidir si se concede o niega el acceso.







**¿Por qué considera que este tipo de autenticación es relevante?**





porque añade una capa de seguridad a nivel de acceso a la red, evitando que dispositivos no autorizados se conecten simplemente por tener acceso físico a un puerto de red o a una señal inalámbrica. Esto es especialmente importante en entornos corporativos o educativos con muchos puntos de conexión, ya que centraliza el control de identidad y previene accesos indebidos, reduciendo el riesgo de ataques internos o de dispositivos desconocidos conectados a la infraestructura.

