# Arquitectura del Sistema

> Este documento describe cómo circula el conocimiento dentro del Servicio Meteorológico Social.

No representa una arquitectura de software.

No describe servidores.

No describe tecnologías.

Describe la arquitectura conceptual del método.

---

# Índice

1. Propósito
2. Arquitectura general
3. Flujo de conocimiento
4. Motores del sistema
5. Bases de información
6. Productos
7. Principios de diseño

---

# 1. Propósito

La arquitectura del sistema existe para ordenar el recorrido que transforma observaciones territoriales distribuidas en evidencia útil.

El sistema no transforma personas en datos.

Transforma observaciones en conocimiento territorial.

---

# 2. Arquitectura general

```text
RED DE ESTACIONES

        │
        ▼

OBSERVACIONES

        │
        ▼

EVENTOS

        │
        ▼

FENÓMENOS

        │
        ▼

INDICADORES

        │
        ▼

PRONÓSTICOS

        │
        ▼

RECOMENDACIONES

        │
        ▼

DEVOLUCIÓN A LA RED
```

La arquitectura posee un ciclo cerrado.

Toda observación ingresa al sistema, se transforma en conocimiento y debe volver a la red mediante una devolución.

---

# 3. Flujo de conocimiento

## 3.1 Estaciones

Las estaciones constituyen los puntos de observación del sistema.

En la implementación inicial serán personas.

A futuro podrán ser organizaciones, instituciones, sensores automáticos u otros sistemas capaces de producir observaciones bajo protocolo.

---

## 3.2 Observaciones

Las observaciones son registros realizados por estaciones.

Describen hechos situados en un territorio y un período determinado.

No interpretan.

No explican.

No recomiendan.

---

## 3.3 Eventos

Los eventos son manifestaciones concretas identificadas a partir de observaciones.

Un evento posee territorio, tiempo y contenido observable.

Los eventos permiten agrupar observaciones relacionadas sin convertirlas todavía en explicación.

---

## 3.4 Fenómenos

Los fenómenos surgen de la integración de eventos.

Un fenómeno representa un patrón observable.

No constituye una causa.

No constituye una solución.

No constituye una recomendación.

---

## 3.5 Indicadores

Los indicadores sintetizan información sobre eventos y fenómenos.

Permiten comparar territorios, períodos y evolución temporal.

Los indicadores no son conclusiones.

Son evidencia organizada.

---

## 3.6 Pronósticos

Los pronósticos estiman la evolución probable de uno o más fenómenos territoriales.

Todo pronóstico debe indicar:

* territorio;
* período de validez;
* evidencia utilizada;
* nivel de confianza.

---

## 3.7 Recomendaciones

Las recomendaciones transforman pronósticos en posibles líneas de acción.

No pertenecen al proceso de observación.

Representan una aplicación del conocimiento producido por el sistema.

---

## 3.8 Devolución

La devolución cierra el ciclo.

La red no sólo entrega observaciones.

También recibe conocimiento.

Sin devolución, el sistema se transforma en extracción de datos.

---

# 4. Motores del sistema

## 4.1 Motor de participación

Mantiene activa la red de estaciones.

Trabaja sobre:

* incorporación;
* permanencia;
* devolución;
* confianza;
* continuidad.

---

## 4.2 Motor de observación

Convierte aportes de las estaciones en observaciones válidas.

Trabaja sobre:

* protocolo;
* frecuencia;
* territorialización;
* formato;
* criterios de validez.

---

## 4.3 Motor territorial

Asocia las observaciones, eventos y fenómenos con unidades territoriales.

Puede integrar:

* barrios;
* radios censales;
* circuitos electorales;
* localidades;
* municipios;
* capas externas.

---

## 4.4 Motor analítico

Procesa observaciones, eventos y fenómenos para producir indicadores.

Trabaja sobre:

* históricos;
* agregaciones;
* comparación temporal;
* comparación territorial;
* detección de patrones.

---

## 4.5 Motor de pronóstico

Transforma indicadores en escenarios probables.

No produce recomendaciones.

Produce estimaciones sobre la evolución de fenómenos.

---

## 4.6 Motor de comunicación

Transforma pronósticos en recomendaciones.

Su función no es observar.

Su función es asistir la toma de decisiones comunicacionales.

---

# 5. Bases de información

## 5.1 Base operacional

Representa el presente del sistema.

Contiene:

* estaciones;
* observaciones;
* eventos;
* registros de participación;
* devoluciones realizadas.

---

## 5.2 Base analítica

Representa el conocimiento acumulado.

Contiene:

* fenómenos;
* indicadores;
* series históricas;
* pronósticos;
* evaluaciones de resultados.

---

# 6. Productos

## 6.1 Evidencia territorial

Resultado principal del método.

Incluye:

* observaciones;
* eventos;
* fenómenos;
* indicadores.

---

## 6.2 Pronóstico territorial

Estimación sobre la evolución probable de fenómenos en un territorio y período determinado.

---

## 6.3 Recomendación comunicacional

Aplicación del pronóstico a una decisión de comunicación.

---

## 6.4 Devolución comunitaria

Producto destinado a la red de estaciones.

Puede incluir:

* mapas;
* resúmenes;
* boletines;
* comparaciones territoriales;
* evolución histórica.

---

# 7. Principios de diseño

## 7.1

El método tiene prioridad sobre la tecnología.

---

## 7.2

La arquitectura debe seguir siendo válida aunque cambie la implementación.

---

## 7.3

Ninguna observación debe convertirse directamente en recomendación.

---

## 7.4

Todo pronóstico debe construirse sobre evidencia territorial.

---

## 7.5

Toda participación debe producir devolución.

---

## 7.6

La arquitectura debe permitir reconstruir el recorrido completo desde una recomendación hasta las observaciones que la hicieron posible.

---

# Regla editorial

Este documento describe la arquitectura conceptual del sistema.

La arquitectura técnica deberá documentarse en otro lugar sólo cuando exista una implementación concreta.

No se debe incorporar tecnología en este documento salvo que sea indispensable para explicar el método.
