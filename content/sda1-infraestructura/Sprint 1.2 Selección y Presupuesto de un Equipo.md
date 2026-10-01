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
>**Clasificación por nivel. Asignad el nivel según la siguiente escala.**
>- **Nivel Bajo (<15000)**: Puesto básico de facturación, caja/TPV y navegación ofimática.
>- **Nivel Medio(15000 - 28000):** Puesto administrativo multitaréa y gestión simultanea de aplicaciones.
>- **Nivel Alto(>28000):** Puesto de alto rendimiento, edición multimedia pesada o servidor local.
> 
>**Precio sin IVA.** Buscad el precio de venta en alguna tienda de informática de referencia [PCComponentes](https://www.pccomponentes.com/categorias/procesadores), [CoolMod](https://www.coolmod.com/componentes-pc-procesadores/)


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




