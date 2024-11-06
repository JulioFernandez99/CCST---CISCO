# 2.1 Clientes y Servidores

### 2.1.2 Roles de cliente y servidor
Todas las PC conectadas a una red que participan directamente en las comunicaciones de la red se clasifican como hosts. Los hosts pueden enviar y recibir mensajes a través de la red. En las redes modernas, las PC hosts pueden actuar como cliente, servidor o ambos, como se muestra en la figura. El software instalado en la computadora determina cuál es la función que cumple la computadora.

<div align="center">
    <a href="" target="_blank"><img src="recursos\2.1.2.png" style="width:50rem"></a>
</div>

Los servidores son hosts con software instalado que les permite proporcionar información, por ejemplo correo electrónico o páginas web, a otros hosts de la red. Cada servicio requiere un software de servidor independiente. Por ejemplo, para proporcionar servicios Web a la red, un host necesita un software de servidor Web. Cada destino que visita en línea es ofrecido por un servidor ubicado en alguna parte de una red que está conectada a Internet global. 

Los clientes son computadoras host que tienen instalado un software que les permite solicitar información al servidor y mostrar la información obtenida. Un ejemplo de software cliente son los navegadores web como Internet Explorer, Safari, Mozilla Firefox o Chrome.

| Tipo          | Descripción                                                                                                                                                             |
|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Correo electrónico | El servidor de correo electrónico ejecuta el software del servidor de correo electrónico. Los clientes utilizan software de cliente de correo, como Microsoft Outlook, para acceder al correo electrónico en el servidor. |
| Web           | El servidor web ejecuta software de servidor web. Los clientes usan un software de navegador, como Windows Internet Explorer, para acceder a páginas web en el servidor. |
| Archivo       | El servidor de archivos almacena archivos de usuario y empresariales en una ubicación central. Los dispositivos cliente acceden a estos archivos con software cliente como el Explorador de Archivos de Windows. |


### 2.1.3 Redes entre pares
El software de servidor y el de cliente normalmente se ejecutan en computadoras distintas, pero también es posible que una misma computadora los ejecute a ambos a la vez. ```En pequeñas empresas y hogares, muchas PC funcionan como servidores y clientes en la red. Este tipo de red se denomina red entre pares (Peer-to-Peer - P2P).```

La red P2P más simple consta de dos computadoras conectadas directamente mediante una conexión por cable o inalámbrica. Ambas computadoras pueden utilizar esta red simple para intercambiar datos y servicios entre sí; para ello, actuarán como cliente o servidor según sea necesario.

También se pueden conectar varias PC para crear una red P2P más grande, pero esto requiere un dispositivo de red, como un conmutador, para interconectar las computadoras.

La principal desventaja de un entorno P2P es que el rendimiento de un host puede verse afectado si éste actúa como cliente y servidor a la vez. En la figura se enumeran algunas de las ventajas y desventajas de las redes entre pares.
En empresas más grandes, en las que el tráfico de red puede ser intenso, con frecuencia es necesario tener servidores dedicados para poder responder a la gran cantidad de solicitudes de servicio.

Las ventajas y desventajas de las redes entre pares (P2P) se muestran en la figura.

<div align="center">
    <a href="" target="_blank"><img src="recursos\2.1.3.png" style="width:50rem"></a>
</div>

Las ventajas de las redes entre pares:

- Fácil de configurar
- Menos complejo
- Menor costo porque es posible que no se necesiten dispositivos de red ni servidores dedicados.
- Se pueden utilizar para tareas sencillas como transferir archivos y compartir impresoras

Las desventajas de las redes entre pares:

- La administración no está centralizada
- No son tan seguras
- No son escalables
- Todos los dispositivos pueden funcionar como clientes y como servidores, lo que puede lentificar el rendimiento

### 2.1.4 Aplicaciones entre pares
Una aplicación P2P permite que un dispositivo funcione como cliente y como servidor dentro de la misma comunicación, como se muestra en la figura. En este modelo, cada cliente es un servidor y cada servidor es un cliente. Las aplicaciones P2P requieren que cada terminal proporcione una interfaz de usuario y ejecute un servicio en segundo plano.

Algunas aplicaciones P2P utilizan un sistema híbrido donde se descentraliza el intercambio de recursos, pero los índices que apuntan a las ubicaciones de los recursos están almacenados en un directorio centralizado. En un sistema híbrido, cada punto accede a un servidor de índice para obtener la ubicación de un recurso almacenado en otro punto.

<div align="center">
    <a href="" target="_blank"><img src="recursos\2.1.4.png" style="width:50rem"></a>
</div>

Ambos clientes pueden enviar y recibir mensajes simultáneamente.

