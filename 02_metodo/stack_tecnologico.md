# Stack Tecnológico

> Este documento describe la implementación tecnológica del laboratorio. Ninguna de las herramientas aquí mencionadas forma parte del método. Todas podrán cambiar sin modificar la esencia del Servicio Meteorológico Social.

---

# Índice

1. Filosofía
2. Infraestructura
3. Comunicación
4. Persistencia
5. Procesamiento
6. Inteligencia Artificial
7. Visualización
8. Desarrollo
9. Automatización
10. Principios del stack
11. Evolución

---

# 1. Filosofía

El método tiene prioridad sobre la tecnología.

Cada herramienta existe únicamente porque resuelve un problema concreto.

Nunca se incorpora tecnología "por las dudas".

Toda incorporación deberá responder una pregunta sencilla.

> ¿Qué problema resuelve?

---

# 2. Infraestructura

## Notebook dedicada

Todo el laboratorio se desarrollará sobre una computadora dedicada exclusivamente al proyecto.

Objetivos.

* mantener un entorno limpio;
* facilitar reproducibilidad;
* aislar experimentos;
* simplificar backups.

---

## Teléfono dedicado

Un único teléfono para el laboratorio.

Permitirá separar la identidad del proyecto de las cuentas personales.

---

## Chip dedicado

Número exclusivo para el laboratorio.

Permitirá operar WhatsApp Business y otros servicios futuros.

---

# 3. Comunicación

## WhatsApp Business

Será la primera plataforma de interacción con las estaciones.

Funciones previstas.

* Comunidad.
* Canales.
* Listas de difusión.
* Automatización.
* Respuestas rápidas.

---

## Instagram

Canal de descubrimiento.

No será utilizado para registrar observaciones.

Su objetivo será atraer nuevas estaciones.

---

## Correo electrónico

Reservado para documentación y comunicaciones institucionales.

---

# 4. Persistencia

## Git

Repositorio privado.

Documentación.

Código.

Método.

Experimentación.

---

## GitHub

Control de versiones.

Gestión del conocimiento.

---

## PostgreSQL

Base principal del laboratorio.

---

## PostGIS

Modelo territorial.

Toda observación tendrá referencia espacial.

---

# 5. Procesamiento

Python.

SQL.

Scripts de automatización.

Procesamiento espacial.

Series temporales.

Generación de indicadores.

---

# 6. Inteligencia Artificial

La IA no constituye un requisito del MVP.

Será incorporada únicamente cuando exista un problema claramente identificado.

Posibles usos.

* clasificación temática;
* resumen automático;
* agrupamiento;
* generación de informes;
* asistencia al consultor;
* detección de patrones.

---

# 7. Visualización

Dashboard.

Mapas.

Series temporales.

Indicadores.

Pronósticos.

No se prioriza el diseño visual.

Se prioriza la comprensión.

---

# 8. Desarrollo

Lenguaje principal.

Python.

Base espacial.

PostgreSQL + PostGIS.

API.

REST.

Repositorio.

GitHub.

---

# 9. Automatización

Objetivos.

* reducir tareas repetitivas;
* minimizar errores manuales;
* acelerar procesamiento;
* mantener trazabilidad.

Toda automatización deberá documentarse.

---

# 10. Principios del Stack

## Simplicidad

La solución más simple tiene prioridad.

---

## Reproducibilidad

Todo el laboratorio debe poder instalarse nuevamente siguiendo la documentación.

---

## Bajo costo

El laboratorio buscará minimizar costos de infraestructura.

---

## Software abierto

Siempre que resulte posible se priorizarán herramientas abiertas.

---

## Modularidad

Toda herramienta debe poder reemplazarse sin afectar el método.

---

## Trazabilidad

Todo dato debe poder reconstruir su recorrido.

---

# 11. Evolución

El stack tecnológico evolucionará junto con el laboratorio.

No existe compromiso permanente con ninguna herramienta.

La única obligación del stack consiste en implementar correctamente el método.

---

# Stack inicial (MVP)

## Hardware

* Notebook dedicada
* Teléfono Android
* Chip exclusivo

---

## Comunicación

* WhatsApp Business
* Instagram

---

## Persistencia

* Git
* GitHub
* PostgreSQL
* PostGIS

---

## Desarrollo

* Python
* SQL
* Visual Studio Code

---

## Visualización

* QGIS
* Leaflet
* Dashboard web

---

## Documentación

* Markdown
* GitHub

---

# Regla de oro

El día que una tecnología limite la evolución del método, deberá reemplazarse.

Nunca al revés.
