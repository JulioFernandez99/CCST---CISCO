# 5.1 Protocolos de comunicación

### 5.1.1 Protocolos de Comunicación
La comunicación en nuestra vida cotidiana tiene diferentes formas y existe en muchos entornos. Tenemos diferentes expectativas dependiendo de si estamos conversando por Internet o participando en una entrevista de trabajo. Cada situación tiene su comportamiento y estilo correspondiente.

Antes de comenzar a comunicarnos, establecemos reglas o acuerdos que rigen la conversación. Estos acuerdos incluyen lo siguiente:

¿Cuál método de comunicación debemos utilizar?
¿Qué idioma debemos usar?
¿Debemos confirmar que se reciben nuestros mensajes?
Haga clic a continuación para ver un ejemplo de determinación del método, el idioma y las estrategias de confirmación.

<details>
        <summary>Metodo</summary>
        <div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.1.1.3.png" style="width:50rem"></a>
        </div>
</details>  
<br>

<details>
        <summary>Idioma</summary>
        <div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.1.1.2.png" style="width:50rem"></a>
        </div>
</details>  
<br>

<details>
        <summary>Confirmacion</summary>
        <div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.1.1.3.png" style="width:50rem"></a>
        </div>
</details>  
<br>


---

### 5.1.2 Por Qué Importan los Protocolos
Las computadoras, al igual que los seres humanos, utilizan reglas o protocolos para comunicarse. Los protocolos son necesarios para que las computadoras se comuniquen correctamente a través de la red. Tanto en un entorno cableado como en uno inalámbrico, una red local se define como un área en la que todos los hosts deben "hablar el mismo idioma" lo que, en términos informáticos, significa que deben "compartir un protocolo común". Si todas las personas de una misma sala hablaran idiomas diferentes, no podrían comunicarse. De manera similar, si los dispositivos de una red local no utilizaran los mismos protocolos, no podrían comunicarse. Los protocolos de red definen muchos aspectos de la comunicación a través de la red local. Como se muestra en la tabla, estos incluyen formato de mensaje, tamaño de mensaje, temporización, codificación, encapsulamiento y patrones de mensaje.

| **Características de los protocolos** | **Descripción** |
|---------------------------------------|-----------------|
| **Formato del mensaje**               | Cuando se envía un mensaje se debe utilizar un formato o estructura específicos. Los formatos de los mensajes dependen del tipo de mensaje y el canal que se utilice para entregar el mensaje. |
| **Tamaño del mensaje**                | Las reglas que controlan el tamaño de las partes que se comunican a través de la red son muy estrictas. También pueden variar de acuerdo con el canal utilizado. Los mensajes largos pueden dividirse en partes más pequeñas para garantizar su entrega confiable. |
| **Sincronización**                    | La sincronización determina la velocidad de transmisión de bits en la red, además de afectar cuándo un host puede enviar datos y la cantidad de datos en una transmisión. |
| **Codificación**                      | El host emisor convierte los mensajes en bits, que son codificados en patrones de sonidos, ondas de luz o impulsos electrónicos según el medio de transmisión. El host de destino decodifica las señales para interpretar el mensaje. |
| **Encapsulamiento y Patrón del mensaje** | Cada mensaje debe incluir un encabezado con información de direcciones de origen y destino para su entrega. La encapsulación añade esta información a los datos del mensaje. Algunos mensajes requieren confirmación de recepción, mientras otros pueden transmitirse sin confirmar su entrega. | 

---

# 5.2 Estándares de Comunicación

### DHCP/ICMPv6

Los protocolos DHCP e ICMPv6 proporcionan información de direccionamiento IP y configuración de red. DHCP (Protocolo de Configuración Dinámica de Host) asigna automáticamente direcciones IP a dispositivos dentro de una red, lo que permite que se identifiquen y comuniquen. ICMPv6 (Protocolo de Mensajes de Control de Internet para IPv6) facilita la configuración automática de direcciones en redes IPv6 y realiza tareas de diagnóstico y mantenimiento de red. Estos protocolos también indican al dispositivo la dirección de la puerta de enlace predeterminada, para que sepa hacia dónde enviar paquetes destinados a otras redes, y la dirección del servidor DNS, que permite la resolución de nombres de dominio (por ejemplo, www.example.com) a direcciones IP. Por ejemplo, cuando un usuario solicita una página web de un servidor, el dispositivo consulta el servidor DNS para obtener la dirección IP correspondiente al dominio solicitado.

