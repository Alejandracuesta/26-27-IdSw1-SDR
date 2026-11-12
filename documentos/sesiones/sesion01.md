<!--
  PLANTILLA DE SESIÓN DE REQUISITADO · GRUPO 4
  ============================================
  Cómo usarla:
  1. Copia este archivo como `sesionNN.md` (sesion02.md, sesion03.md…).
  2. Sustituye todo lo que va entre <ANGULOS>.
  3. Borra los apartados que no apliquen en esa sesión, salvo 1, 2, 3, 9 y 10, que van siempre.
  4. Los comentarios como este no se ven en GitHub; puedes dejarlos o borrarlos.

  Convenciones (mantenerlas en todas las sesiones):
  - IDs de requisitos continuos entre sesiones: si la sesión 1 acabó en RF-24, la siguiente empieza en RF-25.
    Nunca se reutiliza un ID; si un requisito se descarta, se marca X y se deja.
  - Etiquetas de origen:  C = confirmado · P = propuesto · Q = pendiente · X = descartado
  - Evidencia: minuto de la grabación (mm:ss–mm:ss) o cita literal del cliente.
  - Lo que decide el grupo (D-xx) nunca se presenta como si lo hubiera pedido el cliente.
  - Diagramas: fuente en `modelosUML/sesionNN-nombre.puml` y SVG en `imagenes/sesionNN-nombre.svg`.
-->

# SESIÓN 01:
### 27/10/2026

<div align=center>

| | |
|-|-|
| **Tipo** | Reunión extra |
| **Cliente** | Jose Manuel Breñosa |
| **Grupo** | 4 |
| **Coordinación** | @Alejandracuesta |
| **Redacta el acta** | Alejandra Cuesta |
| **Duración** | 12:15 – 13:30 |
| **Grabación** | Sí  · [transcript](../sesiones/transcripts/sesion01.md) |

</div>

## Índice

