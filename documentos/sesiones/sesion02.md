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

# SESIÓN 02:
### 12/11/2026

<div align=center>

| | |
|-|-|
| **Tipo** | Reunión extra |
| **Cliente** | Jose Manuel Breñosa |
| **Grupo** | 4 |
| **Coordinación** | @Alejandracuesta |
| **Redacta el acta** | Alejandra Cuesta |
| **Duración** | 12:15 – 12:40 |
| **Grabación** | Sí  · [transcript](../sesiones/transcripts/sesion02.md) |

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
| Juan Carlos Quintana | NO |
| José Luis de la Asunción | SÍ |
| Emilio Muciño | SÍ |
| Daniel Cotarelo | SÍ |
| **Total** | **6/7 (85%)** |

</div>

## 2. Objetivo de la sesión

## 2. Objetivo de la sesión

Enseñar al cliente el borrador del modelo del dominio y resolver las dudas que quedaron abiertas en la sesión 1, sobre todo qué hacer con el investigador, que en nuestro modelo se quedaba aislado.

**Material que llevamos:**
- Borrador del modelo del dominio (v2).
- Lista de preguntas de la sesión 1.

## 3. Respuestas a las preguntas pendientes

**Estado:** ✅ resuelta · 🔶 parcial · ⏳ no se preguntó (pasa a la sesión 3)

| Nº | Pregunta (sesión 01) | Respuesta del cliente | Estado | Impacto |
|:-:|-|-|:-:|-|
| 1 | ¿La aplicación es solo para usted o para cualquier profesor? | No se preguntó. | ⏳ | Sigue abierta. Ahora pesa más porque habla de colaboradores (ver apartado 4.4). |
| 2 | ¿Todas las tareas tienen fecha límite? | **No.** Hay tareas generales sin fecha, como mejorar un recurso didáctico (14:35–14:55). | ✅ | RF-14: la fecha límite es opcional. |
| 3 | ¿Cómo se puntúa la importancia? | No se preguntó. | ⏳ | — |
| 4 | ¿Cada subtarea tiene su propia fecha, importancia y tiempo? | No lo dijo directamente, pero repitió que cada subtarea *"a su vez son tareas"* (02:40 · 08:05). | 🔶 | Una subtarea tiene los mismos datos que una tarea. Conviene confirmarlo. |
| 5 | ¿Se puede terminar una tarea con subtareas pendientes? ¿Se termina sola la principal? | No se preguntó. | ⏳ | — |
| 6 | ¿Archivar es lo mismo que borrar? | No se preguntó. | ⏳ | — |
| 7 | ¿Máximo de niveles de subtareas? | No dio un número: se divide *"cuando sea necesario, cuando tú lo creas conveniente"* (02:40). | 🔶 | Lo decide el profesor. Podemos dejarlo sin límite. |
| 8 | ¿El sistema coloca las tareas solo o propone y decide usted? | No se preguntó. | ⏳ | — |
| 9 | ¿El aviso de "180 días" solo avisa o sube la tarea en la lista? | **Solo avisa:** *"va a haber tareas que sean tan poco importantes que van a estar ahí de por vida"* (13:55). | ✅ | RF-15 aclarado: el aviso no cambia la prioridad. |
| 10 | ¿Hay tareas que nunca se pueden mover, además de las clases? | **Todas las tareas se pueden mover:** *"ya si son inamovibles, ya las consideraré como inamovibles yo"* (08:35). | ✅ | No hace falta marcar tareas fijas. Solo las clases son fijas. |
| 11 | ¿Una tarea se puede hacer en varios ratos o en un solo bloque? | En **un bloque**. Una tarea tiene un tiempo estimado y una hora de comienzo. Si se puede partir, él mismo crea subtareas (05:00 · 06:55). | ✅ | No partimos una tarea en trozos. Si hace falta, se crean subtareas. |
| 12 | Si una tarea se queda a medias, ¿se recoloca solo lo que falta? | **No:** se queda **entera como no realizada** y se vuelve a planificar (06:55–08:05). | ✅ | Nuevo estado "no realizada". |
| 13 | ¿Agenda por día, por semana o ambas? | **Las dos** (11:05). | ✅ | RF-19 ampliado. |
| 14 | ¿Quiere avisos cuando se acerque una fecha límite? | No se preguntó. | ⏳ | — |
| 15 | ¿Hay horas fijas de tutoría? | **No.** Las tutorías surgen de las dudas que le mandan los alumnos por email (11:30–12:05). | ✅ | La tutoría sigue siendo un tipo de tarea, no una clase fija. |
| 16 | Si una clase cae en día no lectivo, ¿se pierde o se recupera? | **Se pierde** (10:00–10:35). Se podría recuperar creando una tarea de recuperación (10:40–10:45). | ✅ | RF-06 aclarado. |
| 17 | ¿Se crean solas las tareas de "preparar" y "subir a Campus" al crear una clase? | No se preguntó. | ⏳ | — |
| 18 | ¿Un examen es una clase o una tarea? | **El examen es una clase; prepararlo son tareas** (09:25). | ✅ | Nuevo tipo de clase: examen. |
| 19 | ¿Qué tareas de investigación tiene? ¿Hay proyectos? | **Sí, hay proyectos**, pequeños o grandes, con tareas dentro (00:45). La investigación incluye investigar, publicar y desarrollar (16:25). | ✅ | Nueva clase **Proyecto**. |