### IP

El protocolo IP (Protocolo de Internet) se encarga de la entrega de los paquetes desde la fuente hasta el destino final a través de una red, similar al proceso de enviar una carta con una dirección específica. En este caso, el paquete de datos viaja desde el dispositivo del usuario hasta el servidor web que aloja el contenido solicitado. A su vez, el servidor web responde enviando los datos de la página web solicitada, también mediante paquetes IP.

### TCP

TCP (Protocolo de Control de Transmisión) es un protocolo que garantiza la fiabilidad en la transmisión de datos. Esto significa que asegura que toda la información que fue enviada desde la fuente sea recibida correctamente en el destino, en el orden correcto y sin pérdidas. En una transmisión como la descarga de una página web, TCP asegura que todos los fragmentos de información lleguen completos; si algún paquete IP no llega a su destino, TCP detecta la pérdida y vuelve a enviar el paquete hasta que la información esté completa. Esto es crucial para aplicaciones en tiempo real o sensibles a la pérdida de datos, como la carga de una página web o la transferencia de archivos.




### HTTP

HTTP (Protocolo de Transferencia de Hipertexto) es el protocolo de aplicación utilizado para la comunicación entre el navegador del usuario y el servidor web. Una vez que TCP establece una conexión confiable y se resuelve la dirección IP del servidor (gracias a DNS), HTTP permite solicitar y recibir archivos, como texto, imágenes y videos, que componen la página web. Cuando el usuario ingresa una URL en su navegador, se envía una solicitud HTTP al servidor para obtener los datos de esa página. El servidor responde con los datos correspondientes en un formato que el navegador puede interpretar y mostrar al usuario.

### 5.2.2 Internet y Estándares
Con la creciente cantidad de nuevos dispositivos y nuevas tecnologías en línea, ¿cómo es posible manejar todos los cambios y continuar brindando servicios de manera confiable, tales como el correo electrónico? La respuesta son los estándares de Internet.

Un estándar es un conjunto de reglas que determina cómo se realiza algo. Los estándares de red e Internet aseguran que todos los dispositivos que se conectan a la red implementen el mismo conjunto de reglas o protocolos del mismo modo. Usando estándares, es posible que diferentes tipos de dispositivos se envíen información entre sí a través de Internet. Por ejemplo, el modo en que los dispositivos formatean, envían y reciben un correo electrónico se realiza de una manera estandarizada. Si una persona envía un correo electrónico a través de una computadora personal, otra persona puede utilizar un teléfono celular para recibir y leer ese correo siempre que el teléfono utilice los mismo estándares.

### 5.2.3 Organizaciones de Estándares de Red
Un estándar de Internet es el resultado final de un ciclo completo de discusión, resolución de problemas y pruebas. Estos distintos estándares son desarrollados, publicados y mantenidos por diferentes organizaciones, tal como se indica en la figura. Cuando se propone un nuevo estándar, cada etapa del desarrollo y del proceso de aprobación es registrada en un documento numerado de solicitud de comentarios (RFC, Request for Comments) para seguir la evolución del estándar. Las RFC para los estándares de Internet son publicadas y administradas por el Grupo de Trabajo de Ingeniería de Internet (Internet Engineering Task Force - IETF).

En la figura se muestran otras organizaciones de estándares que mantienen Internet.

<div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.2.3.png" style="width:50rem"></a>
</div>

---
# 5.3 Modelos de Comunicación de Red

### 5.3.3 El Modelo TCP/IP

