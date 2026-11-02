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
 
# 3 ¿Cómo se conectan los dispositivos de nuestro negocio?

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

>[!example] Diseña la conectividad de tu negocio
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


