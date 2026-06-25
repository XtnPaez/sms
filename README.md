# Servicio Meteorológico Social

> Laboratorio para el diseño y validación de un método reproducible de producción de evidencia territorial distribuida.

El Servicio Meteorológico Social (SMS) es un laboratorio de investigación cuyo objetivo consiste en estudiar si una red distribuida de estaciones puede producir evidencia territorial suficiente para identificar fenómenos emergentes y construir pronósticos útiles para la toma de decisiones.

El principal producto del laboratorio no será una aplicación informática.

Será un método capaz de sobrevivir a cualquier implementación tecnológica.

---

# Cómo leer este repositorio

Los documentos están organizados según el ciclo de construcción del conocimiento.

No según la tecnología utilizada.

Cada carpeta responde una pregunta diferente.

```text
00_meta
¿Cómo se mantiene el laboratorio?

01_laboratorio
¿Por qué existe el laboratorio?

02_metodo
¿Cómo funciona el método?

03_experimentos
¿Qué evidencia produjo el laboratorio?

04_bibliografia
¿Qué conocimiento previo utilizamos?

99_material
Material de apoyo.
```

---

# Estructura

```text
sms/

├── README.md

├── 00_meta/
│   ├── CHANGELOG.md
│   ├── IDEAS.md
│   ├── REGLAS_DEL_LABORATORIO.md
│   └── TODO.md

├── 01_laboratorio/
│   ├── acta_fundacional.md
│   ├── manifiesto.md
│   ├── fundamentos.md
│   ├── glosario.md
│   ├── estado_del_arte.md
│   ├── proyecto_diplomatura.md
│   ├── masterplan.md
│   ├── preguntas.md
│   ├── decisiones.md
│   └── going_nowhere.md

├── 02_metodo/
│   ├── roadmap.md
│   ├── protocolo_estaciones.md
│   ├── modelo_informacion.md
│   ├── arquitectura_del_sistema.md
│   ├── metricas.md
│   └── stack_tecnologico.md

├── 03_experimentos/

├── 04_bibliografia/

└── 99_material/
```

---

# Cómo trabajar en este repositorio

Antes de crear un documento nuevo.

Preguntarse si realmente responde una pregunta diferente.

Antes de agregar un concepto nuevo.

Verificar si puede explicarse utilizando los conceptos existentes.

Antes de modificar un documento.

Comprobar si el cambio corresponde realmente a ese documento.

Si modifica la teoría o el método.

Reemplazar la versión completa del documento.

No agregar parches.

---

# Principios del laboratorio

* El método tiene prioridad sobre la tecnología.
* La evidencia tiene prioridad sobre la opinión.
* La comunidad tiene prioridad sobre el dato.
* Los experimentos tienen prioridad sobre las funcionalidades.
* La simplicidad tiene prioridad sobre la complejidad.

---

# Estado actual

El laboratorio se encuentra finalizando la construcción de su marco metodológico.

La siguiente etapa consiste en obtener evidencia mediante el primer experimento de campo.

El estado de evolución del método puede consultarse en:

`02_metodo/roadmap.md`

---

# Hipótesis central

Una red distribuida de estaciones que realiza observaciones territoriales siguiendo un protocolo común puede producir evidencia suficiente para identificar fenómenos emergentes y construir pronósticos territoriales antes de que esos fenómenos se consoliden como agenda pública.

La validez de esta hipótesis deberá establecerse experimentalmente.

---

# Licencia

Por definir.
