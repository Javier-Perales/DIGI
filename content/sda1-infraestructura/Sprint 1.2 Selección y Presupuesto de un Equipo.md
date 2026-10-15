---
title: Sprint 1.2 Selección y Presupuesto de un Equipo
sda: "Misión 1: Infraestructura"
tags:
  - cpu
  - ram
  - ssd
  - hd
  - usb
  - hdmi
criterios_evaluacion:
entregable: Informe previo de requerimientos. Hoja de cálculo de presupuesto. Informe justificativo de sostenibilidad
---

> [!abstract] El Desafío
> **Objetivo:** Analizar los requerimientos del cliente para comparar equipos comerciales y recomendar el puesto de trabajo que mejor se ajuste a sus necesidades. Justificar la elección mediante un presupuesto y criterios de consumo y sostenibilidad.

## 📦 Entregable

> [!question] 
> 1. [[recursos/Ficha previa de decisión de hardware.docx|Ficha previa de decisión de hardware.]] Ficha puente entre el briefing y el presupuesto. Convierte las necesidades reales detectadas en decisiones técnicas razonadas.
> **2. Hoja de cálculo con el presupuesto del equipo.** Comparativa entre dos opciones de hardware (Básica vs. Avanzada) con fórmulas dinámicas (SUMA, cálculo de IVA al 21%, totales y fórmula de coste eléctrico anual estimado en €/año).
> **3. Informe de sostenibilidad**. Análisis de la eficiencia de la fuente de alimentación, índice de reparabilidad y reducción de basura electrónica. 
---

# Explicación inicial de componentes

| Característica               | Función que deben recordar                                                     | Pregunta útil para el cliente                                       |
| ---------------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------- |
| **CPU**                      | Procesa las tareas de los programas.                                           | ¿Qué aplicaciones utilizará?                                        |
| **RAM**                      | Mantiene disponibles los programas y datos con los que trabaja en ese momento. | ¿Utilizará varias aplicaciones a la vez?                            |
| **Almacenamiento**           | Conserva aplicaciones y archivos.                                              | ¿Qué archivos guardará y cuánto espacio necesitará?                 |
| **GPU**                      | Procesa las imágenes que muestra o genera el equipo.                           | ¿Realizará tareas gráficas exigentes?                               |
| **Fuente de alimentación**   | Suministra energía a los componentes del equipo de sobremesa.                  | ¿Es adecuada para ese equipo y qué eficiencia indica el fabricante? |
| **Conexiones y periféricos** | Permiten conectar el equipo y utilizar otros dispositivos.                     | ¿Necesita impresora, TPV, monitor, red por cable…?                  |
| **Formato**                  | Determina si el equipo puede transportarse con facilidad.                      | ¿Trabajará siempre en el mismo puesto? ¿Necesidad de espacio?       |

> [!info] Identifica
> ![[recursos/componentes_hw.png]]
---

# 1. CPUs
Al analizar un procesador (CPU), hay varios factores clave que debes tener en cuenta para comprender su rendimiento y cómo se adapta a tus necesidades.

### 1.1. Arquitectura del procesador
La **CPU o procesador** es el componente encargado de ejecutar las instrucciones de los programas.

Al comparar procesadores, una de las características que debemos conocer es su **arquitectura**, que determina qué instrucciones pueden ejecutar. Podemos imaginarla como el «lenguaje» que entiende el procesador.

Dos de las familias de arquitecturas más habituales son **x86** y **ARM**. Dentro de cada una existen procesadores con prestaciones y consumos muy diferentes.

#### Arquitectura x86

- **Diseño CISC** (_Complex Instruction Set Computing_): incluye instrucciones que permiten realizar operaciones relativamente complejas. Esto no significa que todas se ejecuten en un único paso ni que el procesador sea más rápido.
- **Empresas destacadas:** **Intel y AMD** diseñan los procesadores x86 más habituales en los ordenadores personales.
- **Dispositivos comunes:** ordenadores de sobremesa, portátiles y servidores.
- **Denominación habitual:** en los equipos actuales encontramos principalmente **x86-64**, también denominada **x64**, que corresponde a la arquitectura de 64 bits.
#### Arquitectura ARM

