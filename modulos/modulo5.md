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

---

### 5.3.4 El Modelo de Referencia OSI

Hay dos tipos básicos de modelos para describir las funciones que deben estar presentes para que las comunicaciones de red sean exitosas: modelos de protocolo y modelos de referencia. Modelo de Protocolo - Este modelo coincide estrechamente con la estructura de un conjunto de protocolos en particular. Una suite de protocolos incluye el conjunto de protocolos relacionados que generalmente proporcionan toda la funcionalidad requerida para que las personas se comuniquen con la red de datos. El modelo TCP/IP es un modelo de protocolos porque describe las funciones que ocurren en cada capa de protocolos dentro de una suite de TCP/IP. Modelo de Referencia - Este tipo de modelo describe las funciones que se deben completar en una capa en particular, pero no especifica exactamente cómo se debe realizar una función. Un modelo de referencia no pretende ofrecer un nivel de detalle suficiente para definir en forma precisa la manera en la que cada protocolo debería funcionar en cada capa. El objetivo principal de un modelo de referencia es ayudar a comprender mejor las funciones y los procesos necesarios para las comunicaciones de red. El modelo de referencia de redes más conocido fue creado por el proyecto Interconexión de Sistemas Abiertos (Open Systems Interconnection -OSI) en la Organización Internacional de Estandarización (ISO). Se usa para diseño de redes de datos, especificaciones de funcionamiento y resolución de problemas. Este modelo se conoce comúnmente como el modelo OSI.


| **Capa del modelo OSI**     | **Descripción** |
|-----------------------------|-----------------|
| **7 - Aplicación**          | La capa de aplicación contiene protocolos utilizados para comunicaciones proceso a proceso. |
| **6 - Presentación**        | Proporciona una representación común de los datos transferidos entre los servicios de la capa de aplicación. |
| **5 - Sesión**              | Proporciona servicios a la capa de presentación para organizar su diálogo y administrar el intercambio de datos. |
| **4 - Transporte**          | Define los servicios para segmentar, transferir y reensamblar los datos para las comunicaciones individuales entre terminales. |
| **3 - Red**                 | Proporciona servicios para intercambiar los datos individuales en la red entre terminales identificados. |
| **2 - Enlace de Datos**     | Describe los métodos para intercambiar tramas de datos entre dispositivos en un medio común. |
| **1 - Física**              | Describe los medios mecánicos, eléctricos, funcionales y de procedimiento para activar, mantener y desactivar conexiones físicas para la transmisión de bits hacia y desde un dispositivo de red. |

---
### 5.3.5 Comparación del Modelo OSI y el Modelo TCP/IP
Debido a que TCP/IP es el conjunto de protocolos en uso para las comunicaciones por Internet, ¿por qué también necesitamos aprender el modelo OSI?

El modelo TCP/IP es un método para visualizar las interacciones de los diversos protocolos que conforman el conjunto de protocolos TCP/IP. No describe las funciones generales necesarias para todas las comunicaciones de red. Describe las funciones de red específicas de los protocolos en uso en el conjunto de protocolos TCP/IP. Por ejemplo, en la capa de acceso a la red, la suite de protocolos TCP/IP no especifica los protocolos que se deben utilizar para transmitir a través de un medio físico, ni el método de codificación de las señales para la transmisión. Las capas 1 y 2 de OSI tratan los procedimientos necesarios para acceder a los medios y las maneras físicas de enviar datos por la red.

Los protocolos que forman la suite de protocolos TCP/IP pueden describirse en términos del modelo de referencia OSI. Las funciones que se producen en la capa de Internet del modelo TCP/IP se incluyen en la capa de red del modelo OSI, tal como se indica en la figura. La funcionalidad de la capa de transporte es la misma en ambos modelos. Sin embargo, la capa de acceso a la red y la capa de aplicaciones del modelo TCP/IP se dividen a su vez en el modelo OSI para describir funciones discretas que deben realizarse en estas capas.



<div align="center">
                <a href="" target="_blank"><img src="recursos\modulo5\5.3.5.png" style="width:50rem"></a>
</div>



Las similitudes clave se encuentran en la capa de transporte y en la capa de red. Sin embargo, los dos modelos se diferencian en el modo en que se relacionan con las capas que están por encima y por debajo de cada capa.

La capa 3 de OSI, la capa de red, asigna directamente a la capa de Internet TCP/IP. Esta capa se utiliza para describir protocolos que abordan y dirigen mensajes a través de una internetwork.
La capa 4 de OSI, la capa de transporte, asigna directamente a la capa de transporte TCP/IP. Esta capa describe los servicios y las funciones generales que proporcionan la entrega ordenada y confiable de datos entre los hosts de origen y de destino.
La capa de aplicación TCP/IP incluye un número de protocolos que proporciona funcionalidad específica a una variedad de aplicaciones de usuario final. Las capas 5, 6 y 7 del modelo OSI se utilizan como referencias para proveedores y desarrolladores de software de aplicación para fabricar productos que funcionan en redes.
Tanto el modelo TCP/IP como el modelo OSI se utilizan comúnmente en la referencia a protocolos en varias capas. Dado que el modelo OSI separa la capa de enlace de datos de la capa física, se suele utilizan cuando se refiere a esas capas inferiores.