Los modelos en capas nos ayudan a ver cómo se integran los diversos protocolos para posibilitar las comunicaciones de red. Este modelo describe el funcionamiento de los protocolos que se produce en cada capa y la interacción con las capas que se encuentran por encima y por debajo de ellas. El modelo en capas presenta muchos beneficios: Ayuda en el diseño de protocolos, ya que los protocolos que operan en una capa específica tienen información definida según la cual actúan, y una interfaz definida para las capas superiores e inferiores. Fomenta la competencia, ya que los productos de distintos proveedores pueden trabajar en conjunto. Hace posible que se implementen cambios tecnológicos en un nivel sin afectar a los demás niveles. Proporciona un lenguaje común para describir las funciones y capacidades de networking. El primer modelo en capas para comunicaciones entre redes se creó a principios de la década de 1970 y se conoce con el nombre de modelo de internet. Define cuatro categorías de funciones que deben estar presentes para que las comunicaciones sean exitosas. El conjunto de protocolos TCP/IP que se utilizan para las comunicaciones por Internet sigue la estructura de este modelo, como se muestra en la tabla. Por esto, es común que al modelo de internet se le conozca como modelo TCP/IP.

| **Capa del modelo TCP/IP** | **Descripción** |
|----------------------------|-----------------|
| **Aplicación**             | Representa datos para el usuario, además del control de codificación y de diálogo. |
| **Transporte**             | Admite la comunicación entre distintos dispositivos a través de diversas redes. |
| **Internet**               | Determina el mejor camino a través de una red. |
| **Acceso a la red**        | Controla los dispositivos de hardware y los medios que forman la red. |

Tu texto está casi completo; solo hace falta ajustar algunas oraciones para mejorar la claridad y corregir algunos errores de ortografía. Aquí tienes una versión revisada:

---

**Ejemplo (enviar un mensaje):**  
Cuando un dispositivo crea un mensaje, utiliza protocolos de diferentes capas de la pila de protocolos.

**Capa de acceso a la red -> Protocolo Ethernet**  
El protocolo Ethernet se utiliza para la comunicación entre tarjetas de interfaz de red (NIC, por sus siglas en inglés) dentro de la misma red. Permite la transmisión de datos de una NIC a otra en una red local (LAN).

**Capa de Internet -> Protocolo IP**  
Puede ser la versión IPv4 o la versión IPv6. El protocolo IP organiza el envío de mensajes desde el origen hasta el destino final, ya sea dentro de la misma red o a través de múltiples redes interconectadas.

**Capa de transporte -> Protocolo TCP**  
El Protocolo de Control de Transmisión (TCP) garantiza la transmisión confiable de datos, asegurando que el mensaje llegue completo y en el orden correcto al destino.

**Capa de aplicación -> Protocolo HTTP**  
El protocolo HTTP rige el intercambio o la transferencia de archivos HTML, permitiendo que el contenido web se transmita entre el cliente (como un navegador) y el servidor.

En conclusión, enviar un mensaje requiere el uso de varios protocolos que funcionan en diferentes capas de la pila de protocolos.

<div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\pilaProtocolos.png" style="width:50rem"></a>
</div>

---

### 5.3.4 El Modelo de Referencia OSI

Hay dos tipos básicos de modelos para describir las funciones que deben estar presentes para que las comunicaciones de red sean exitosas: modelos de protocolo y modelos de referencia. 

- **Modelo de Protocolo** - Este modelo coincide estrechamente con la estructura de un conjunto de protocolos en particular. Una suite de protocolos incluye el conjunto de protocolos relacionados que generalmente proporcionan toda la funcionalidad requerida para que las personas se comuniquen con la red de datos. El modelo TCP/IP es un modelo de protocolos porque describe las funciones que ocurren en cada capa de protocolos dentro de una suite de TCP/IP. 

- **Modelo de Referencia** - Este tipo de modelo describe las funciones que se deben completar en una capa en particular, pero no especifica exactamente cómo se debe realizar una función. Un modelo de referencia no pretende ofrecer un nivel de detalle suficiente para definir en forma precisa la manera en la que cada protocolo debería funcionar en cada capa. El objetivo principal de un modelo de referencia es ayudar a comprender mejor las funciones y los procesos necesarios para las comunicaciones de red. 


El modelo de referencia de redes más conocido fue creado por el proyecto Interconexión de Sistemas Abiertos (Open Systems Interconnection -OSI) en la Organización Internacional de Estandarización (ISO). Se usa para diseño de redes de datos, especificaciones de funcionamiento y resolución de problemas. Este modelo se conoce comúnmente como el modelo OSI.