## 4. Información nueva del cliente

### 4.1. El investigador no se puede quitar

Le dijimos que en nuestro modelo el investigador se quedaba aislado y le preguntamos si podíamos quitarlo. Respondió que **no**:

> *"No, no se puede cargar. Puedes asignarle tareas tipo proyecto o investigaciones a secas… Pueden ser mini proyectos o proyectos grandes con tareas específicas dentro del proyecto."* (00:45)

Lo que hace un investigador (16:25):
- **Investigar**, a veces por interés propio, sin obligación de publicar.
- **Publicar.**
- **Proyectos**, que a su vez tienen tareas de investigación, publicación y desarrollo.

No quiere que entremos en mucho detalle, porque **en esta universidad la investigación tiene poco peso** y pesa más la docencia (17:00–17:30). Nos propuso una solución sencilla:

> *"Las tareas, las mismas de docencia, podrían ser de investigación y con simplemente un identificador que ayude al profesor a saber si es de investigación o de docencia, como un color o una etiqueta o algo, ya está."* (17:35)

### 4.2. Cuándo se divide una tarea en subtareas

> *"Cuando sea necesario. Cuando tú lo creas conveniente."* (02:40)

Su ejemplo, construir una bici (02:40–03:30):

```
Construir una bici
└─ Pintar la bici
    ├─ Lijar
    ├─ Masillar
    ├─ Lijar otra vez
    ├─ Imprimar
    └─ Pintar
```

Cada subtarea *"a su vez son tareas porque se pueden segmentar en más subtareas"*.

### 4.3. Tareas en orden o a la vez

Las tareas pueden ir **en orden** (secuenciales) o **a la vez** (en paralelo):

> *"Secuencialmente es cuando unas necesitan de otras y en paralelo es cuando no hay necesidad entre ellas."* (03:55–04:30)

En la bici, por ejemplo, no se puede pintar antes de lijar.

### 4.4. Quién hace cada tarea

Al hablar de tareas en paralelo mencionó que **no siempre las hace él**:

> *"Si son en paralelo y las tiene que ejecutar un agente, el agente podrá ser la persona u otra persona, si alguien está colaborando contigo, o un agente artificial."* (03:55)

Es una idea nueva que puede ampliar mucho el sistema (ver pregunta 1 del apartado 9).

### 4.5. El tiempo de una tarea

(05:00–05:40)

- Cada tarea tiene un **tiempo de ejecución**: lo que el profesor calcula que le va a llevar. *"Suele llevarse más tiempo de lo que uno estima."*
- Tiene una **hora de comienzo**. Con la duración se calcula a qué hora debería acabar.
- Si no da tiempo, se puede **cortar y seguir en otro momento** o **alargar** el rato que se le está dedicando.

### 4.6. Tareas cortadas: no realizadas

Una tarea no se parte en trozos de tiempo. Si se puede dividir, él mismo crea subtareas. Y si le interrumpen, la tarea se queda **entera como no realizada**:

> *"Si una tarea la puedo partir en diferentes trozos, ya crearé esas subtareas… Y no me pondré a hacer una tarea si veo que no me va a dar tiempo… Igual me viene alguien y me dice, tenemos que irnos a no sé dónde. Pues entonces tendré que cortarla y se quedará como no realizada… Igual tengo que replanificar los tiempos. Pero la tarea se queda sin hacer."* (06:55–07:40)

