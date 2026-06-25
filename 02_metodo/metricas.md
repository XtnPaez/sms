# Métricas

> Este documento define cómo evaluaremos el funcionamiento del Servicio Meteorológico Social. Las métricas no buscan medir únicamente el software. Buscan medir la calidad del método.

---

# Índice

1. Objetivo
2. Filosofía
3. Métricas de Comunidad
4. Métricas de Cobertura
5. Métricas de Observación
6. Métricas del Modelo
7. Métricas del Pronóstico
8. Métricas de Comunicación
9. Indicadores derivados
10. Evolución de las métricas

---

# 1. Objetivo

Todo experimento necesita una forma de evaluar sus resultados.

El Servicio Meteorológico Social no medirá únicamente cantidad de usuarios o cantidad de respuestas.

Su objetivo principal consiste en evaluar si el método logra producir conocimiento útil.

---

# 2. Filosofía

Una métrica nunca constituye un objetivo.

Las métricas existen para comprender mejor el comportamiento del sistema y facilitar la toma de decisiones.

Cuando una métrica deja de producir conocimiento, debe ser revisada o eliminada.

---

# 3. Métricas de Comunidad

## Cantidad de estaciones

Número total de estaciones registradas.

---

## Estaciones activas

Cantidad de estaciones que realizaron al menos una observación durante el período analizado.

---

## Permanencia

Tiempo promedio de permanencia de una estación dentro de la red.

---

## Retención

Porcentaje de estaciones que continúan participando después de:

* 1 semana
* 1 mes
* 3 meses
* 6 meses

---

## Incorporación

Cantidad de nuevas estaciones por período.

---

# 4. Métricas de Cobertura

## Cobertura territorial

Porcentaje del territorio que posee al menos una estación.

---

## Densidad

Cantidad de estaciones por unidad territorial.

---

## Vacíos

Territorios sin observaciones.

---

## Redundancia

Territorios con exceso de estaciones respecto del promedio.

---

# 5. Métricas de Observación

## Frecuencia

Cantidad promedio de observaciones por estación.

---

## Continuidad

Cantidad de períodos consecutivos con participación.

---

## Diversidad temática

Cantidad de temas diferentes observados por una estación.

---

## Consistencia

Grado de estabilidad de una estación a lo largo del tiempo.

---

## Correlación

Coincidencia entre observaciones realizadas por estaciones cercanas.

---

# 6. Métricas del Modelo

## Tiempo de procesamiento

Tiempo necesario para transformar observaciones en indicadores.

---

## Cobertura temática

Cantidad de temas detectados.

---

## Señales débiles

Cantidad de fenómenos detectados antes de consolidarse.

---

## Latencia

Tiempo transcurrido entre la aparición de una conversación y su detección por el modelo.

---

# 7. Métricas del Pronóstico

## Anticipación

¿Cuántos días antes detectó el fenómeno?

---

## Precisión

Grado de coincidencia entre el pronóstico y la evolución posterior.

---

## Confianza

Nivel de evidencia disponible para construir el pronóstico.

---

## Persistencia

Cantidad de períodos consecutivos durante los cuales un mismo fenómeno permanece activo.

---

# 8. Métricas de Comunicación

## Recomendaciones emitidas

Cantidad de recomendaciones producidas.

---

## Recomendaciones utilizadas

Cantidad de recomendaciones efectivamente adoptadas por el usuario.

---

## Utilidad percibida

Evaluación cualitativa realizada por el consultor.

---

# 9. Indicadores derivados

A futuro podrán desarrollarse indicadores como:

* Temperatura Social
* Presión Social
* Índice de Incertidumbre
* Índice de Cobertura
* Índice de Participación
* Índice de Confianza
* Índice de Actividad Territorial

Estos indicadores deberán documentarse individualmente antes de incorporarse al método.

---

# 10. Evolución de las métricas

Las métricas constituyen parte del método.

Podrán modificarse a medida que avance el laboratorio.

Toda incorporación, modificación o eliminación deberá quedar registrada en **decisiones.md**.

---

# Principio general

El éxito del laboratorio no dependerá del tamaño de la comunidad.

Dependerá de su capacidad para producir conocimiento útil, reproducible y territorialmente consistente.
