# Servicio Meteorológico Social (SMS)

> **Laboratorio para el diseño, implementación y validación de un método de observación territorial distribuida capaz de producir evidencia, pronósticos y recomendaciones para la toma de decisiones.**

---

# ¿Qué es este repositorio?

Este repositorio documenta el desarrollo del **Servicio Meteorológico Social (SMS)**.

No es un proyecto de software.

No es una tesis.

No es únicamente un trabajo para una diplomatura.

Es el cuaderno de laboratorio donde registramos el proceso de diseño de un método experimental para transformar observaciones territoriales distribuidas en conocimiento colectivo.

El primer caso de aplicación del método será la **comunicación política**, pero el laboratorio está concebido para ser reutilizable en otros dominios donde resulte necesario comprender la evolución de conversaciones territoriales.

---

# Hipótesis general

Así como una red de estaciones meteorológicas permite anticipar la evolución del clima físico, una red distribuida de observadores territoriales podría anticipar la evolución de fenómenos sociales.

El objetivo del laboratorio consiste en comprobar si esa hipótesis resiste el contacto con la realidad.

---

# Filosofía

El laboratorio se apoya sobre algunos principios simples.

* Escuchar antes de comunicar.
* Observar antes de interpretar.
* Documentar antes de concluir.
* Experimentar antes de afirmar.
* Construir método antes que tecnología.

La tecnología podrá cambiar.

El método no.

---

# Estado actual del laboratorio

```text
████████░░░░░░░░░░░░░░░░░░

Fundamentos               ✓
Modelo conceptual         ✓
Método                    ✓

Infraestructura           □
Experimentos              □
Piloto                    □
Validación                □
Producto                  □
Escalabilidad             □
```

El objetivo actual consiste en construir y validar el primer experimento de campo.

---

# Cómo recorrer este repositorio

Los documentos fueron organizados siguiendo el ciclo natural de construcción del conocimiento.

Se recomienda recorrerlos en el siguiente orden.

```text
MANIFIESTO

↓

FUNDAMENTOS

↓

GLOSARIO

↓

ESTADO DEL ARTE

↓

PROYECTO DIPLOMATURA

↓

MASTERPLAN

↓

MÉTODO

↓

EXPERIMENTOS
```

Cada documento responde una pregunta distinta.

---

## Manifiesto

¿Por qué vale la pena intentar construir un Servicio Meteorológico Social?

---

## Fundamentos

¿Cómo nació la idea?

¿Qué analogías la inspiraron?

¿Qué hipótesis pretende poner a prueba?

---

## Glosario

Define el lenguaje utilizado por el laboratorio.

Todo concepto nuevo debería aparecer primero aquí.

---

## Estado del Arte

Describe qué métodos existen actualmente para producir evidencia territorial y cuál es el aporte diferencial del laboratorio.

---

## Proyecto Diplomatura

Representa el recorte experimental que será desarrollado durante la diplomatura.

No describe el alcance completo del laboratorio.

---

## Masterplan

Reúne todas las ideas que exceden el MVP.

Su función es conservar oportunidades futuras sin alterar el rumbo del experimento principal.

---

## Método

Describe el funcionamiento del Servicio Meteorológico Social.

Aquí se encuentran:

* roadmap;
* protocolo de estaciones;
* modelo de información;
* métricas;
* arquitectura;
* stack tecnológico.

---

## Experimentos

Toda hipótesis debe validarse mediante experimentos.

Cada prueba, exitosa o fallida, forma parte del conocimiento del laboratorio.

---

# Cómo trabajar en este repositorio

Este laboratorio utiliza algunas reglas simples.

* Una idea vive en un único lugar.
* Las hipótesis no son conclusiones.
* Toda decisión importante queda registrada.
* Los caminos descartados también producen conocimiento.
* Antes de modificar un documento, verificar si la idea pertenece realmente a ese documento.
* El MVP tiene prioridad sobre cualquier expansión futura.
* Ningún documento está terminado.

---

# Estructura

```text
README.md

00_meta/
    CHANGELOG.md
    TODO.md
    IDEAS.md
    REGLAS_DEL_LABORATORIO.md

01_laboratorio/
    manifiesto.md
    fundamentos.md
    glosario.md
    estado_del_arte.md
    proyecto_diplomatura.md
    masterplan.md
    preguntas.md
    decisiones.md
    going_nowhere.md

02_metodo/
    roadmap.md
    protocolo_estaciones.md
    modelo_informacion.md
    arquitectura_del_sistema.md
    metricas.md
    stack_tecnologico.md

03_experimentos/

04_bibliografia/

05_material/
```

---

# Qué entendemos por éxito

El éxito del laboratorio no consiste en desarrollar una aplicación.

Tampoco consiste en construir una comunidad grande.

El éxito consistirá en responder una pregunta.

> ¿Es posible diseñar un método reproducible para transformar observaciones territoriales distribuidas en evidencia útil para anticipar la evolución del clima social?

Si la respuesta es afirmativa, el laboratorio habrá producido un nuevo método.

Si la respuesta es negativa, el laboratorio habrá producido conocimiento igualmente valioso.

Ambos resultados justifican el experimento.

---

# Principio editorial

Este repositorio documenta la evolución de un método.

Los documentos no representan versiones definitivas.

Representan el estado del conocimiento alcanzado en cada momento del laboratorio.

Por esa razón, la documentación constituye parte del experimento y no únicamente su registro.

---

# Licencia intelectual del laboratorio

El conocimiento aquí documentado deberá poder ser comprendido, reproducido, criticado y mejorado.

La mayor contribución del Servicio Meteorológico Social no será una herramienta informática.

Será un método para producir evidencia territorial distribuida.