### 4.7. Todas las tareas se pueden mover

Solo las clases son fijas. Las tareas se consideran todas movibles; si alguna no se puede mover, él lo tendrá en cuenta (08:35). Ejemplo: una reunión que convoca otra persona en teoría no se mueve, pero se la pueden cambiar de hora otros (08:50).

### 4.8. Exámenes

**Preparar el examen son tareas; el examen en sí es una clase** (09:25).

### 4.9. Clases que se pierden

Si una clase cae en un día no lectivo, **se pierde y no se recupera**. Le pasa a menudo en el segundo cuatrimestre con los días no lectivos que no se avisan con tiempo (10:00–10:35). Se podría recuperar, pero no suele hacerse. Si quiere recuperarla, puede crearse una **tarea de recuperación de clase** (10:40–10:45).

### 4.10. Seminarios de final de cuatrimestre

En sus asignaturas hace **seminarios** al final del cuatrimestre, después de que acaben las clases. Los trata **como clases normales**: los alumnos repasan ejercicios (11:30–12:00).

### 4.11. Cómo funcionan sus tutorías

No tiene horas fijas de tutoría; otros profesores sí las tienen (12:05). Su forma de trabajar (12:05–13:00):

1. Si un alumno tiene una duda, le pide que se la mande por **email**.
2. Si es una duda que pueden tener otros alumnos, la **resuelve en clase**, para que la oigan todos.
3. Si el alumno está muy perdido, le da una **tutoría individual**.
4. Si el tema es muy importante, **abre la tutoría a otros alumnos**.
5. Las tutorías las planifica **fuera de clase**.

### 4.12. Tareas sin fecha límite

Hay tareas sin fecha, por ejemplo *"mejorar un determinado recurso didáctico"*. No suele dedicarles un rato aparte; las va trabajando poco a poco en clase, probando distintas formas de explicar (14:55–15:35).

### 4.13. Agenda

Quiere ver la agenda **por día y por semana** (11:05).

## 5. Cambios en los requisitos

**Leyenda:** C = confirmado por el cliente · P = el cliente lo ve bien, pero no es obligatorio · Q = no está claro, hay que preguntarlo.

### 5.1. Nuevos

**Requisitos funcionales**

| ID | | Requisito | Minuto |
|-|:-:|-|-|
| RF-25 | C | Como investigador, crear proyectos (pequeños o grandes), investigaciones y publicaciones, cada uno con sus propias tareas. | 00:45 · 16:25 |
| RF-26 | C | Distinguir a simple vista, con una etiqueta o un color, si una tarea es de docencia o de investigación. | 17:35 |
| RF-27 | C | Indicar si las subtareas van en orden (una necesita que acabe otra) o se pueden hacer a la vez. | 03:55–04:30 |
| RF-28 | Q | Indicar quién hace cada tarea: el profesor, un colaborador o un agente artificial. | 03:55 |
| RF-29 | C | Cada tarea tiene una hora de comienzo; la hora de fin se calcula con el tiempo estimado. | 05:00 |
| RF-30 | C | Poder alargar una tarea en curso o cortarla. Si se corta, queda como no realizada y se vuelve a planificar. | 05:00 · 07:00–07:40 |
| RF-31 | C | Registrar los exámenes como clases y su preparación como tareas. | 09:25 |
| RF-32 | P | Crear una tarea de "recuperar clase" si el profesor quiere recuperar una clase perdida. | 10:40–10:45 |
| RF-33 | C | Añadir clases extra, como los seminarios de final de cuatrimestre, que funcionan igual que una clase normal. | 11:30 |

**Reglas de negocio**

| ID | | Regla | Minuto |
|-|:-:|-|-|
| RN-09 | C | Todas las tareas se pueden mover. Solo las clases son fijas. | 08:35 |
| RN-10 | C | El aviso de antigüedad no cambia la prioridad: solo informa. | 13:55 |
| RN-11 | C | Una clase que cae en día no lectivo se pierde; no se recupera sola. | 10:00 |
| RN-12 | C | Una tarea interrumpida cuenta como no realizada entera, no a medias. | 07:30 · 08:05 |
| RN-13 | C | Si una tarea necesita que acabe otra, no puede hacerse antes que ella. | 03:55 |
| RN-14 | C | No hay horas fijas de tutoría; se planifican fuera de clase cuando hacen falta. | 11:30 · 12:05 |
| RN-15 | C | Una subtarea es una tarea más: se puede dividir y se completa por su cuenta. | 02:40 · 08:05 |