### 2.1.5 Múltiples Roles en la Red
Una computadora con software de servidor puede proporcionar servicios simultáneamente a uno o muchos clientes, tal como se indica en la figura.

Además, una única PC puede ejecutar varios tipos de software de servidor. En una negocio doméstico o pequeño, puede ser necesario que una PC funcione como servidor de archivos, servidor web y servidor de correo electrónico.

Una única PC también puede ejecutar varios tipos de software de cliente. Debe haber un software de cliente para cada servicio requerido. Si un host tiene varios clientes instalados, puede conectarse a varios servidores de manera simultánea. Por ejemplo, un usuario puede consultar el correo electrónico y ver una página web mientras envía mensajes instantáneos y escucha la radio por Internet.

<div align="center">
    <a href="" target="_blank"><img src="recursos\2.1.5.png" style="width:50rem"></a>
</div>

---
### Pregunta 1
Así es.

Los servidores son hosts con software instalado que les permite proporcionar información, por ejemplo correo electrónico o páginas Web, a otros hosts de la red.

---
### Pregunta 2
Así es.

Los clientes son computadoras host que tienen instalado un software que les permite solicitar información al servidor y mostrar la información obtenida.




---
### Pregunta 3
Así es.

Una red entre pares consiste en dos computadoras conectadas directamente donde ambas computadoras pueden intercambiar datos y servicios entre sí, actuando como cliente o servidor según sea necesario.


---
<br>

# 2.2 Componentes de la red

### 2.2.2 Infraestructura de red
El trayecto que toma un mensaje desde el origen al destino puede ser tan simple como un solo cable que conecta una computadora con otra o tan complejo como una red que, literalmente, abarca todo el planeta. Esta infraestructura de red es la plataforma que da soporte a la red. Proporciona el canal estable y confiable por el cual se producen las comunicaciones.

La infraestructura de red contiene tres categorías de componentes de hardware, como se muestra en la figura:

- Dispositivos finales
- Dispositivos intermedios
- Medios de red

<div align="center">
    <a href="" target="_blank"><img src="recursos\2.2.2.png" style="width:50rem"></a>
</div>

Los dispositivos y los medios son los elementos físicos o hardware de la red. Por lo general, el hardware está compuesto por los componentes visibles de la plataforma de red, como una PC portátil, una PC, un switch, un router, un punto de acceso inalámbrico o el cableado que se utiliza para conectar estos dispositivos. A veces, puede que algunos componentes no sean visibles. En el caso de los medios inalámbricos, los mensajes se transmiten a través del aire mediante radio frecuencias invisibles u ondas infrarrojas.

Haga una lista de los componentes de la infraestructura de red instalados en su red doméstica. Incluya los cables o puntos de acceso inalámbrico que proporcionan sus conexiones de red.

### 2.2.3 Dispositivos finales
Los dispositivos de red con los que las personas están más familiarizadas se denominan “dispositivos finales” o “hosts”. Estos dispositivos forman la interfaz entre los usuarios y la red de comunicación subyacente.

Algunos ejemplos de dispositivos finales son:

Computadores (estaciones de trabajo, PC portátiles, servidores de archivos, servidores web)
Impresoras de red
Teléfonos y equipo de teleconferencias
Cámaras de seguridad
Dispositivos móviles (como smartphones, tablets, PDA y lectores inalámbricos de tarjetas de débito y crédito, y escáneres de códigos de barras)
Un dispositivo final (o host) es el origen o el destino de un mensaje transmitido a través de la red, tal como se muestra en la animación. Para identificar los hosts de forma exclusiva, se usan direcciones. Cuando un host inicia la comunicación, utiliza la dirección del host de destino para especificar a dónde se debe enviar el mensaje.

---
### Pregunta 1
¡Así es! Bien hecho.

En las zonas rurales que no cuentan con una infraestructura de telecomunicaciones por cable, el acceso inalámbrico a través de un servicio celular suele ser la única opción para el acceso a Internet. Las opciones para Marjani incluyen un teléfono inteligente o una tableta.

---
### Pregunta 2
¡Así es! Bien hecho.

Las redes domésticas generalmente se conectan al proveedor de servicios de Internet mediante un módem y un router con capacidades inalámbricas. A veces, estos dos dispositivos se combinan en un solo dispositivo. En este escenario, Eilert deberá llevar el router inalámbrico a la casa del cliente, ya que este solo tiene el módem.

---
### Pregunta 3
¡Así es! Bien hecho.

Los trabajadores de salud comunitarios que viajan de casa en casa durante sus rondas diarias dependen en gran medida del acceso inalámbrico. Por lo tanto, es muy probable que Rosalía utilice una tableta y medios inalámbricos para conectarse a Internet para actualizar los registros médicos y las videoconferencias con otro médico, cuando sea necesario.


