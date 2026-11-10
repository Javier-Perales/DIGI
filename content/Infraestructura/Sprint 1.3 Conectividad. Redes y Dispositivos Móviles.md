---
title: Sprint 1.3 Conectividad. Redes y Dispositivos Móviles
sda: Misión 1. Infraestructura
tags:
criterios_evaluacion:
entregable:
---
> [!abstract] Reto
> En este sprint aprenderemos cómo funcionan las redes informáticas y las principales tecnologías de conectividad, tanto por cable como inalámbricas (Ethernet, Wi-Fi, 4G/5G, Bluetooth y NFC). También descubriremos cómo se identifican los dispositivos mediante direcciones IP, cómo configurar conexiones y cómo diagnosticar problemas habituales.
>
>Nuestro reto será diseñar una **solución de conectividad eficiente y segura para el negocio de nuestro cliente**, aplicando los conocimientos adquiridos a situaciones reales.

# 1. Fundamentos de la conectividad

>[!example] Anatomía de la conectividad cableada
>Inspecciona el ordenador de clase y resuelve las siguientes cuestiones:
>- ¿Qué cable sale de la parte trasera del ordenador para daros Internet?
>- ¿Cómo es el conector que tiene en los extremos?
>- ¿A dónde va a parar en la pared?

La **conectividad** es la capacidad que tienen los dispositivos electrónicos para establecer conexiones e intercambiar información con otros dispositivos o redes.

![[recursos/conectividad.png]]

Podemos distinguir dos formas principales de conexión:

- **Conexiones cableadas**: utilizan un medio físico, como un cable Ethernet, para transmitir información. Suelen proporcionar una conexión estable.
- **Conexiones inalámbrica**s: transmiten información mediante ondas electromagnéticas, sin necesidad de un cable entre los dispositivos. Por ejemplo, Wi-Fi y Bluetooth.

## 1.1 ¿Qué es una red informática?

Una **red informática** es un conjunto de dispositivos interconectados que pueden comunicarse entre sí y compartir información o recursos.

En una pequeña empresa, una red permite:

- Compartir una impresora entre varios ordenadores.
- Acceder a documentos almacenados en otro equipo o servidor.
- Utilizar una misma conexión a Internet.
- Conectar teléfonos móviles, tabletas y otros dispositivos.
- Acceder a servicios internos del negocio.

![[recursos/red_informática.png]]

### 1.1.1 Tipos de redes según su extensión

|Tipo|Significado|Características y ejemplo|
|---|---|---|
|LAN|Local Area Network|Red local de una oficina, vivienda o instituto.|
|WLAN|Wireless Local Area Network|Red local inalámbrica, normalmente mediante Wi-Fi.|
|WAN|Wide Area Network|Red extensa que conecta redes situadas en diferentes ubicaciones geográficas.|

**¿Y qué es Internet?**

Internet es una red mundial formada por numerosas redes interconectadas. Permite acceder a servicios como páginas web, correo electrónico, almacenamiento en la nube y aplicaciones de mensajería.

Una LAN puede funcionar perfectamente sin Internet.

# 2. Elementos de una red informática

Para conectar los dispositivos de una empresa necesitamos conocer qué función desempeña cada componente.

- **Tarjeta de red (NIC)**. Es el componente que permite que un dispositivo se conecte a una red. Puede ser Ethernet o Wi-Fi. Los ordenadores suelen incorporar una o varias interfaces de red.
![[recursos/nic.png|300]]

- **Switch o conmutador**. Permite conectar varios dispositivos mediante cables Ethernet dentro de una red local. Por ejemplo, los ordenadores y la impresora de la empresa.
![[recursos/switch.png|350]]

- **Router o enrutador.** Permite comunicar redes diferentes. En una oficina, suele conectar la red local con Internet. Muchos routers domésticos incorporan también funciones de switch y Wi-Fi.
![[recursos/router.png|350]]

- **Punto de acceso inalámbrico (AP)**. Permite conectar dispositivos mediante Wi-Fi a una red local. Es especialmente útil para teléfonos móviles, tabletas y portátiles.
![[recursos/punto_acceso.png|350]]

- **Cable Ethernet**. Es uno de los medios físicos más utilizados en redes locales. Los cables de pares trenzados, como Cat 5e y Cat 6, suelen utilizar conectores conocidos como RJ45.

