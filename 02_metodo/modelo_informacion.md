# Modelo de Información

> Este documento define las entidades conceptuales del Servicio Meteorológico Social y las relaciones entre ellas. No describe una base de datos específica. Describe la información que el método necesita producir, conservar y transformar.

---

# Índice

1. Objetivo
2. Filosofía
3. Entidades principales
4. Relaciones
5. Ciclo de vida de la información
6. Niveles de agregación
7. Histórico
8. Capas territoriales
9. Productos derivados
10. Preguntas abiertas

---

# 1. Objetivo

Toda observación realizada por una estación debe transformarse, mediante un proceso gradual de integración, en conocimiento útil para el laboratorio.

Este documento define ese recorrido.

No modela tablas.

Modela conocimiento.

---

# 2. Filosofía

El laboratorio trabaja con una idea simple.

**Los datos nunca existen aislados.**

Cada dato forma parte de un contexto.

Ese contexto es el que permite construir conocimiento.

Por esa razón el método no almacena únicamente observaciones.

Almacena relaciones.

---

# 3. Entidades principales

## Estación

Produce observaciones.

---

## Observación

Unidad mínima del método.

Toda observación posee:

* tiempo
* territorio
* estación
* contenido

---

## Territorio

Lugar al cual pertenece la observación.

Puede representarse mediante distintas unidades.

* barrio
* radio censal
* circuito
* comuna
* localidad
* municipio

---

## Tema

Clasificación temática de una observación.

No necesariamente coincide con la forma en que fue registrada.

---

## Pronóstico

Resultado del procesamiento de múltiples observaciones.

Nunca proviene de una sola estación.

---

## Recomendación

Interpretación comunicacional del pronóstico.

Constituye el producto final del método.

---

# 4. Relaciones

```text
ESTACIÓN

↓

OBSERVACIÓN

↓

TEMA

↓

TERRITORIO

↓

SERIE TEMPORAL

↓

PRONÓSTICO

↓

RECOMENDACIÓN
```

El laboratorio nunca trabaja con observaciones aisladas.

Siempre trabaja con relaciones.

---

# 5. Ciclo de vida de la información

```text
Observación

↓

Clasificación

↓

Georreferenciación

↓

Histórico

↓

Agregación

↓

Indicadores

↓

Pronóstico

↓

Recomendación
```

Cada etapa agrega contexto.

Nunca reemplaza información.

---

# 6. Niveles de agregación

Una misma observación podrá analizarse en distintos niveles.

Individual.

↓

Barrio.

↓

Comuna.

↓

Municipio.

↓

Provincia.

↓

Región.

↓

País.

El método deberá permitir cambiar de escala sin perder consistencia.

---

# 7. Histórico

Toda observación permanece.

Nunca se reemplaza.

Nunca se corrige.

Los modelos cambian.

Los datos originales permanecen.

El histórico constituye uno de los principales activos del laboratorio.

---

# 8. Capas territoriales

Las observaciones pueden enriquecerse mediante capas externas.

Ejemplos.

## Demografía

* población
* edad
* hogares

---

## Infraestructura

* escuelas
* hospitales
* clubes
* plazas

---

## Condiciones sociales

* pobreza
* empleo
* conectividad

---

## Política

* resultados electorales
* participación
* representación territorial

---

## Ambiente

* clima
* inundaciones
* espacios verdes

---

Estas capas no generan observaciones.

Las contextualizan.

---

# 9. Productos derivados

El laboratorio podrá producir distintos niveles de información.

## Datos

Observaciones.

---

## Información

Observaciones organizadas.

---

## Indicadores

Series temporales.

---

## Conocimiento

Patrones.

---

## Pronósticos

Escenarios probables.

---

## Recomendaciones

Sugerencias para la comunicación política.

---

# 10. Preguntas abiertas

* ¿Qué información nunca debe perderse?
* ¿Qué parte pertenece al dato y cuál al modelo?
* ¿Qué procesos deben ser reproducibles?
* ¿Qué capas territoriales producen mayor capacidad explicativa?
* ¿Qué información puede publicarse y cuál debe permanecer privada?

---

# Nota

Este documento es deliberadamente independiente de cualquier tecnología.

La implementación podrá realizarse en PostgreSQL, PostGIS u otro sistema.

Si el método cambia de plataforma, este documento debería permanecer prácticamente igual.