- **Diseño RISC** (_Reduced Instruction Set Computing_): se basa en instrucciones generalmente más simples y regulares. Esto no significa que solo pueda ejecutar programas sencillos.  
- **Empresas destacadas:** Arm desarrolla y licencia la arquitectura y diseños de procesadores. Empresas como Apple, Qualcomm o Samsung diseñan chips basados en ARM.
- **Dispositivos comunes:** teléfonos móviles, tabletas, sistemas integrados y también portátiles, ordenadores de sobremesa y servidores.
- **Ejemplo:** desde 2020, Apple utiliza procesadores propios basados en ARM en sus Mac, como los de la serie M.
- **Denominación habitual:** en muchos dispositivos actuales aparece como **ARM64**, que corresponde a la arquitectura de 64 bits.

#### ¿Qué diferencias debemos tener en cuenta?

|Aspecto|Qué debemos comprobar|
|---|---|
|**Consumo y autonomía**|Muchos equipos ARM destacan por su eficiencia energética, pero el consumo depende del procesador concreto y la autonomía también depende de la batería, la pantalla y el uso.|
|**Rendimiento**|Ambas arquitecturas pueden ofrecer un rendimiento elevado. Debemos comparar modelos concretos y su comportamiento en las tareas que necesitamos realizar.|
|**Compatibilidad**|El sistema operativo, los programas y los controladores de los periféricos deben ser compatibles con la arquitectura elegida. Algunas aplicaciones pueden funcionar mediante traducción o emulación.|

>[!tip] Recomendación de CPU
>Antes de recomendar un equipo, identifica **qué programas y periféricos necesita el cliente** y comprueba su compatibilidad con el sistema operativo y la arquitectura del procesador.
>Después, compara el rendimiento, la autonomía y el precio de los equipos que cumplen esos requisitos.
>
>**La arquitectura por sí sola no permite decidir qué procesador es mejor: la elección debe responder a las necesidades del cliente.**