### 5.2. Modificados

| ID | Antes | Ahora | Minuto |
|-|-|-|-|
| RF-06 | Q · Marcar las clases que hay que recuperar; falta saber cómo. | C · Una clase en día no lectivo se pierde. Si el profesor quiere recuperarla, crea una tarea (RF-32). | 10:00–10:45 |
| RF-14 | Q · Fecha límite; falta saber si es obligatoria. | C · La fecha límite es **opcional**: hay tareas generales sin fecha. | 14:35–14:55 |
| RF-15 | C · Avisar de tareas que llevan mucho tiempo sin hacerse. | C · Se mantiene, aclarando que **solo avisa** y no sube la prioridad. | 13:55 |
| RF-16 | C · Subtareas con varios niveles. | C · Se dividen cuando el profesor lo crea conveniente; cada subtarea es una tarea completa. | 02:40 |
| RF-19 | C · Ver la agenda del día. | C · Ver la agenda **por día y por semana**. | 11:05 |

### 5.3. Descartados

| ID | Requisito | Motivo |
|-|-|-|
| — | Marcar tareas como fijas o movibles | Todas las tareas se pueden mover (08:35). |
| — | Horario fijo de tutorías | El cliente no tiene horas fijas (11:30). |
| — | Partir una tarea en varios trozos de tiempo | Si se puede partir, el profesor crea subtareas (06:55). |

## 6. Cambios en el alcance

| | Cambio | Motivo |
|-|-|-|
| Entra | Perfil de investigador: proyectos, investigaciones y publicaciones, con sus tareas. | 00:45 · 16:25 |
| Entra | Clases extra (seminarios) y exámenes como clases. | 09:25 · 11:30 |
| Sale | Detallar los tipos de investigación, publicaciones o proyectos. | *"No quiero daros tanto detalle"*: la investigación tiene poco peso aquí (17:00). |
| Pendiente | Tareas hechas por otras personas o por un agente artificial. | Lo mencionó (03:55), pero haría que el sistema fuera para varios usuarios. Hay que confirmarlo. |

## 7. Modelado

### 7.1. Diagramas actualizados

En esta sesión enseñamos el modelo v1 (sesión 1). Con lo hablado en las dos sesiones hemos hecho la **versión 2**. 

- [Versión 2](../../images/v2.png)

### 7.2. Cambios respecto a la versión anterior

| Cambio | Elemento | Motivo |
|-|-|-|
| Añadido | **Profesor** con dos perfiles: **Docente** e **Investigador** | Todo profesor tiene los dos perfiles (16:25). Comparten calendario, horario de trabajo y agenda. |
| Modificado | **Docente** | Se queda con todo lo de docencia: asignaturas, clases y sus tareas (preparar clase, emails, tutorías, reuniones, Campus…). |
| Añadido | **Investigador** | Recupera su sitio en el modelo (*"no se puede cargar"*, 00:45). Tiene los proyectos, las investigaciones y las publicaciones (16:25). |
| Añadido | **Proyecto**, **Investigación** y **Publicación** | Los tres trabajos del investigador, cada uno con sus tareas. El proyecto puede ser pequeño o grande (00:45). |
| Añadido | Etiqueta **docencia / investigación** en la tarea | No la escribe el profesor: sale de si la tarea es del docente o de un trabajo de investigación. Se muestra como color o etiqueta (17:35). |
| Añadido | Relación "**necesita**" entre tareas | Para las tareas que van en orden (03:55). |
| Añadido | **Hora de comienzo** y **hora de fin prevista** en el hueco de la agenda | El cliente habla de tiempo de ejecución y hora de comienzo (05:00). La hora de fin se calcula sumando las dos. |
| Añadido | Estado **no realizada** en la tarea | Para las tareas cortadas a medias (07:30). |
| Añadido | Tipos de clase **examen** y **seminario** | 09:25 · 11:30 |
| Añadido | Tipos de tarea **preparar examen** y **recuperar clase** | 09:25 · 10:45 |
| Modificado | Hueco en la agenda | Antes, una tarea podía ocupar varios huecos; ahora ocupa **uno**. Si se corta, se vuelve a planificar entera (06:55). |
| Modificado | Duración de la tarea | Pasa a llamarse **tiempo de ejecución**, como lo llama el cliente (05:00). |
| Modificado | Clase | El tipo de clase y el aula pasan a la propia clase, porque los seminarios no vienen del horario de Ordenación Académica (11:30). |
| Eliminado | Estado "a recuperar" y relación "una clase recupera otra" | Las clases de días no lectivos se pierden; si se quiere recuperar una, se crea una tarea de recuperar clase (10:00–10:45). |
| Eliminado | Tipo de tarea "examen" | El examen es una clase; lo que queda como tarea es prepararlo (09:25). |
| Sin cambios | Tutoría | Sigue siendo un tipo de tarea; no hay horario fijo (11:30). |

