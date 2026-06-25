# Modelo de Información

> Este documento describe cómo el Servicio Meteorológico Social transforma observaciones distribuidas en conocimiento territorial.

No representa un modelo de base de datos.

No representa un modelo UML.

Representa el modelo conceptual del laboratorio.

---

# Índice

1. Propósito
2. Principios
3. Ciclo de transformación
4. Componentes del modelo
5. Relaciones
6. Productos del modelo
7. Regla editorial

---

# 1. Propósito

El laboratorio no produce conocimiento de manera directa.

Produce observaciones.

El conocimiento aparece como consecuencia de un proceso de integración.

Este documento describe ese proceso.

---

# 2. Principios

El modelo sigue los siguientes principios.

* cada componente cumple una única función;
* cada transformación agrega valor;
* ninguna etapa puede omitirse;
* todo resultado debe ser trazable hasta las observaciones originales.

---

# 3. Ciclo de transformación

```text
ESTACIÓN

↓

OBSERVACIÓN

↓

EVENTO

↓

FENÓMENO

↓

INDICADOR

↓

PRONÓSTICO

↓

RECOMENDACIÓN
```

Cada componente representa un nivel diferente de elaboración del conocimiento.

El laboratorio no produce recomendaciones directamente.

Las construye recorriendo todas las etapas anteriores.

---

# 4. Componentes del modelo

## 4.1 Estación

Origen de toda observación.

Una estación representa un punto permanente de observación del territorio.

Produce observaciones.

No produce conocimiento.

---

## 4.2 Observación

Registro primario realizado por una estación.

Representa un hecho localizado espacial y temporalmente.

Las observaciones constituyen la materia prima del laboratorio.

---

## 4.3 Evento

Agrupación de observaciones que describen una misma ocurrencia.

Los eventos permiten organizar la información sin interpretarla todavía como un fenómeno.

Representan el primer nivel de integración.

---

## 4.4 Fenómeno

Patrón identificado a partir de múltiples eventos.

Un fenómeno representa una regularidad territorial.

Su existencia depende de la evidencia acumulada.

Los fenómenos constituyen el principal objeto de estudio del laboratorio.

---

## 4.5 Indicador

Medida obtenida mediante el análisis de uno o más fenómenos.

Los indicadores permiten comparar.

No interpretan.

No recomiendan.

Describen.

---

## 4.6 Pronóstico

Estimación probabilística sobre la evolución futura de uno o más fenómenos.

Todo pronóstico deberá indicar.

* territorio;
* período;
* nivel de confianza;
* evidencia utilizada.

---

## 4.7 Recomendación

Aplicación práctica de un pronóstico.

Las recomendaciones no pertenecen al método científico.

Constituyen un posible uso del conocimiento producido.

Diferentes actores podrán formular recomendaciones distintas utilizando la misma evidencia.

---

# 5. Relaciones

```text
Una estación

produce

muchas observaciones

↓

Muchas observaciones

pueden formar

un evento

↓

Muchos eventos

pueden revelar

un fenómeno

↓

Uno o más fenómenos

permiten calcular

indicadores

↓

Los indicadores

permiten construir

pronósticos

↓

Los pronósticos

permiten elaborar

recomendaciones
```

Cada transformación conserva la posibilidad de reconstruir completamente el recorrido inverso.

Toda recomendación deberá poder rastrearse hasta las observaciones originales que la hicieron posible.

La trazabilidad constituye un principio fundamental del laboratorio.

---

# 6. Productos del modelo

El modelo genera tres tipos de productos.

## Evidencia

Compuesta por:

* observaciones;
* eventos;
* fenómenos;
* indicadores.

---

## Conocimiento

Representado por los pronósticos.

---

## Aplicación

Representada por las recomendaciones.

Esta separación evita confundir evidencia con decisiones.

---

# 7. Regla editorial

Toda modificación del método deberá ser consistente con este modelo.

Si un nuevo concepto no puede ubicarse claramente dentro del ciclo de transformación, deberá justificarse su incorporación o descartarse.

Este documento constituye el modelo conceptual oficial del Servicio Meteorológico Social.

Toda implementación tecnológica deberá adaptarse a él y no al revés.