>[!question] Comparar CPU para recomendar hardware. **FASE 1. Compara el rendimiento y el precio**
>**RESUELVE LA ACTIVIDAD EN EL DOCUMENTO `Comparativa_CPU.docx` ALMACENADO EN LA CARPETA `02_Hardware`**
>
>Antes de recomendar el hardware del equipo de nuestro cliente, debemos conocer las características de distintos procesadores y valorar qué opciones se ajustan a sus necesidades.
>En esta actividad investigarás tres CPU, compararás sus prestaciones y justificarás una recomendación.
> 
>Los nombres comerciales no siempre reflejan la potencia real de un procesador. Vais a medir la capacidad de cálculo bruto mediante una prueba estandarizada (_benchmark_) y a registrar su coste actual.
>**Herramienta de rendimiento:** Acceded a **[PassMark CPU Benchmarks](https://www.cpubenchmark.net/cpu-list/)**  y buscad cada modelo en la barra superior para obtener su puntuación **CPU Mark**. 
>
>|Modelo de CPU|Puntuación CPU Mark|Clasificación por nivel|Precio aproximado sin IVA (€)|Tienda y fecha de consulta|
>|---|---|---|---|---|
>|Ryzen 7 7700|||||
>|Intel Core i3-12100|||||
>|Intel Core i5-13400|||||
>|AMD Ryzen 5 5600G|||||
>|Intel Core i7-14700|||||
>|AMD Ryzen 5 4600G|||||
>
>**Clasificación por nivel. Asignad el nivel según la siguiente escala.**
>- **Nivel Bajo (<15000)**: Puesto básico de facturación, caja/TPV y navegación ofimática.
>- **Nivel Medio(15000 - 28000):** Puesto administrativo multitaréa y gestión simultanea de aplicaciones.
>- **Nivel Alto(>28000):** Puesto de alto rendimiento, edición multimedia pesada o servidor local.
> 
>**Precio sin IVA.** Buscad el precio de venta en alguna tienda de informática de referencia [PCComponentes](https://www.pccomponentes.com/categorias/procesadores), [CoolMod](https://www.coolmod.com/componentes-pc-procesadores/)


>[!question] El dilema económico
>El gerente de la empresa os pide directamente que instaléis el **Intel Core i7-14700** porque "quiere que el ordenador no se quede viejo nunca", aunque su  uso diario consistirá en emitir facturas, consultar el correo y gestionar pedidos web.
>- Observando la tabla anterior: **¿cuánta diferencia de precio y rendimiento hay respecto al i3 o Ryzen 5?**
>- Como consultores **¿qué le recomendaríais para evitar un gasto desproporcionado?**


>[!question] Comparar CPU para recomendar hardware. **FASE 2. Características Técnicas**
>Completa la siguiente tabla **respetando el modelo exacto indicado:** una letra o un sufijo diferente puede corresponder a otro procesador.
>
>**Herramienta de especificaciones**: [techpowerup.com/cpu-specs](https://techpowerup.com/cpu-specs), localizad cada modelo exacto y completad los siguientes parámetros:
>- **Socket:** Tipo de zócalo para verificar compatibilidad con la placa base.   
>- **Núcleos / Hilos (Cores / Threads):** Capacidad de cálculo simultáneo.
>- **Caché (L1/L2/L3)**: memoria rápida situada en el procesador que almacena temporalmente datos e instrucciones para reducir los accesos a la RAM.
>- **Frecuencia Turbo (Boost Clock):** Velocidad máxima en GHz.
>- **TDP (Thermal Design Power):** Consumo térmico y energético en Vatios (W).
>- **Gráficos Integrados (IGP):** Indicad si el chip incluye tarjeta gráfica integrada (**Sí / No**).
>
>|Procesador|Socket compatible|Núcleos / Hilos|Frecuencia Turbo (GHz)|Caché (L1 / L2 / L3)|Consumo TDP (W)|¿Lleva gráficos integrados? (Sí/No)|
>|---|---|---|---|---|---|---|
>|**Intel Core i3-12100**|||||||
>|**AMD Ryzen 5 4600G**|||||||
>|**Intel Core i5-13400**|||||||
>|**AMD Ryzen 5 5600G**|||||||
>|**Intel Core i7-14700**|||||||
>|**AMD Ryzen 7 7700**|||||||
>
:

- **Socket o zócalo** es la interfaz física que conecta el procesador a la placa base. Cada tipo de procesador requiere un socket específico, por lo que es crucial asegurarse de que el procesador y la placa base sean compatibles.
- Un **core o núcleo** es una unidad de procesamiento independiente dentro del procesador. Cuantos más núcleos tenga un procesador, más tareas puede manejar simultáneamente.
- Los **hilos / threads** son las unidades más pequeñas que gestionan las tareas dentro de un núcleo. Más hilos permiten un mejor rendimiento en aplicaciones multitarea y tareas que se benefician del paralelismo, como edición de video o renderizado 3D.
- La **frecuencia** de los procesadores se mide en gigahercios (GHz), que representan miles de millones de ciclos por segundo. Un procesador de 3.5 GHz, por ejemplo, ejecuta 3,500 millones de ciclos cada segundo.
- La **memoria caché** es una memoria muy rápida integrada en la CPU para almacenar datos e instrucciones de uso frecuente. Tipos: - L1: Pequeña y ultrarrápida, cercana a los núcleos. - L2: Un poco más grande y más lenta que L1. - L3: Compartida entre todos los núcleos, más lenta pero de mayor capacidad.
- **TDP (Thermal Design Power)** medida en vatios, indica la cantidad de calor que el procesador disipa bajo carga máxima. Un TDP más alto implica mayor consumo de energía y la necesidad de mejores soluciones de refrigeración.
- La mayoría de los procesadores modernos incluyen una **tarjeta gráfica integrada**, que es útil para tareas gráficas básicas sin necesidad de una tarjeta gráfica dedicada.

>[!question] Selección de procesador
>Antes de recomendar un equipo a nuestro cliente, debemos clasificar el mercado de procesadores según su rendimiento real, coste real y consumo energético.
>Asigna cada uno de los procesadores anteriores a una de las siguientes categorías. Razona la respuesta.
>1. **Gama Entrada (Ofimática / TPV):**
>2. **Gama Media (Multitarea / Estándar):**
>3. **Gama Alta/Profesiona (Edición / Carga Pesada):**

#### Comparativa ARM
En el punto anterior comparamos y clasificamos procesadores de arquitectura x86 de Intel y AMD. En este apartado vamos a evaluar los procesadores ARM de Apple y Qualcom

| Modelo de CPU                | Puntuación CPU Mark | Socket compatible | Núcleos / Hilos | Frecuencia Turbo (GHz) | Caché (L1 / L2 / L3) | Consumo TDP (W) | ¿Lleva gráficos integrados? (Sí/No) |
| ---------------------------- | ------------------- | ----------------- | --------------- | ---------------------- | -------------------- | --------------- | ----------------------------------- |
| Apple M3                     | 19.100              | SoC soldado       | 8/8             | 4GHz                   | NP                   | ~20W            | Sí                                  |
| Snapdragon X Plus X1P 64-100 | 21.400              | SoC soldado       | 10/10           | 3,4GHz                 | 42 MB en total       | ~20W            | Síu                                 |

>[!question] Sostenibilidad. Rendimiento por Vatio
>- Observad el *CPU Mark* del *Ryzen 5 5600G* y el del *Apple M3* o *Snapdragon X Plus*. Rinden prácticamente los mismo. Ahora mirad la columna de consumo. **¿Por qué un portátil con chip ARM aguanta 15 horas de batería y apenas se calienta, mientras que una torre tradicional necesita disipadores de calor y ventiladores?**

>[!question] La trampa de la reparabilidad
>En la torre con el *Core i3-12100*, si dentro de 3 años el cliente necesita más potencia o se quema la placa base, cambiamos esa pieza por 80 € y el ordenador sigue funcionando. **Si en el equipo con *Apple M3* o *Snapdragon* falla la memoria RAM o se estropea el chip, ¿qué ocurre?**

>[!question] El veredicto del consultor
>Vuestro cliente de la tienda local os dice: 'Quiero un equipo para tenerlo fijo en el mostrador cobrando y haciendo pedidos durante 8 años'.
>**¿Le recomendáis una torre modular x86 (Intel/AMD) o un equipo compacto con chip ARM soldado?** Justificad vuestra respuesta valorando coste inicial, consumo de luz y facilidad de reparación.
>Partimos de los siguientes supuestos:
>- Torre en formato Micro-ATX equipada con un procesador Intel i3-12100 o AMD RYzen 5 4600G puede estar sobre los 450€ sin IVA.
>- Un MiniPC con procesador ARM puede estar sobre los 850€
>- Tomamos como base que el comercio está abierto 8 horas al día, 300 días al año (2400 horas anuales) y un precio medio de la electricidad de 0,18€KWh.

>[!question] A103(CE1+CE5) Comparativa de CPU
>Entrega en formato pdf el documento `Comparativa_CPU`. 
>El documento deberá contener todas las respuestas a las cuestiones anteriores.
# 2. RAM

Analogía:
- **SSD/HDD = armario**  
- **RAM = mesa de trabajo**  
- **CPU = persona que está trabajando**

Cuanta más memoria RAM tenga el equipo, más programas y datos podrá mantener disponibles simultáneamente sin necesidad de recurrir continuamente al almacenamiento.

**La memoria RAM almacena temporalmente los programas y datos que el ordenador está utilizando en ese momento. Su contenido se pierde cuando apagamos el equipo.**
**RAM → temporal**  
**SSD/HDD → permanente**

**Capacidad → GB (gigabytes)**

Si consultamos en Windows con el Administrador de Tareas (Task Manager) cuánta memoria tiene el equipo, podría salir una pantalla similar a esta.
![[../recursos/memoria windows.png]]
En Linux podríamos ejecutar en el terminal el comando `free -h`

>[!example] ¿Qué ocurre cuando falta RAM?
>Abre el navegador, varias pestañas, LibreOffice y alguna aplicación adicional.
>Observa cómo aumenta el consumo de memoria. Es posible que el ordenador empiece a ir lento.
>**Cuando la RAM disponible se aproxima a su límite, el sistema puede empezar a responder más lentamente.**

## 2.1 Características para comparar módulos

| RAM               | Capacidad | Tipo | Velocidad |
| ----------------- | --------: | ---- | --------: |
| Kingston Fury     |      8 GB | DDR4 |  3200 MHz |
| Crucial           |     16 GB | DDR4 |  3200 MHz |
| Corsair Vengeance |     16 GB | DDR5 |  5600 MHz |
## 2.2 ¿Cuánta RAM necesita mi cliente?

| Cliente            | Uso                                   | RAM propuesta |
| ------------------ | ------------------------------------- | ------------: |
| Administración     | Navegador + Office + correo           |      **8 GB** |
| Comercio           | Navegador + Office + TPV + multitarea |     **16 GB** |
| Diseño             | Photoshop/GIMP + edición multimedia   |  **16–32 GB** |
| Edición vídeo / 3D | Aplicaciones exigentes                |     **32 GB** |
- **¿Comprarías 64 GB para un ordenador utilizado únicamente para facturación y correo electrónico?**
- **Más RAM no siempre significa mejor compra. Hay que dimensionarla según las necesidades del cliente.**

>[!question] Análisis de equipos comerciales
>Una empresa va a adquirir varios ordenadores para diferentes perfiles de usuario.
> Completa la tabla y guardala en el documento `Análisis RAM.docx` dentro de `02_Hardware`
>|Enlace|Nombre Comercial|Precio|Procesador|Capacidad RAM|Tipo(DDR4/DDR5)|Tipo Cliente|
>|---|---|---|---|---|---|---|
>|[1](https://www.pccomponentes.com/pc-differo-v15-intel-core-i3-12100-8gb-500gb-ssd-nvme-mini-tower)| | | | | |
>|[2](https://www.pccomponentes.com/pccom-work-amd-ryzen-5-8500g-16gb-1tb-ssd)| | | | | |
>|[3](https://www.pccomponentes.com/pc-sobremesa-hp-z2-tower-g1i-intel-core-ultra-7-265k-64gb-1tb-ssd-intel-graphics-windows-11-pro-wi-fi-7)| | | | | |
>|[4](https://www.pccomponentes.com/pccom-work-intel-core-i3-12100-16gb-500gb-ssd-v4)| | | | | |
>|[5](https://www.pccomponentes.com/pccom-studio-intel-core-i7-14700kf-32gb-2tb-ssd-rtx-5070-ti-v2-windows-11-pro)| | | | | |

# 3. Almacenamiento secundario

El almacenamiento secundario es el conjunto de dispositivos que permiten **guardar información de forma permanente**, incluso cuando apagamos el ordenador.

En estos dispositivos se almacenan el sistema operativo, los programas, los documentos, las fotografías y otros archivos.

La principal diferencia con la memoria RAM es que esta última es volátil: pierde su contenido cuando se interrumpe la alimentación eléctrica.

| Característica | Memoria RAM | Almacenamiento secundario |
|---|---|---|
| **Función** | Guardar temporalmente datos en uso | Guardar archivos y programas |
| **Volatilidad** | Volátil | No volátil |
| **Velocidad** | Muy alta | Generalmente inferior a la RAM |
| **Capacidad habitual** | 8–32 GB | 256 GB–4 TB |
| **Conserva datos al apagar** | No | Sí |
## 3.1 Principales tecnologías

#### HDD (Hard Disk Drive)

Disco duro mecánico que almacena información magnéticamente en platos giratorios.

- Gran capacidad a bajo precio.  
- Tiene componentes mecánicos.
- Más lento y sensible a golpes.
- Adecuado para almacenar grandes cantidades de archivos.

![[../recursos/hdd.png|250]]

#### SSD SATA (Solid State Drive)

Unidad de estado sólido que utiliza memoria flash, sin partes móviles.

- Mayor velocidad que un HDD.
- Utiliza habitualmente la interfaz SATA III.
- Velocidad secuencial típica de hasta unos 550 MB/s.
- Buena opción para modernizar ordenadores antiguos.
![[../recursos/ssd.png|250]]

#### SSD NVMe (Non-Volatile Memory Express)

Unidad de estado sólido que normalmente utiliza PCI Express para comunicarse con el ordenador.

- Velocidad muy superior a SATA.
- Habitualmente tiene formato físico M.2.
- Velocidades de varios miles de MB/s.
- Ideal para equipos modernos y aplicaciones exigentes.
![[../recursos/nvme.png|250]]
## 3.2 Características técnicas
Para comparar dispositivos de almacenamiento, estudiaremos cuatro características.

|Característica|Explicación|
|---|---|
|Tecnología|HDD o SSD|
|Capacidad|Cantidad de información que puede almacenar, expresada en GB o TB|
|Interfaz|Sistema de conexión y comunicación: SATA o PCIe/NVMe|
|Velocidad de lectura secuencial|Cantidad de datos que puede leer por segundo, expresada en MB/s|
>[!question] Ampliación de análisis de equipos comerciales
> Renombra el archivo 'Analisis_RAM.docx' por '**Analisis_PC.docx**'
> La tabla completa podría tener esta estructura:
> 
>| Torre                              | Tipo almacenamiento | Capacidad | Interfaz | Lectura (MB/s) |
>| ---------------------------------- | ------------------- | --------- | -------- | -------------- |
>| [1](https://www.pccomponentes.com/pc-differo-v15-intel-core-i3-12100-8gb-500gb-ssd-nvme-mini-tower)                  | ...                 | ...       | ...      | ...            |
>| [2](https://www.pccomponentes.com/pccom-work-amd-ryzen-5-8500g-16gb-1tb-ssd)       | ...                 | ...       | ...      | ...            |
>| [3](https://www.pccomponentes.com/pc-sobremesa-hp-z2-tower-g1i-intel-core-ultra-7-265k-64gb-1tb-ssd-intel-graphics-windows-11-pro-wi-fi-7)      | ...                 | ...       | ...      | ...            |
>| [4](https://www.pccomponentes.com/pccom-work-intel-core-i3-12100-16gb-500gb-ssd-v4)     | ...                 | ...       | ...      | ...            |
>| [5](https://www.pccomponentes.com/pccom-studio-intel-core-i7-14700kf-32gb-2tb-ssd-rtx-5070-ti-v2-windows-11-pro) | ...                 | ...       | ...      | ...            |
>
>Si alguna torre tiene dos unidades de almacenamiento, deberás registrar ambas.
>1. Identifica si utiliza HDD, SSD SATA o SSD NVMe.
>2. Indica su capacidad en GB o TB.
>3. Investiga qué interfaz de conexión utiliza. 
>4. Localiza la velocidad de lectura secuencial anunciada por el fabricante, si está disponible.
>5. **Cuando el fabricante no proporcione algún dato, escribe «No especificado». No inventes valores ni utilices los de otro modelo.**

>[!question] Responde a estas tres cuestiones:
>Después, responde a estas tres cuestiones:
 >- **P1**. ¿Qué torre dispone del almacenamiento más rápido? Justifica tu respuesta.
>- **P2**. ¿Qué torre tiene mayor capacidad total de almacenamiento? ¿Coincide con la torre que tiene el procesador más rápido?    
>- **P3**. Para un ordenador destinado a tareas de ofimática y navegación web, ¿elegirías un HDD de 2 TB o un SSD NVMe de 500 GB? Justifica tu elección


# 4. Fuentes de alimentación y eficiencia energética

La **fuente de alimentación** (PSU, *Power Supply Unit*) transforma la corriente alterna de la red eléctrica en corriente continua, que necesitan los componentes de un ordenador de sobremesa.

Al elegir una fuente debemos comprobar **dos características diferentes**:
- **Potencia (W):** cuánta energía por segundo puede suministrar a los componentes. Se expresa en vatios.
- **Eficiencia (%):** qué proporción de la energía tomada del enchufe llega realmente a los componentes. La parte restante se pierde principalmente en forma de calor.
 
## 4.1. ¿Qué significa que una fuente sea eficiente?

Imaginad dos fuentes que suministran **200 W a los componentes** del mismo ordenador:
- Una fuente con **80 % de eficiencia** necesita tomar **250 W del enchufe**.
- Una fuente con **90 % de eficiencia** necesita tomar aproximadamente **222,2 W del enchufe**.

La segunda desperdicia menos energía para realizar el mismo trabajo.

**Fórmulas:**
- `Eficiencia = Potencia de salida / Potencia de entrada` (expresada como porcentaje si multiplicamos por 100).
- `Potencia de entrada (W) = Potencia de salida (W) / Eficiencia` (la eficiencia se introduce como decimal: 0,90 para el 90 %).

## 4.2. Certificación 80 PLUS

**80 PLUS** es un programa de certificación que permite comparar la eficiencia de determinadas fuentes de alimentación. Sus niveles más habituales en equipos de sobremesa son **Standard, Bronze, Silver, Gold, Platinum y Titanium**.

| Nivel de Certificación          | Eficiencia típica al 50 % de carga | Pérdida en calor | Uso recomendado en la empresa                                     |
| :------------------------------ | :--------------------------------: | :--------------: | :---------------------------------------------------------------- |
| **Genérica (Sin sello)**        |            ~65 % - 70 %            |   30 % - 35 %    | ❌ **Desaconsejada**: riesgo eléctrico y mayor gasto energético.   |
| **80 PLUS White (Básica)**      |                80 %                |       20 %       | Equipos de uso esporádico o presupuestos muy ajustados.           |
| **80 PLUS Bronze**              |                85 %                |       15 %       | Puesto de oficina estándar y comercios de proximidad.             |
| **80 PLUS Gold**                |                90 %                |       10 %       | Puestos con jornadas intensivas (cajas, TPV, servidores locales). |
| **80 PLUS Platinum / Titanium** |            92 % - 94 %             |    6 % - 8 %     | Servidores 24/7 y estaciones de trabajo de alto rendimiento.      |

**Fuente de consulta:** [80 PLUS – Tabla oficial para 230 V EU](https://www.clearesult.com/80plus/taxonomy/term/9). Podéis comprobar si un modelo concreto aparece en el [buscador de fuentes certificadas](https://www.clearesult.com/80plus/).

## 4.3. ¿Cuánto dinero puede ahorrar una fuente eficiente?

Recuperamos el caso de **la tienda local** estudiado al comparar las CPU. El negocio utiliza el ordenador **8 horas al día, 300 días al año** y paga **0,18 €/kWh** por la electricidad.

Para aislar el efecto de la fuente, comparamos **dos fuentes hipotéticas de 400 W** que alimentan exactamente el mismo equipo, cuando este solicita **200 W de salida** (el 50 % de su potencia nominal).

| Dato                                 | Fuente A (Bronze) | Fuente B (Gold) |
| ------------------------------------ | ----------------: | --------------: |
| Potencia nominal de la fuente        |             400 W |           400 W |
| Potencia entregada a los componentes |             200 W |           200 W |
| Eficiencia al 50 % de carga          |              88 % |            92 % |
| Potencia tomada del enchufe          |          227,27 W |        217,39 W |
| Energía en 2.400 horas               |        545,45 kWh |      521,74 kWh |
| **Coste eléctrico anual**            |       **98,18 €** |     **93,91 €** |

**Consumo anual (kWh):** 
$$\text{Consumo (kWh)} = \frac{\text{Potencia tomada del enchufe (W)} \times \text{Horas de uso al año (h)}}{1000}$$ 
**Coste anual estimado (€/año):**  
 $$\text{Coste anual (€)} = \text{Consumo (kWh)} \times \text{Precio de la electricidad (€/kWh)}$$ 
**Resultado:** bajo estos supuestos, la fuente Gold ahorraría aproximadamente **4,27 € al año** respecto a la Bronze. En **8 años**, el ahorro sería de unos **34,15 €**, si las condiciones no cambian.

# 5. Basura electrónica (RAEE) y reparabilidad

Cuando un ordenador, un monitor o un periférico deja de utilizarse y se desecha, puede convertirse en un **residuo de aparato eléctrico y electrónico (RAEE)**. En inglés se utiliza la expresión ***e-waste***.

Estos equipos contienen materiales valiosos, como metales y plásticos, pero también componentes que requieren una recogida y un tratamiento adecuados. **No deben tirarse al contenedor de basura convencional.**
## 5.1. Antes de tirar, ¿podemos alargar su vida útil?

| Decisión                          | Ejemplo en el comercio del cliente                                                  | ¿Qué conseguimos?                                       |
| --------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------- |
| **Evitar una compra innecesaria** | No sustituir un ordenador que sigue cubriendo las necesidades del TPV.              | Evitar generar residuos antes de tiempo.                |
| **Reparar o ampliar**             | Cambiar un SSD, aumentar la RAM o sustituir una pieza averiada.                     | Prolongar la vida útil del equipo.                      |
| **Reutilizar**                    | Destinar un monitor funcional a otro puesto del negocio.                            | Aprovechar un producto que todavía funciona.            |
| **Reciclar correctamente**        | Entregar un teclado irreparable o una fuente averiada en un canal de recogida RAEE. | Facilitar un tratamiento seguro y recuperar materiales. |

**Idea clave:** reciclar es importante, pero **evitar residuos, reparar y reutilizar** puede ser preferible cuando el dispositivo sigue siendo seguro y útil.

> [!tip] Un ordenador lento no es necesariamente basura
> Si el equipo de la tienda tarda demasiado en arrancar, **antes de recomendar uno nuevo** comprobad si cumple los requisitos del negocio y si una ampliación de RAM, un SSD o una actualización del software permitirían seguir utilizándolo.
>

## 5.2. ¿Cómo valoramos la reparabilidad de un equipo?

La **reparabilidad** es la facilidad para mantener, desmontar, reparar o sustituir componentes sin desechar todo el ordenador.

Para comparar nuestras propuestas utilizaremos un **índice didáctico de reparabilidad de 0 a 5 puntos**. **No es una calificación oficial del fabricante**.

| Criterio que debemos verificar | Puntos |
|---|---:|
| Permite acceder a los componentes sin dañarlos. | 1 |
| La memoria RAM puede sustituirse o ampliarse. | 1 |
| La unidad de almacenamiento puede sustituirse. | 1 |
| La fuente de alimentación o el cargador puede sustituirse. | 1 |
| Existen repuestos o documentación de mantenimiento para el modelo. | 1 |
| **Máximo** | **5 puntos** |

**Puntuación:** asignad **1** cuando el criterio esté confirmado y **0** cuando se haya comprobado que no se cumple. Si no encontráis información suficiente, anotad **«No especificado»**; no lo confundáis con una imposibilidad demostrada de reparación ni inventéis una puntuación total.

>[!question] Torre modular frente a equipo compacto
>Recuperad los dos tipos de equipos valorados en la sección de CPU: **torre modular x86** y **equipo compacto con chip ARM**.
>
>- Aplicad el índice anterior a dos modelos concretos. Buscad información en sus fichas técnicas, manuales o documentación de reparación.
>- ¿Qué componentes podrían sustituirse en cada uno si fallan después de tres años?
>- ¿Qué opción recomendaríais para el mostrador de un comercio que quiere utilizar el puesto durante **ocho años**? Justificad tanto sus ventajas como sus limitaciones.

## 5.3. ¿Dónde acaba la basura electrónica?

Los RAEE deben entregarse en un **canal de recogida autorizado**, por ejemplo un punto limpio que admita ese tipo y procedencia de residuo, el distribuidor en los supuestos correspondientes o un gestor de RAEE autorizado. En un negocio hay que comprobar qué sistema de recogida corresponde a sus residuos.

**Antes de entregar o reutilizar un ordenador que haya almacenado información del comercio**, es imprescindible eliminar los datos de clientes, contraseñas y documentos mediante un procedimiento adecuado de borrado seguro o gestión del soporte.

**Fuente de consulta:** [MITECO – Recogida de residuos de aparatos eléctricos y electrónicos](https://www.miteco.gob.es/es/calidad-y-evaluacion-ambiental/temas/prevencion-y-gestion-residuos/flujos/domesticos/fracciones/aparatos_electr/electricos-y-electronicos-donde-depositarlos.html).

>[!question] Decide el destino de los equipos del cliente
>Durante el inventario de la tienda encuentras estos dispositivos. Completa la tabla con una **decisión razonada**: mantener, reparar/ampliar, reutilizar o entregar como RAEE.
>
>| Dispositivo | Situación detectada | Decisión | Justificación y siguiente paso |
>|---|---|---|---|
>| Ordenador de caja | Funciona, pero arranca muy lento. Tiene HDD y 8 GB de RAM. | | |
>| Monitor de 22 pulgadas | Funciona correctamente, pero se ha comprado otro más grande. | | |
>| Teclado | Tiene varias teclas averiadas y la reparación no es viable. | | |
>| Antiguo PC del gerente | Se va a retirar y contiene facturas y datos de clientes. | | |
>
>**Importante:** no todos los dispositivos deben acabar en el mismo lugar. Diferenciad los que todavía tienen utilidad de los que ya son residuos y tened en cuenta la protección de datos.