| **Capa del modelo OSI**     | **Descripción** |
|-----------------------------|-----------------|
| **7 - Aplicación**          | La capa de aplicación contiene protocolos utilizados para comunicaciones proceso a proceso. |
| **6 - Presentación**        | Proporciona una representación común de los datos transferidos entre los servicios de la capa de aplicación. |
| **5 - Sesión**              | Proporciona servicios a la capa de presentación para organizar su diálogo y administrar el intercambio de datos. |
| **4 - Transporte**          | Define los servicios para segmentar, transferir y reensamblar los datos para las comunicaciones individuales entre terminales. |
| **3 - Red**                 | Proporciona servicios para intercambiar los datos individuales en la red entre terminales identificados. |
| **2 - Enlace de Datos**     | Describe los métodos para intercambiar tramas de datos entre dispositivos en un medio común. |
| **1 - Física**              | Describe los medios mecánicos, eléctricos, funcionales y de procedimiento para activar, mantener y desactivar conexiones físicas para la transmisión de bits hacia y desde un dispositivo de red. |

Una **trama** es una unidad de datos en la capa de enlace de datos del modelo OSI. Es el conjunto de bits que un dispositivo de red, como una tarjeta de interfaz de red (NIC), envía a través de una red local. La trama incluye no solo los datos que se están enviando, sino también información adicional que permite la transmisión y la recepción adecuada de esos datos. Esta información adicional incluye la dirección del remitente, la dirección del destinatario, y un campo de verificación para asegurar que los datos no hayan sido dañados durante el tránsito.

### Ejemplo sencillo:

Imagina que tienes un mensaje que quieres enviar a un amigo a través de un sistema de mensajería. En lugar de simplemente escribir el mensaje, también incluyes un sobre con la dirección de tu amigo, tu propia dirección, y sellos de seguridad para asegurarte de que el mensaje llegue correctamente.

En términos de redes:
- **El mensaje** es la **carga útil o datos** (la información que realmente deseas enviar).
- **El sobre con las direcciones** es la **trama**. Este sobre incluye:
  - La dirección del remitente (tu dirección) y la del destinatario (tu amigo), que indican quién envía y quién recibe.
  - Un campo de verificación (similar a un sello de seguridad) que garantiza que el mensaje no esté dañado.

Cuando el mensaje llega a tu amigo, la "trama" se abre, y él puede leer el mensaje contenido en su interior.

### En la red:
Una trama Ethernet, por ejemplo, contiene:
1. **Encabezado de la trama**: con la dirección MAC de origen y destino.
2. **Datos**: el mensaje o la carga útil que se está enviando.
3. **Campo de verificación**: que permite al receptor comprobar que los datos llegaron sin errores.

En resumen, una trama es como un sobre que encapsula y protege los datos para que puedan ser enviados a través de la red de forma segura y eficiente.


---
### 5.3.5 Comparación del Modelo OSI y el Modelo TCP/IP
Debido a que TCP/IP es el conjunto de protocolos en uso para las comunicaciones por Internet, ¿por qué también necesitamos aprender el modelo OSI?

El modelo TCP/IP es un método para visualizar las interacciones de los diversos protocolos que conforman el conjunto de protocolos TCP/IP. No describe las funciones generales necesarias para todas las comunicaciones de red. Describe las funciones de red específicas de los protocolos en uso en el conjunto de protocolos TCP/IP. Por ejemplo, en la capa de acceso a la red, la suite de protocolos TCP/IP no especifica los protocolos que se deben utilizar para transmitir a través de un medio físico, ni el método de codificación de las señales para la transmisión. Las capas 1 y 2 de OSI tratan los procedimientos necesarios para acceder a los medios y las maneras físicas de enviar datos por la red.

Los protocolos que forman la suite de protocolos TCP/IP pueden describirse en términos del modelo de referencia OSI. Las funciones que se producen en la capa de Internet del modelo TCP/IP se incluyen en la capa de red del modelo OSI, tal como se indica en la figura. La funcionalidad de la capa de transporte es la misma en ambos modelos. Sin embargo, la capa de acceso a la red y la capa de aplicaciones del modelo TCP/IP se dividen a su vez en el modelo OSI para describir funciones discretas que deben realizarse en estas capas.