![[recursos/cable rj45.png|300]]
## 2.1 Diferencia entre switch y router

Aunque ambos conectan dispositivos, tienen funciones distintas.

| Switch                                                 | Router                                              |
| ------------------------------------------------------ | --------------------------------------------------- |
| Conecta dispositivos dentro de una red local Ethernet. | Interconecta redes.                                 |
| Utiliza principalmente direcciones MAC.                | Utiliza direcciones IP para encaminar paquetes.     |
| Permite conectar los PC e impresoras de una oficina.   | Permite conectar la red de la oficina con Internet. |
 
## 2.2 ¿Cómo se conectan los dispositivos de nuestro negocio?

Imaginemos que nuestro cliente dispone de los siguientes equipos:

| Dispositivo                 | Tecnología recomendada | Motivo                                  |
| --------------------------- | ---------------------- | --------------------------------------- |
| Ordenador de administración | Ethernet               | Conexión estable para el puesto fijo    |
| Ordenador de caja           | Ethernet               | Conexión estable para las operaciones   |
| Impresora de red            | Ethernet               | Compartirla entre varios empleados      |
| Portátil del gerente        | Wi-Fi                  | Permite desplazarse por el negocio      |
| Teléfono móvil              | Wi-Fi / 4G / 5G        | Acceso inalámbrico y conectividad móvil |
| Auriculares inalámbricos    | Bluetooth              | Comunicación de corto alcance           |

![[recursos/esquema_red.png]]

