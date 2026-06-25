# Stack Tecnológico

> Este documento describe la infraestructura tecnológica utilizada por el Servicio Meteorológico Social.

No define el método.

No define la arquitectura conceptual.

Describe únicamente una posible implementación tecnológica del laboratorio.

---

# Índice

1. Propósito
2. Principios
3. Capacidades del laboratorio
4. Implementación actual
5. Evolución tecnológica
6. Regla editorial

---

# 1. Propósito

El laboratorio necesita determinadas capacidades tecnológicas para funcionar.

Cada capacidad podrá implementarse mediante distintas herramientas.

Por esa razón, el método nunca deberá depender de una tecnología específica.

---

# 2. Principios

La selección tecnológica seguirá los siguientes principios.

* simplicidad;
* software libre cuando resulte posible;
* interoperabilidad;
* bajo costo;
* reemplazabilidad;
* documentación completa.

La incorporación de una nueva herramienta deberá resolver un problema concreto.

Nunca incorporarse únicamente por novedad tecnológica.

---

# 3. Capacidades del laboratorio

## Captura

Permite registrar observaciones.

Implementación actual.

* WhatsApp Business.

Posibles implementaciones futuras.

* aplicación móvil;
* formularios web;
* correo electrónico;
* APIs;
* otros sistemas de mensajería.

---

## Persistencia

Permite almacenar la información producida por el laboratorio.

Implementación actual.

* PostgreSQL.

Posibles implementaciones futuras.

* otras bases de datos compatibles.

---

## Espacial

Permite representar la información territorialmente.

Implementación actual.

* PostGIS.

---

## Procesamiento

Permite transformar observaciones en eventos, fenómenos e indicadores.

Implementación actual.

* SQL;
* scripts de automatización.

Posibles implementaciones futuras.

* motores analíticos;
* procesamiento distribuido.

---

## Publicación

Permite devolver conocimiento hacia la comunidad.

Implementación actual.

* mapas web;
* informes;
* tableros.

---

## Visualización

Permite interpretar la evidencia.

Implementación actual.

* Leaflet;
* QGIS.

Posibles implementaciones futuras.

* dashboards;
* aplicaciones específicas.

---

## Versionado

Permite documentar la evolución del laboratorio.

Implementación actual.

* Git;
* GitHub.

---

## Automatización

Permite reducir tareas repetitivas.

Implementación actual.

* scripts;
* tareas programadas.

Posibles implementaciones futuras.

* inteligencia artificial;
* agentes especializados.

---

# 4. Implementación actual

Infraestructura prevista para el MVP.

## Hardware

* notebook dedicada;
* teléfono exclusivo;
* chip exclusivo.

---

## Software

* WhatsApp Business;
* PostgreSQL;
* PostGIS;
* Git;
* GitHub;
* QGIS;
* Visual Studio Code.

---

## Documentación

Toda la documentación se mantiene en formato Markdown dentro del repositorio del laboratorio.

---

# 5. Evolución tecnológica

La tecnología evolucionará únicamente cuando la evidencia experimental demuestre que una nueva herramienta mejora el funcionamiento del método.

La incorporación de una nueva tecnología deberá responder explícitamente.

* ¿Qué problema resuelve?
* ¿Qué capacidad mejora?
* ¿Qué complejidad agrega?
* ¿Puede reemplazarse en el futuro?

Si estas preguntas no pueden responderse claramente, la incorporación deberá postergarse.

---

# 6. Regla editorial

Este documento describe una implementación posible.

No constituye parte del método.

Si una tecnología cambia y el método permanece válido, el laboratorio habrá sido correctamente diseñado.

El verdadero producto del Servicio Meteorológico Social no será su infraestructura tecnológica.

Será el método capaz de sobrevivir a cualquier infraestructura.