<div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.3.5.png" style="width:50rem"></a>
</div>



Las similitudes clave se encuentran en la capa de transporte y en la capa de red. Sin embargo, los dos modelos se diferencian en el modo en que se relacionan con las capas que están por encima y por debajo de cada capa.

- La capa 3 de OSI, la capa de red, asigna directamente a la capa de Internet TCP/IP. Esta capa se utiliza para describir protocolos que abordan y dirigen mensajes a través de una internetwork.

- La capa 4 de OSI, la capa de transporte, asigna directamente a la capa de transporte TCP/IP. Esta capa describe los servicios y las funciones generales que proporcionan la entrega ordenada y confiable de datos entre los hosts de origen y de destino.

- La capa de aplicación TCP/IP incluye un número de protocolos que proporciona funcionalidad específica a una variedad de aplicaciones de usuario final. Las capas 5, 6 y 7 del modelo OSI se utilizan como referencias para proveedores y desarrolladores de software de aplicación para fabricar productos que funcionan en redes.

- Tanto el modelo TCP/IP como el modelo OSI se utilizan comúnmente en la referencia a protocolos en varias capas. Dado que el modelo OSI separa la capa de enlace de datos de la capa física, se suele utilizan cuando se refiere a esas capas inferiores.




### 5.3.6 Verifique su Comprensión - Modelos de Comunicación de Red

Compruebe su comprensión de los modelos de comunicación de red eligiendo la respuesta correcta a las siguientes preguntas.


---
### Pregunta 1
¿Cuál protocolo es responsable de garantizar la entrega fiable de la información?

R\ TCP

---
### Pregunta 2
¿Qué protocolo utilizan los enrutadores para reenviar mensajes?

R\ IP

---
### Pregunta 3
¿Cuales dos capas del modelo OSI se asignan directamente como la única capa de acceso a la red en el modelo TCP/IP? Elija dos opciones.

R\ Enlace de datos,fisica

---
### Pregunta 4
¿En qué capa del modelo OSI ocurre el direccionamiento IP?

R\ Red

---

# 5.4 Resumen de Principios de Comunicación

### 5.4.1 ¿Qué Aprendí en este Módulo?

<details>
        <summary>Protocolo de comunicacion</summary>
        Los protocolos son necesarios para que las computadoras se comuniquen correctamente a través de la red. Estos incluyen el formato del mensaje, el tamaño del mensaje, el tiempo, la codificación, la encapsulación y los patrones del mensaje.<br><br>
        - Formato del mensaje - Cuando se envía un mensaje, debe usar un formato o estructura específica.<br><br>
        - Tamaño del mensaje - Las reglas que rigen el tamaño de las piezas comunicadas a través de la red son muy estrictas. También pueden ser diferentes, de acuerdo con el canal utilizado.<br><br>
        - Sincronización - La sincronización determina la velocidad a la que se transmiten los bits a través de la red. También afecta cuándo un host individual puede enviar datos y la cantidad total de datos que se pueden enviar en una transmisión dada.<br><br>
        - Codificación - El host de envío convierte primero los mensajes enviados a través de la red en bits. Cada bit se codifica en un patrón de sonidos, ondas de luz o impulsos electrónicos, según el medio de red a través del cual se transmitan los bits.<br><br>
        - Encapsulación - Cada mensaje transmitido en una red debe incluir un encabezado que contenga información de direccionamiento que identifique los hosts de origen y destino. La encapsulación es el proceso de agregar esta información a los elementos de datos que conforman el mensaje.<br><br>
        - Patrón de mensaje - Algunos mensajes requieren una confirmación antes de que se pueda enviar el siguiente mensaje. Este tipo de patrón de solicitud y respuesta es un aspecto común de muchos protocolos de red. Sin embargo, hay otros tipos de mensajes que pueden simplemente transmitirse a través de la red, sin preocuparse de si llegan a su destino.

</details>  
<br>

