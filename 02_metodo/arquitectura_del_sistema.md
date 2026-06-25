# Arquitectura del Sistema

> Este documento describe cómo circula el conocimiento dentro del Servicio Meteorológico Social. No representa una arquitectura de software. Representa la arquitectura del método.

---

# Índice

1. Filosofía
2. Arquitectura general
3. Flujo operativo
4. Los motores del sistema
5. Bases de información
6. Productos
7. Escalabilidad
8. Principios

---

# 1. Filosofía

El Servicio Meteorológico Social no transforma personas en datos.

Transforma observaciones distribuidas en conocimiento colectivo.

La arquitectura del sistema refleja ese recorrido.

---

# 2. Arquitectura general

```text
                   COMUNIDAD

            (Estaciones humanas)

                      │
                      ▼

               OBSERVACIONES

                      │
                      ▼

            BASE OPERACIONAL (OLTP)

                      │
                      ▼

         NORMALIZACIÓN Y CLASIFICACIÓN

                      │
                      ▼

            BASE ANALÍTICA (OLAP)

                      │
          ┌───────────┼────────────┐
          ▼           ▼            ▼

      INDICADORES   MAPAS     SERIES TEMPORALES

          └───────────┼────────────┘
                      ▼

                PRONÓSTICOS

                      │
                      ▼

     RECOMENDACIONES DE COMUNICACIÓN

          ┌───────────┴───────────┐

          ▼                       ▼

   CONSULTOR               COMUNIDAD

                      ▲
                      │
                DEVOLUCIÓN
```

La arquitectura posee un ciclo cerrado.

Toda observación vuelve finalmente a la comunidad transformada en conocimiento.

---

# 3. Flujo operativo

## Paso 1

La estación observa.

No interpreta.

No explica.

No debate.

---

## Paso 2

La observación ingresa al sistema.

Se registra.

Se georreferencia.

Se clasifica.

---

## Paso 3

Las observaciones comienzan a formar series históricas.

Aparecen patrones.

No opiniones.

---

## Paso 4

El laboratorio incorpora contexto.

Capas SIG.

Resultados electorales.

Infraestructura.

Demografía.

Servicios.

Noticias.

---

## Paso 5

Se generan indicadores.

No conclusiones.

Indicadores.

---

## Paso 6

Los indicadores producen un pronóstico.

El pronóstico nunca surge de una única estación.

Siempre representa el comportamiento de la red.

---

## Paso 7

El consultor recibe una recomendación.

No una orden.

Una recomendación basada en evidencia.

---

## Paso 8

La comunidad recibe una devolución.

Mapas.

Indicadores.

Pronósticos.

Conocimiento colectivo.

La devolución alimenta un nuevo ciclo de observación.

---

# 4. Los motores del sistema

## Motor de Participación

Su función es mantener viva la comunidad.

Produce.

* incorporación;
* permanencia;
* participación.

Nunca genera pronósticos.

---

## Motor de Observación

Convierte conversaciones territoriales en observaciones comparables.

Representa el núcleo metodológico del laboratorio.

---

## Motor Analítico

Integra observaciones.

Construye históricos.

Calcula indicadores.

Genera series temporales.

---

## Motor Territorial

Relaciona las observaciones con información espacial.

Integra.

* barrios;
* radios censales;
* circuitos;
* infraestructura;
* indicadores públicos.

---

## Motor de Pronóstico

Transforma indicadores en escenarios probables.

No produce comunicación.

Produce evidencia.

---

## Motor de Comunicación

Transforma el pronóstico en recomendaciones para la comunicación política.

No toma decisiones.

Las asiste.

---

# 5. Bases de información

El laboratorio trabaja con dos grandes bases.

## Base Operacional

Contiene.

* estaciones;
* observaciones;
* respuestas;
* eventos.

Representa el presente.

---

## Base Analítica

Contiene.

* históricos;
* indicadores;
* agregaciones;
* pronósticos.

Representa el conocimiento acumulado.

---

# 6. Productos

La arquitectura genera dos productos distintos.

## Producto A

La comunidad.

Recibe.

* mapas;
* indicadores;
* conocimiento colectivo.

Su objetivo es fortalecer la red.

---

## Producto B

El Servicio Meteorológico Social.

Produce.

* análisis;
* pronósticos;
* recomendaciones.

Su objetivo es asistir procesos de comunicación.

---

# 7. Escalabilidad

La arquitectura fue diseñada para crecer.

Primero.

Barrio.

↓

Municipio.

↓

Provincia.

↓

País.

↓

Red internacional.

La arquitectura no cambia.

Únicamente aumenta la cantidad de estaciones.

---

# 8. Principios

Toda decisión tecnológica deberá respetar estos principios.

## El método tiene prioridad sobre la tecnología.

---

## La comunidad tiene prioridad sobre el modelo.

---

## El conocimiento tiene prioridad sobre el dato.

---

## La observación tiene prioridad sobre la interpretación.

---

## La devolución tiene prioridad sobre la extracción.

---

## Toda observación debe poder reconstruir su recorrido completo.

---

## Regla de diseño

La arquitectura deberá permanecer válida incluso si cambia completamente la tecnología utilizada para implementarla.

El método constituye el verdadero producto del laboratorio.