### 7.3. Decisiones de modelado del grupo

| ID | Decisión | Motivo | ¿Validada? |
|-|-|-|:-:|
| D-01 | La prioridad se calcula con la fecha límite, el tiempo abierta y la importancia. | Sesión 1. El aviso de antigüedad **no** entra en el cálculo (13:55). | Parcial |
| D-02 | ~~Una tarea puede ir en varios huecos.~~ **Una tarea va en un solo hueco**; si se corta, se replanifica. | Respuesta a la pregunta 11. | Sí |
| D-03 | Los recursos tienen tipo y enlace opcional. | Sesión 1. | Pendiente |
| D-04 | Separamos laboratorio de prácticas con ordenador. | Sesión 1. | — |
| D-05 | El profesor tiene dos perfiles. El **investigador** tiene los proyectos, las investigaciones y las publicaciones; el **docente**, todo lo demás. Cada tarea pertenece a uno de los dos, y de ahí sale su etiqueta de docencia o investigación. | El investigador no se puede quitar (00:45), sus trabajos son investigar, publicar y los proyectos (16:25), y basta con un identificador para distinguir las tareas (17:35). | Pendiente de confirmar |
| D-06 | El orden entre tareas se guarda como "esta tarea necesita a esta otra". | Es la forma más sencilla de representar *"unas necesitan de otras"* (03:55). | Pendiente |

## 8. Glosario: términos nuevos o corregidos

| Término | Significado |
|-|-|
| **Profesor** | La persona que usa el sistema. Tiene dos perfiles: docente e investigador. |
| **Docente** *(corregido)* | Perfil del profesor para todo lo de docencia: asignaturas, clases y sus tareas. |
| **Investigador** *(corregido)* | Perfil del profesor para la investigación. Lleva los proyectos, las investigaciones y las publicaciones. |
| **Proyecto** | Trabajo del investigador con tareas dentro. Puede ser pequeño o grande. |
| **Investigación** | Trabajo del investigador por interés propio, sin obligación de publicar. |
| **Publicación** | Trabajo del investigador para publicar resultados. |
| **Etiqueta de ámbito** | Marca (color o etiqueta) que dice si una tarea es de docencia o de investigación. |
| **Tareas secuenciales** | Tareas que van en orden porque una necesita que acabe la otra. |
| **Tareas en paralelo** | Tareas que se pueden hacer a la vez porque no dependen entre sí. |
| **Agente** | Quien hace una tarea: el profesor, un colaborador o un agente artificial. *(Pendiente de confirmar.)* |
| **Tiempo de ejecución** | Lo que el profesor calcula que le llevará una tarea. |
| **Hora de comienzo** | Cuándo se empieza una tarea. Junto al tiempo de ejecución, da la hora de fin prevista. |
| **Tarea no realizada** | Tarea que se empezó pero se cortó. Cuenta como no hecha y hay que volver a planificarla. |
| **Seminario** | Clase extra al final del cuatrimestre para repasar. Funciona como una clase normal. |
| **Tarea general** | Tarea sin fecha límite (p. ej., mejorar un recurso didáctico). |


## 9. Acuerdos y tareas del grupo

| | Tarea | Responsable | Fecha límite |
|:-:|-|-|-|
| ☑ | Transcribir la grabación de la sesión 2 | Alejandra Cuesta y Alejandro de la Peña | 12/11 |
| ☑ | Hacer el modelo del dominio v2 con los cambios del apartado 7.2 | Todos | 12/11 |

---

**Fuentes de esta sesión:** grabación de la reunión del 12/11/2026 ([transcripción sesión 2](../sesiones/transcripts/sesion02.md)) · acta de la ([transcripción sesión 1](../sesiones/transcripts/sesion01.md)).