<details>
        <summary>Estandares de comunicacion</summary>
        Las topologías nos permiten ver la red mediante la representación de dispositivos finales y dispositivos intermediarios. ¿Cómo ve una red un dispositivo? Piense en un dispositivo en una burbuja. Lo único que ve un dispositivo es su propia información de direccionamiento. ¿Cómo sabe el dispositivo que está en la misma red que otro dispositivo? La respuesta son los protocolos de red. La mayoría de las comunicaciones de red se divide en unidades de datos o paquetes más pequeños. <br><br>
        Un estándar es un conjunto de reglas que determina cómo se realiza algo. Los estándares de red e Internet aseguran que todos los dispositivos que se conectan a la red implementen el mismo conjunto de reglas o protocolos del mismo modo. Usando estándares, es posible que diferentes tipos de dispositivos se envíen información entre sí a través de Internet.<br><br>
        Un estándar de Internet es el resultado final de un ciclo completo de discusión, resolución de problemas y pruebas. Estos diferentes estándares son desarrollados, publicados y mantenidos por una variedad de organizaciones. Cuando se propone un nuevo estándar, cada etapa del desarrollo y del proceso de aprobación es registrada en un documento numerado de Solicitud de Comentarios (RFC, Request for Comments) para seguir la evolución del estándar. Las RFC para los estándares de Internet son publicadas y administradas por el Grupo de Trabajo de Ingeniería de Internet (IETF).

</details>  
<br>

<details>
        <summary>Modelos de comunicacion de red</summary>
        Los protocolos son reglas que rigen las comunicaciones. La comunicación correcta entre hosts requiere la interacción entre una serie de protocolos. Los protocolos incluyen HTTP, TCP, IP y Ethernet. Estos protocolos se implementan en el software y el hardware que están instalados en cada host y dispositivo de red.<br><br>
        La interacción entre los diferentes protocolos en un dispositivo se puede ilustrar como una pila de protocolos. En una pila se ilustran los protocolos como una jerarquía en capas, donde cada protocolo de nivel superior depende de los servicios de los protocolos que aparecen en los niveles inferiores. La separación de funciones permite que cada capa de la pila funcione independientemente de las otras capas.<br><br>El conjunto de protocolos TCP/IP que se utilizan para las comunicaciones por Internet sigue la estructura de este modelo.<br><br>
        - Aplicación - Representa datos para el usuario, además de codificación y control de diálogo<br><br>
        - Transporte - Admite la comunicación entre varios dispositivos a través de diversas redes.<br><br>
        - Internet - Determina la mejor ruta a través de la red<br><br>
        - Acceso a la red - Los dispositivos de hardware y los medios que componen la red.<br><br>
        Un modelo de referencia describe las funciones que se deben completar en una capa en particular, pero no especifica exactamente cómo se debe lograr una función. El objetivo principal de un modelo de referencia es ayudar a comprender mejor las funciones y los procesos necesarios para las comunicaciones de red.<br><br>El modelo de referencia entre redes más conocido fue creado por el proyecto OSI en la ISO internacional. Se usa para diseño de redes de datos, especificaciones de funcionamiento y resolución de problemas. Este modelo se conoce comúnmente como el modelo OSI.

</details>  
<br>

<details>
        <summary>Descripcion de la capa del modelo OSI</summary>
        7 – Aplicación - La capa de aplicación contiene protocolos que se utilizan para las comunicaciones de proceso a proceso.<br><br>
        6 – Presentación - La capa de presentación proporciona una representación común de los datos transferidos entre los servicios de la capa de aplicación.<br><br>
        5 – Sesión - La capa de sesión proporciona servicios a la capa de presentación para organizar su diálogo y gestionar el intercambio de datos.<br><br>
        4 – Transporte - La capa de transporte define los servicios para segmentar, transferir y volver a ensamblar los datos para las comunicaciones individuales entre los dispositivos finales.<br><br>
        3 – Red - La capa de red proporciona servicios para intercambiar datos individuales a través de la red entre dispositivos finales identificados.<br><br>
        2 – Enlace de datos - Los protocolos de la capa de enlace de datos describen métodos para intercambiar tramas de datos entre dispositivos a través de un medio común.<br><br>
        1 – Físico - Los protocolos de la capa física describen los medios mecánicos, eléctricos, funcionales y de procedimiento para activar, mantener y desactivar conexiones físicas para la transmisión de bits hacia y desde un dispositivo de red.
</details>  
<br>

# Cuestionario de Principios de Comunicación

