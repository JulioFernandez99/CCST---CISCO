
# ¿Qué Voy a Aprender en este Módulo?

**Título del Módulo:** Capa de Acceso 

**Objetivo del Módulo:** Explicar cómo se produce la comunicación en las redes Ethernet.


### 7.1 Encapsulación y la Trama de Ethernet


**Ethernet Frame**

La trama Ethernet permite la comunicación entre interfaces de red dentro de la misma red local. A continuación se describen los campos principales de una trama Ethernet:

1. **Preambulo (7 bytes)**  
   El preámbulo consiste en una serie de bits que sincroniza la tarjeta de interfaz de red (NIC) de recepción con los bits de la transmisión en curso. Esto asegura que ambas interfaces de red estén sincronizadas antes de iniciar la recepción de los datos reales.

2. **Delimitador de Inicio de Trama (SFD) (1 byte)**  
   El delimitador de inicio de trama (Start Frame Delimiter, SFD) indica a la tarjeta de interfaz de red receptora que, a partir de este punto, comenzará la transmisión de la información relevante de la trama Ethernet.

3. **Dirección MAC de Destino (6 bytes)**  
   Esta es la dirección MAC de la tarjeta NIC en la red de destino, a la cual está dirigida la trama Ethernet. Las direcciones MAC permiten identificar de forma única cada dispositivo en la red local.

4. **Dirección MAC de Origen (6 bytes)**  
   Indica la dirección MAC del dispositivo que originó la trama Ethernet, es decir, la tarjeta de interfaz de red de la cual proviene la transmisión.

5. **Longitud o Tipo de Campo (2 bytes)**  
   Este campo puede tener dos significados dependiendo del valor contenido:
   - **Longitud**: Cuando el valor es menor a 1536, se interpreta como la longitud de la carga útil en bytes.
   - **Tipo**: Si el valor es igual o mayor a 1536, indica el tipo de protocolo de red contenido (por ejemplo, IPv4 o IPv6), especificando el tipo de datos transportados en la trama.

6. **Datos o Carga Útil (46-1500 bytes)**  
   Este campo contiene los datos reales de la trama, que podrían ser un paquete de red como IPv4, IPv6 u otros protocolos encapsulados. Los datos pueden incluir cabeceras adicionales como las de TCP o HTTP. Ethernet solo se encarga de transferir estos datos de una tarjeta de interfaz de red a otra dentro de la misma red local.

7. **Secuencia de Verificación de Trama (FCS) (4 bytes)**  
   El campo FCS (Frame Check Sequence) realiza una verificación de errores en el dispositivo receptor para asegurar la integridad de los datos. Mediante un cálculo de redundancia cíclica (CRC), se verifica que los datos no hayan sido alterados durante la transmisión.

**Conclusión**

La estructura de la trama Ethernet está diseñada para facilitar la transmisión confiable de datos entre dispositivos dentro de una misma red local. Cada campo cumple una función específica, desde la sincronización inicial y la identificación de dispositivos, hasta la transferencia de la carga útil y la verificación de errores. Esto permite que la tecnología Ethernet sea una de las más confiables y ampliamente utilizadas para la comunicación en redes locales.


### 7.1.2 Encapsulación
Cuando envía una carta, la persona que la escribe utiliza un formato aceptado para asegurarse de que la carta se entregue y de que el destinatario la comprenda. De la misma manera, un mensaje que se envía a través de una red de computadoras sigue reglas de formato específicas para que pueda ser entregado y procesado.

El proceso que consiste en colocar un formato de mensaje (la carta) dentro de otro formato de mensaje (el sobre) se denomina encapsulamiento. Cuando el destinatario revierte este proceso y quita la carta del sobre se produce el desencapsulamiento del mensaje. De la misma manera en la que una carta se encapsula en un sobre para la entrega, los mensajes de las computadoras también deben encapsularse.

Cada mensaje de computadora se encapsula en un formato específico, llamado trama, antes de enviarse a través de la red. Una trama actúa como un sobre: proporciona la dirección del destino y la dirección del host de origen. El formato y el contenido de una trama están determinados por el tipo de mensaje que se envía y el canal que se utiliza para enviarlo. Los mensajes que no tienen el formato correcto no se pueden enviar al host de destino o no pueden ser procesados por éste.

<details>
        <summary>Red </summary>
Semejante a enviar una carta, un mensaje que se envía a través de una red de computadoras sigue reglas de formato específicas para que pueda ser entregado y procesado.
<br><br>
Al igual que el envío de una carta, un mensaje que se envía a través de una red informática sigue reglas de formato específicas para su entrega y procesamiento.
<br><br>
El Protocolo de Internet (IP) es un protocolo con una función similar a la del ejemplo sobre. En la figura, los campos del paquete de Protocolo de Internet versión 6 (IPv6) identifican el origen del paquete y su destino. IP es responsable de enviar un mensaje desde el origen del mensaje al destino a través de una o más redes.
<br><br>
Nota: Los campos del paquete IPv6 se analizan en detalle en otro módulo.

<div align="center">
                <a href="" target="_blank"><img src="recursos\modulo7\red.png" style="width:50rem"></a>
</div>
</details>  
<br>

---

### 7.2 La Capa de Acceso


---

[↶Regresar](../README.md)