1. [Asistencia](#1-asistencia)
2. [Objetivo de la sesión](#2-objetivo-de-la-sesión)
3. [Respuestas a las preguntas pendientes](#3-respuestas-a-las-preguntas-pendientes)
4. [Información nueva del cliente](#4-información-nueva-del-cliente)
5. [Cambios en los requisitos](#5-cambios-en-los-requisitos)
6. [Cambios en el alcance](#6-cambios-en-el-alcance)
7. [Modelado](#7-modelado)
8. [Glosario: términos nuevos o corregidos](#8-glosario-términos-nuevos-o-corregidos)
9. [Preguntas para la próxima sesión](#9-preguntas-para-la-próxima-sesión)
10. [Acuerdos y tareas del grupo](#10-acuerdos-y-tareas-del-grupo)

---

## 1. Asistencia

<!-- Regla de la asignatura: si asiste menos del 80 % del grupo (menos de 6 de 7), la reunión se cancela. -->

<div align=center>

| Integrante | Asiste |
|-|:-:|
| Alejandra Cuesta | SÍ |
| Ismael Cobo | SÍ |
| Alejandro de la Peña | SÍ |
| Juan Carlos Quintana | SÍ |
| José Luis de la Asunción | SÍ |
| Emilio Muciño | SÍ |
| Daniel Cotarelo | SÍ |
| **Total** | **7/7 (100%)** |

</div>

## 2. Objetivo de la sesión

<!-- Qué queríamos conseguir al entrar a la reunión. Una o dos frases. -->
Escuchar y tomar apuntes de los requisitos del cliente.

**Material que llevamos:**
- Ordenador para apuntar requisitos.
- Grabadora de audio.

## 3. Respuestas a las preguntas pendientes

<!--
  Copiar aquí las preguntas del apartado 9 de la sesión anterior y apuntar la respuesta.
  Estado: ✅ resuelta · 🔶 parcial · ⏳ sin tratar (pasa a la siguiente sesión)
  Impacto: qué requisito, regla o clase cambia por la respuesta.
-->

| Nº | Pregunta (sesión <NN-1>) | Respuesta del cliente | Estado | Impacto |
|:-:|-|-|:-:|-|
| 1 | ¿Cuál es el proyecto que nos planteas? | Planificación de Tareas | ✅ | Ninguno |
| 2 | ¿Hace falta diferenciar entre festivo o día de la universidad? ¿O entre no lectivo y lectivo? | Hace falta, para explicar a los profesores: festivo, no lectivo y laborable.| ✅ | Ninguno |
| 3 | ¿Pueden haber investigadores solos, tal cual, o solo profesor investigador y profesor tal cual? | Podría haberlos, pero no es el caso de esta universidad, que yo sepa. Aquí todo el mundo da clases.| ✅ | Ninguno |
| 4 | ¿Qué más cosas quieres que tenga el analizador? | Se le mete, de alguna forma, el calendario del curso. | ✅ | Ninguno |
| 5 | ¿Y se las hacemos para que sea configurable para cada profesor? | Sí, eso es. | ✅ | Ninguno |
| 6 | ¿Tienes posibilidad de importar también las clases, los horarios dentro de cualquier calendario? | Sí, pero mirándolo como que lo va a hacer una vez al cuatrimestre, lo puede hacer el docente a mano y no tenéis que implementar nada especial. | ✅ | Ninguno |

## 4. Información nueva del cliente

<!--
  Lo que el cliente contó por primera vez en esta sesión, agrupado por temas.
  Incluir citas literales cuando aporten matiz: > *"cita"* (mm:ss)
  Borrar los temas que no salieron.
-->

### 4.1. Qué quiere el cliente

Quiere una aplicación que le organice su día a día como profesor: al llegar por la mañana, ver qué tiene que hacer y en qué orden. No es lo mismo que el planificador de Manuel Masías, que sirve para la planificación general del cuatrimestre y está pensado para la universidad. Este es para el profesor.

> *"Llegar, ver mi planificador y decir: «Hoy tengo: primero, leer email; segundo, preparar clase; tercero, reunión de coordinación con no sé qué; cuarto, tutoría de no sé cuánto»."*(02:56)

Nos pidió centrarnos en Informática y en su caso personal:

> *"A mí lo que me interesa es que funcione para mí."*  (11:46).

### 4.2. Profesor

En esta universidad todos los profesores son también investigadores, así que tienen dos tipos de tareas: las de docencia y las de investigación o proyectos.

> *"Podría haberlos [solo investigadores], pero no es el caso de esta universidad… Aquí todo el mundo da clases."* (04:01)

### 4.3. Calendario

Hay que distinguir tres tipos de día:

- Festivo: No se trabaja y no se planifica nada.
- No lectivo (por ejemplo, el día de la universidad): se trabaja, pero no hay clases. Las clases de ese día se cancelan.
- Lectivo: Se trabaja y hay clases.
> *"El calendario se saca del que publica la universidad. Se puede meter a mano o desde un archivo"* (04:35–05:17).

### 4.4. Horario de trabajo

Cada profesor tiene su propio horario de entrada y salida. Nos explicó las reglas de RRHH (37,5 horas a la semana, máximo 9 horas al día, descanso obligatorio), pero nos pidió no tenerlas en cuenta. Basta con que cada profesor meta su horario.

> *"Para vosotros es más fácil que el docente diga cuáles son sus horarios de trabajo cada día. O sea, que os lo meta a mano o en un Excel."* (06:40).

### 4.5. Clases

- El horario de clases lo pone Ordenación Académica y no se puede cambiar.
> *"El profesor lo mete a mano una vez por cuatrimestre"* (07:23–07:59).
- Si el profesor se pone enfermo y no puede dar una clase, tiene que recuperarla (07:45).
- Hay tipos de clase: teoría, ejercicios, teórico-práctica, laboratorio y prácticas con ordenador (09:03).
- Hay tipos de aula: aula normal con proyector, aula de ordenadores y laboratorio (11:12).
- La reserva de aulas no es cosa nuestra: ya la lleva Ordenación Académica (10:00–10:23).

### 4.6. Antes, durante y después de cada clase

Para el cliente, las clases son "lo realmente importante de cada docencia" (12:04). 
Alrededor de cada clase hay trabajo:

- Antes: preparar o revisar el material y los ejercicios.
- Durante: comprobar que el material esté disponible.
- Después: tareas como programar en Campus la entrega de unos deberes (12:40–12:51).
- Hay que distinguir las tareas dentro del aula de las de fuera del aula. Las de investigación siempre son fuera (08:24–08:49).

### 4.7. Los recursos

Cada clase necesita recursos: el material, los ejercicios o un aula con ordenadores. El cliente quiere poder anotarlos y enlazar carpetas de su Google Drive (10:32 · 13:37 · 24:26).

### 4.8. Tipos de tareas e imprevistos

- Tareas que tiene un profesor: emails, tutorías, reuniones, encuestas, exámenes, programar tareas y quizzes en Campus… (13:48).

- Algunas aparecen sin avisar, como las tutorías, y hay que hacerles hueco:

> *"Las tutorías… son imprevistos que te caen… de repente te cae una tutoría y la tienes que encajar."* (14:32)

Todo tiene que caber en sus horas de trabajo. Si una semana se llena, lo que no cabe pasa a la siguiente (15:00–15:27).

### 4.9. Prioridades: el problema principal

El cliente puso este ejemplo:

> *"Estoy preparando la clase de mañana y la de esta tarde; y de repente me viene un director de grado y me dice que tenemos reunión. Me secuestra… me quita una hora y la preparación de clases ya no la he podido hacer. Entonces tendré que recolocarla y ver los huecos disponibles."* (15:47–16:12)

Para saber dónde recolocar las cosas necesita prioridades. La próxima clase es lo más urgente (16:20).

Quiere:

- Una lista de tareas pendientes de colocar, ordenada por prioridad, para colocarlas él (16:42–16:54);
- Un contador que le diga cuánto falta para la fecha límite (17:04);
- Poder poner cuánto tiempo calcula que le llevará cada tarea, para que el sistema le ayude a buscar hueco (17:14);
- Un aviso para las tareas olvidadas, del tipo "llevas 180 días sin hacer esta tarea" (18:41).

La prioridad se calcula con dos cosas:

> *"Un parámetro temporal —cuánto tiempo lleva abierta y cuánto falta para la entrega— y otro de importancia asignado directamente por mí."* (19:06)

Sabe que hacerlo totalmente automático es muy difícil: "os lo estoy planteando en versión fácil" (17:41).

### 4.10. Cómo es una tarea

- Título.
- Descripción corta, de una sola línea. No quiere una descripción larga: "Cuanto más rápida sea la lectura, mejor" (22:02).
- Tiempo estimado.
- Fecha límite.
- Importancia, que la pone él.
- Sin archivos adjuntos: "eso va a Campus. El planificador solo me debe indicar lo que tengo que hacer" (19:48).

### 4.11. Subtareas (lo más importante para él)

Una tarea se puede dividir en subtareas, y esas en otras, y así sucesivamente. Es lo que no encuentra en ningún programa que haya probado (23:54).

> *"Lo fundamental es que haya alguna forma de segmentar en subtareas, y que cada subtarea sea a su vez segmentable en subtareas sucesivas."* (20:01)

Su ejemplo (20:43–21:15):

```
Preparar sesión
├─ Teoría
│   ├─ Revisar materiales
│   ├─ Mejorarlos
│   ├─ Buscar vídeos
│   └─ Preparar lectura previa en Campus
└─ Ejercicios
    ├─ Revisarlos
    ├─ Cambiar enunciados
    └─ Repensar la explicación si el año anterior no funcionó
```
Sobre cuántos niveles: primero dijo "sin límite" (20:24) y luego que le parecía bien limitarlo a 5 o 10 niveles (21:34).

### 4.12. Terminar y archivar tareas

- Una tarea terminada se marca con una casilla (22:06).
- Las terminadas pasan a una lista de tareas hechas (22:16).
- Las que ya no sirven se archivan, como en Gmail (22:20).
- Si terminas una tarea, sus subtareas aparecen también como terminadas (22:43).
- Las subtareas que falten se ven con una marca o un color (22:52).

### 4.13. Dónde se usa

Una aplicación web que funcione en ordenador, móvil y tablet (13:16).

## 5. Cambios en los requisitos

<!--
  Solo lo que cambia respecto a la sesión anterior: requisitos nuevos, modificados o descartados.
  La lista completa y vigente vive en la sesión 1 más los cambios de cada sesión
  (o en un documento de requisitos consolidado, si lo creamos).
-->
Como es la primera sesión, todos los requisitos son nuevos.

Leyenda:
 - C = confirmado por el cliente · 
 - P = el cliente lo ve bien, pero no es obligatorio · 
 - Q = no está claro, hay que preguntarlo.

### 5.1. Nuevos

| ID | | Requisito | Evidencia |
|-|:-:|-|-|
|RF-01| |C|	Guardar el calendario con el tipo de cada día: festivo, no lectivo o lectivo.	01:29 · 04:35|
|RF-02|	|P|	Meter el calendario a mano o desde un archivo.	04:56|
|RF-03||C|	Cada profesor mete su horario de trabajo de cada día.	06:40|
|RF-04||C|	Meter el horario de clases una vez por cuatrimestre.	07:59|
|RF-05||C|	Cancelar las clases de los días no lectivos y no poner nada en festivos.	01:54 · 05:17|
|RF-06||Q|	Marcar las clases que hay que recuperar. Falta saber cómo.	07:45|
|RF-07||C|	Indicar el tipo de cada clase y qué tipo de aula necesita.	09:03 · 11:12|
|RF-08||C|	Separar las tareas de dentro y de fuera del aula, y relacionar una tarea con una clase |(antes, durante o después).	08:24 · 12:04
|RF-09||C|	Anotar los recursos que necesita una clase o tarea, con enlace a Drive si hace falta.	10:32 · 24:26|
|RF-10||C|	Crear tareas de distintos tipos: docencia, investigación, emails, tutorías, reuniones, exámenes, Campus…	03:44 · 13:48|
|RF-11||C|	Cada tarea tiene título y una descripción de una línea.	19:26 · 21:54|
|RF-12||C|	Cada tarea tiene un tiempo estimado.	17:14|
|RF-13||C|Cada tarea tiene una importancia que pone el profesor.	19:06|
|RF-14||Q|	Cada tarea tiene fecha límite y un contador del tiempo que queda. Falta saber si la fecha es obligatoria.	17:04|
|RF-15||C|	Avisar de las tareas que llevan mucho tiempo sin hacerse.	18:41|
|RF-16||C|	Dividir una tarea en subtareas, y esas en otras, con varios niveles.	20:01 · 21:34|
|RF-17||C	|Marcar tareas como terminadas. Al terminar una tarea, se marcan sus subtareas.	22:06 · 22:43|
|RF-18|	|C|	Ver la lista de tareas hechas y archivar las que ya no sirven.	22:16 · 22:20|
|RF-19||C|	Ver la agenda del día con las tareas en orden.	02:56|
|RF-20||C|	Ver la lista de tareas sin colocar, ordenada por prioridad.	16:42|
|RF-21||C|	Calcular la prioridad con el tiempo (cuánto lleva abierta y cuánto falta) y la importancia.	19:06|
|RF-22||C|	Ayudar a encontrar un hueco libre para una tarea según su duración, sin pisar las clases.	16:12 · 17:23|
|RF-23||C|	Añadir imprevistos (tutorías, reuniones) y recolocar lo que se ha movido.	14:32 · 16:12|
|RF-24||C|	Si algo no cabe en la semana, pasarlo a la siguiente.	15:20|

#### Requisitos no funcionales (cómo tiene que ser el sistema)

| ID | Requisito | Minuto |
| :--- | :--- | :--- |
| RNF-01C | Que se lea rápido: textos de una línea. | 22:02 |
| RNF-02C | Aplicación web para ordenador, móvil y tablet. | 13:16 |
| RNF-03C | Que cada profesor pueda configurar su horario. | 07:04 |
| RNF-04C | Sencillo y centrado en Informática. | 11:46 |

#### Reglas de negocio (normas que el sistema debe respetar)

| ID | Regla | Minuto |
| :--- | :--- | :--- |
| RN-01C | En un día festivo no se planifica nada. | 05:17 |
| RN-02C | En un día no lectivo se trabaja, pero no hay clases. | 01:43 |
| RN-03C | Las clases son fijas: ninguna tarea puede ocupar su hora. | 07:23 |
| RN-04C | Todo se planifica dentro del horario de trabajo del profesor. | 07:12 · 15:00 |
| RN-05C | Las tareas de investigación siempre son fuera del aula. | 08:49 |
| RN-06C | La importancia la decide el profesor. | 19:06 |
| RN-07C | Si se termina una tarea, se terminan sus subtareas. | 22:43 |
| RN-08C | Archivar una tarea no la borra. | 22:20 |

### 5.2. Modificados

No aplica: es la primera sesión.

### 5.3. Descartados

#### Cosas que preguntamos y el cliente dijo que no

| ID | Requisito | Motivo |
| :--- | :--- | :--- |
| — | Adjuntar archivos a las tareas | "Eso va a Campus" (19:48) |
| — | Descripción larga de la tarea | Le basta con una línea (21:54) |
| — | Etiquetas de colores para ordenar | "No es indispensable" (23:06) |

## 6. Cambios en el alcance

<!-- Qué entra o sale del alcance en esta sesión. Si no hay cambios, escribir "Sin cambios". -->

### Alcance inicial (Primera sesión)

| Cambio | Elemento / Funcionalidad | Motivo |
| :--- | :--- | :--- |
| **Entra** | Organizador del día a día del profesor: calendario, horario, clases, tareas con subtareas, prioridades e imprevistos. | Es lo que pide el cliente. |
| **Sale** | Reglas de RRHH (37,5 h, máximo 9 h, descansos). | "No tengáis en cuenta las reglas" (06:59) |
| **Sale** | Reserva de aulas. | Ya la lleva Ordenación Académica (10:00) |
| **Sale** | Comprobar el aforo real de las aulas en exámenes. | El cliente lo ve imposible de controlar (24:40–25:28) |
| **Sale** | Otras carreras (CAFyD…). | Solo Informática (11:46) |

## 7. Modelado

### 7.1. Diagramas actualizados

- [Versión 1](../../images/v1.png)

### 7.2. Decisiones de modelado del grupo

<!-- Continúa la numeración D-xx de sesiones anteriores. Indicar si el cliente ya las validó. -->

### Decisiones nuestras, no del cliente (Hay que confirmarlas con él)

| ID | Decisión | Motivo | ¿Validada? |
| :--- | :--- | :--- | :--- |
| D-01 | La prioridad no la escribe nadie: se calcula sola a partir de la fecha límite, el tiempo que lleva abierta y la importancia. | El cliente nos dio los ingredientes, no la fórmula. | Pendiente |
| D-02 | Una tarea se puede colocar en varios huecos de la agenda. | Para poder moverla. Falta saber si se puede partir en trozos. | Pendiente |
| D-03 | Los recursos tienen tipo (documento, material o software) y un enlace opcional. | El cliente dio ejemplos de los tres. | Pendiente |
| D-04 | Separamos "laboratorio" de "prácticas con ordenador". | El cliente nos dejó decidirlo (09:32). | — |

## 8. Glosario: términos nuevos o corregidos

### Glosario de Términos

| Término | Significado |
| :--- | :--- |
| **Docente** | El profesor que usa el sistema. Aquí todos son también investigadores. |
| **Día festivo** | Día en que no se trabaja. |
| **Día no lectivo** | Día en que se trabaja pero no hay clases (p. ej., el día de la universidad). |
| **Día lectivo** | Día en que se trabaja y hay clases. |
| **Bloque de disponibilidad** | Horas de trabajo que pone el profesor para cada día. |
| **Horario de clases** | Horario fijo que pone Ordenación Académica. |
| **Sesión** | Una clase concreta, en un día y a una hora. |
| **Recurso** | Lo que hace falta para una clase o tarea: un documento, un material o un programa. |
| **Tarea** | Cualquier cosa que el profesor tiene que hacer. |
| **Subtarea** | Una tarea que forma parte de otra más grande. |
| **Importancia** | Lo importante que es una tarea para el profesor. La pone él. |
| **Prioridad** | Orden en que conviene hacer las tareas, según la importancia y el tiempo. |
| **Imprevisto** | Algo que aparece sin avisar (una tutoría, una reunión) y obliga a mover otras tareas. |
| **Archivar** | Quitar una tarea de la vista sin borrarla. |

## 9. Preguntas para la próxima sesión

<!--
  Incluir las que quedaron ⏳ o 🔶 en el apartado 3 más las nuevas.
  Agrupar por tema. Las que más afectan al modelo, primero.
-->
### Preguntas y Dudas para el Cliente

---

#### Sobre la prioridad y la agenda

1. **¿Hay tareas que nunca se pueden mover, además de las clases?** Por ejemplo, una reunión ya fijada. 
2. **¿Una tarea se puede hacer en varios ratos o tiene que ir en un solo bloque?**
3. **Si una tarea se queda a medias por un imprevisto:** ¿Se vuelve a colocar solo lo que falta? 
4. **¿Quiere ver la agenda por día, por semana o las dos?**
5. El aviso de "llevas 180 días sin hacer esta tarea", ¿solo avisa o también hace que la tarea suba en la lista? 

--- 

#### Sobre las clases
1. **¿Hay horas fijas de tutoría en su horario, o todas las tutorías son imprevistas?** 
2. **Si una clase cae en un día no lectivo:** ¿Se pierde o hay que recuperarla? ¿Quién elige el día de recuperación? 
3. **Al crear una clase:** ¿Quiere que aparezcan solas las tareas de "preparar", "revisar material" y "subir a Campus"? 

---

## 10. Acuerdos y tareas del grupo

<!-- Quién hace qué antes de la próxima sesión. Marcar [x] al terminar. -->
### Tareas Pendientes y Realizadas

| Tarea | Responsable | Fecha límite |
| :--- | :--- | :--- |
| ☑ Transcribir la grabación de la sesión 1 | `Jose Luis de la Asunción` `Alejandra Cuesta` | 29/10 |
| ☑ Modelo del dominio v1 en la pizarra | Todo el grupo | 04/11 |

**Próxima sesión:** 12/11/2026 · 12:15 · Clase -1,14

---

**Fuentes de esta sesión:** [transcripción de la reunión del 27/10/2026](../sesiones/transcripts/sesion01.md)