### Pregunta 1
¿Cuál es el objetivo de la capa física de OSI?

R/ Transmitir bits por los medios locales

La capa física se encarga de transmitir las señales reales por los medios físicos en forma de bits. El intercambio de tramas, el control del acceso a los medios y la detección de errores son funciones de la capa de enlace de datos.

---
### Pregunta 2
¿Qué afirmación es correcta sobre los protocolos de red?

R/ Definen cómo se intercambian los mensajes entre el origen y el destino.

Los protocolos de red se implementan en hardware, software o ambos. Interactúan entre sí dentro de diferentes capas de una pila de protocolos. Los protocolos no tienen nada que ver con la instalación de los equipos de red. Se requieren protocolos de red para intercambiar información entre los dispositivos de origen y de destino en redes locales y remotas.

---
### Pregunta 3
¿Cuáles son los tres acrónimos o siglas que representan organismos de estandarización? (Elija tres opciones).

R/ IANA, IEEE , IETF

TCP/IP es una pila de protocolos que contiene muchos otros protocolos, como HTTP, FTP y DNS. Se requiere el uso de la pila de protocolos TCP/IP cuando se comunica en Internet. Una dirección MAC es una dirección grabada en una tarjeta de red Ethernet. OSI es el modelo de siete capas que se usa para explicar la forma en que funcionan las redes.

---
### Pregunta 4
¿Qué término de red describe un conjunto particular de reglas en una capa que rigen la comunicación en esa capa?

R/ Protocolo

Un protocolo determina cómo se formatea un mensaje y establece las reglas para partes específicas del proceso de comunicación.

---
### Pregunta 5
¿Qué capa del modelo OSI define los servicios para segmentar y rearmar los datos de comunicaciones individuales entre terminales?

R/ transporte

El modelo OSI consta de siete capas: aplicación, presentación, sesión, transporte, red, enlace de datos y física. La capa de transporte define los servicios para segmentar, transferir y rearmar los datos para las comunicaciones individuales entre terminales.

---
### Pregunta 6
¿Cuál es el propósito de los protocolos en las comunicaciones de datos?

R/ Proporcionar las reglas requeridas para que se produzca un tipo específico de comunicación.

Los protocolos proporcionan las reglas que definen cómo se transmite un mensaje a través de una red. Los requisitos de implementación, como los detalles electrónicos y de ancho de banda para la comunicación de datos, se especifican en estándares. Los sistemas operativos no están especificados por protocolos, pero implementan protocolos. Los protocolos determinan cómo y cuándo se envía un mensaje, pero no controlan su contenido.

---
### Pregunta 7
¿Qué término se refiere al conjunto de reglas que define cómo funciona una red?

R/ Estándar

Los estándares garantizan que diferentes dispositivos que se conectan a la red puedan comunicarse entre sí. En el ámbito de las redes existen muchos estándares que definen cómo debería funcionar una red y garantizan que se implementen los mismos protocolos en todos los componentes.

---
### Pregunta 8
¿Cuáles son las tres capas del modelo OSI que conforman la capa de aplicación del modelo TCP/IP? (Elija tres opciones).

R/ Sesión, Presentación, APlicacion

Las tres capas superiores del modelo OSI (sesión, presentación y aplicación) equivalen a la única capa de aplicación del modelo TCP/IP.

---
### Pregunta 9
¿Qué organización emite y administra los documentos de Petición de comentarios (Request for Comments, RFC)?

R/ IETF

La organización Internet Engineering Task Force (IETF) emite y administra la Petición de comentarios (RFC).

---
### Pregunta 10
¿Cuáles son las dos capas del modelo OSI que tienen la misma funcionalidad que las dos capas del modelo TCP/IP?(Escoge dos.)

R/ Enlace de datos, Física

En conjunto, las capas física y de enlace de datos OSI son equivalentes a la capa de acceso a la red TCP/IP. La funcionalidad de capa de transporte OSI es equivalente a la de la capa de transporte TCP/IP, y la de la capa de red OSI es equivalente a la de la capa de Internet TCP/IP. Las capas de aplicación, presentación y sesión del modelo OSI se alinean con la capa de aplicación del modelo TCP/IP.

---

[↶Regresar](../README.md)