>[!question] Diseña la conectividad de tu negocio
>Identifica los dispositivos que necesitan conectividad y representar gráficamente cómo se conectarían dentro de la empresa asignada.
>
>**Fase 1. Recupera el briefing del cliente**. Completa una tabla similar a esta:
>
> |Dispositivo|Cantidad|Tipo de conexión|
> |---|---|---|
> |Ordenadores de escritorio|2|Ethernet|
> |Impresora de red|1|Ethernet|
> |Portátil|1|Wi-Fi|
> |Smartphones|2|Wi-Fi / 4G/5G|
> 
>Adapta la tabla a las necesidades de tu cliente.
>
>**Fase 2. Diseña el esquema de conectividad**
>
>Utiliza una herramienta de diagramas, como [diagrams.net](https://app.diagrams.net/?utm_source=chatgpt.com), para representar cómo conectarías todos los dispositivos.
>
>Tu esquema debe incluir:
>- Conexión a Internet y router.
>- Switch, si necesitas conectar varios dispositivos por Ethernet.
>- Ordenadores e impresora.
>- Punto de acceso Wi-Fi, integrado en el router o independiente.
>- Dispositivos móviles y portátiles.
>
> **Entrega**
>Guarda el esquema en PDF con el nombre `P1_Esquema_Conectividad.docx` en la carpeta `03_Redes` de DigiLab Solutions.

## 2.3 Direcciones MAC

Hasta ahora hemos visto que un **switch** permite conectar los ordenadores, impresoras y otros equipos de una red local Ethernet. Pero ¿cómo sabe el switch por qué puerto debe enviar la información para que llegue al destinatario correcto?

Para responder, necesitamos conocer las **direcciones MAC**.

Una **dirección MAC** (_Media Access Control_) es un identificador que utiliza una interfaz de red para comunicarse dentro de una red local, como Ethernet o Wi-Fi. En una comunicación Ethernet, las tramas incluyen una **MAC de origen** y una **MAC de destino**.

Por tanto, **cada interfaz que envía y recibe tramas Ethernet como equipo de origen o destino necesita utilizar una dirección MAC**. Un ordenador con tarjeta Ethernet y Wi-Fi puede tener **dos direcciones MAC distintas**, una por cada interfaz.

> [!info] ¿Cómo es una MAC?  
> Las direcciones MAC habituales de Ethernet están formadas por **48 bits = 6 bytes**, representados mediante **12 dígitos hexadecimales** (del `0` al `9` y de la `A` a la `F`).
> 
> Por ejemplo: `0C:1A:2B:3C:4D:5E`
> 
> `0C` · `1A` · `2B` · `3C` · `4D` · `5E` → **6 grupos de 2 dígitos hexadecimales**.

**¿Por qué se dice que las MAC son únicas?** Las direcciones MAC **asignadas universalmente por los fabricantes** se administran para que sean únicas a escala mundial. Tradicionalmente, una parte identifica a la organización fabricante y otra parte se asigna a la interfaz concreta. **Sin embargo, esta unicidad no es una garantía absoluta**: una dirección MAC puede modificarse por software, ser administrada localmente o generarse aleatoriamente, como ocurre en algunos móviles para proteger la privacidad.

> [!tip] No confundas MAC con IP
> 
> - **MAC:** identifica una interfaz en las comunicaciones de una red local Ethernet o Wi-Fi. El switch Ethernet utiliza las MAC para decidir por qué puerto enviar las tramas.
> - **IP:** es una dirección lógica que permite identificar y localizar interfaces y enviar paquetes entre redes. Los routers utilizan direcciones IP para encaminar esos paquetes.
> 
> Un mismo ordenador puede tener, al mismo tiempo, una dirección MAC y una dirección IP.

>[!question] Consulta la dirección MAC de tu equipo
> Abre el terminal y ejecuta `ip link`
> 1. ¿Cuál es tu dirección MAC? 
> 2. ¿Cuántos bytes y cuántos bits representan?
> 3. ¿Qué diferencia hay entre una dirección MAC y una dirección IP?
> 4. Si un ordenador tiene conexión Ethernet y Wi-Fi, ¿puede tener más de una MAC?
> 5. ¿Por qué necesita un switch consultar las MAC de destino?

# 3. Direccionamiento y servicios de red

>[!question] ¿Cómo funciona Internet?
> Internet es una red mundial formado por numerosas redes informáticas interconectadas. Estas redes pertenecen a empresas, universidades, administraciones públicas y proveedores de servicios. 
> Visualiza el siguiente video [¿Cómo funciona Internet](https://www.youtube.com/watch?v=rw41W8crZ_Y) y responde a las siguientes preguntas:
> 1. ¿Cómo se denomina la dirección única que identifica a cada dispositivo conectado a Internet? ¿Cuál es su estructura básica?
> 2. ¿Qué es un servidor DNS y cuál es su funcionamiento en la navegación por Internet?
> 3. Ejecuta el comando `ipconfig` (en Windows) o `ifconfig` (en Linux/Mac) en tu terminal y anota la dirección IP asignada a tu dispositivo. ¿Comparala con la dirección IP de tus compañeros de clase. ¿Son iguales o diferentes? ¿En qué se diferencian?

**Recurso adicional:** [The Internet: IP and DNS](https://www.youtube.com/watch?v=5o8CwafCxnU)

## 3.1 Direcciones IP

La dirección IP es el identificador de cada equipo/dispositivo dentro de un conjunto de redes (Internet). Cada dispositivo conectado a Internet debe tener una dirección IP asignada.

Las **direcciones IP están formadas por 4 bytes (32 bits)**. Se suelen representar de la forma `a.b.c.d` donde cada una de estas letras representa un byte (8 bits) y su valor puede ir de `0` a `255`. ()

>[!question] Clases de direcciones IP
>Las direcciones IP se clasifican en **clases A, B, C, D y E**, según el rango de direcciones que abarcan. **Las clases A, B y C son las utilizadas para direccionar redes privadas y públicas**.
>
>Para identificar a qué clase pertenece una IP, nos debemos fijar en que los primeros bits del primer byte.
>![[recursos/clasesIP.png]]
>
>Recurso: [IP Decimal a binario](https://www.youtube.com/watch?v=-AsYSB8QOEQ&list=PLKwGLCp8O0jHi26RByHWd0-JOapWk-aH0)
>
>1. **Identifica la clase a la que pertenecen las siguientes direcciones IP:**
 >   a. 12.168.14.255  
 >   b. 80.58.12.68  
 >   c. 172.67.14.92  
 >   d. 200.255.192.64  
 >   e. 190.72.90.0
>    
>2. **Completa la siguiente tabla indicando el rango de direcciones IP disponibles para cada una de las clases A, B y C:**
>
> | Clase   | Desde | Hasta |
>| ------- | ----- | ----- |
>| Clase A |       |       |
>| Clase B |       |       |
>| Clase C |       |       |
>
 
## 3.2 Identificador de red y de equipo

En cada IP tiene codificada la red a la que pertenece el equipo y al propio equipo dentro de esa red. A cada una de estas partes se denomina identificador de red e identificador de equipo (host). 

**La separación entre ambas partes viene dada por la mascara de red**. La máscara de subred es una dirección IP que indica qué parte de la dirección IP corresponde a la red y qué parte corresponde al host.

>[!info] Por cada dirección IP, existen dos partes diferenciadas:
>
>- **Identificador de red**: Permite identificar a la red a la que pertenece el dispositivo.
>- **Identificador de host**: Permite identificar al dispositivo dentro de la red.

La máscara de red se representa de la misma forma que una dirección IP, es decir, con 4 bytes separados por puntos. Los bits de la máscara que están en `1` indican la parte de la dirección IP que corresponde a la red, mientras que los bits en `0` indican la parte que corresponde al host.

Normalmente, podemos encontrarla representada de dos formas:

- **Notación decimal con puntos**: `255.255.255.0` En este caso los primeros 3 bytes están en `1` y el último en `0`, por lo que los primeros 24 bits corresponden a la red y los últimos 8 bits al host.
- **Notación CIDR (Classless Inter-Domain Routing)**: `/24` En este caso, el número indica la cantidad de bits que corresponden a la red. En este caso, los primeros 24 bits corresponden a la red y los últimos 8 bits al host.

**Recurso**: - [Red vs Host](https://www.youtube.com/watch?v=W_dTBb03oJQ&list=PLKwGLCp8O0jHi26RByHWd0-JOapWk-aH0&index=3)

>[!question] Identificador de red e identificador de host
>Dadas las siguientes direcciones IP y sus respectivas máscaras, indica cuál es el identificador de red y cuál es el identificador de host:
> 
> | #   | Dirección IP  | Máscara de Red | Identificador de Red (Net ID) | Identificador de Host (Host ID) |
>| --- | ------------- | -------------- | ----------------------------- | ------------------------------- |
>| 1   | 192.168.1.15  | 255.255.255.0  |                               |                                 |
>| 2   | 10.0.0.42     | 255.0.0.0      |                               |                                 |
>| 3   | 172.16.5.100  | 255.255.0.0    |                               |                                 |
>| 4   | 192.168.100.2 | 255.255.255.0  |                               |                                 |
>| 5   | 8.8.8.8       | 255.0.0.0      |                               |                                 |
>| 6   | 172.31.0.1    | /16            |                               |                                 |
>| 7   | 192.168.0.254 | /24            |                               |                                 |
>| 8   | 10.25.50.75   | /8             |                               |                                 |
>| 9   | 172.20.200.10 | /16            |                               |                                 |
>| 10  | 192.0.2.1     | /24            |                               |                                 |
>

>[!question] Direccionamiento de equipos de red
>Relaciona cada dirección IP con la red a la que pertenece. Habrá direcciones IP que no pertenezcan a ninguna de las redes indicadas, en cuyo caso habrá que obtener el identificador de red correspondiente.
>
>| Columna A: Direcciones IP (Dispositivos) | Columna B: Identificadores de Red |
>| ---------------------------------------- | --------------------------------- |
>| 1. 192.168.1.15 /24                      | A. 10.0.0.0 /8                    |
>| 2. 172.16.50.4 /16                       | B. 192.168.1.0 /24                |
>| 3. 10.1.1.100 /8                         | C. 172.16.0.0/16                  |
>| 4. 192.168.1.200 /16                     | D. 192.168.50.0 /24               |
>| 5. 172.16.1.25 /24                       | E. 172.20.0.0                     |
>| 6. 10.254.254.254 /16                    | F. 10.0.0.0 /16                   |
>| 7. 192.168.1.45 /24                      |                                   |
>| 8. 172.16.100.1 /24                      |                                   |
>| 9. 10.0.0.5 /16                          |                                   |
>| 10. 192.168.2.1 /24                      |                                   |
>

>[!question] Direcciones públicas vs direcciones privadas
>Investiga y responde a las siguientes preguntas ([IP Pública vs Privada: ¡Descubre la Diferencia!](https://youtu.be/42j3i3N2_4U?si=pdZAZXtHgfrwRxIK)):
>
>- ¿Con qué tipos de IPs, publica o privada, utilizan los diferentes servicios de Internet?
>- Por tanto, ¿Cuál es la diferencia entre una dirección IP pública y una dirección IP privada?

