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

# SESIÓN <NN>:
### <DD/MM/AAAA>

<div align=center>

| | |
|-|-|
| **Tipo** | <Reunión oficial (horario de clase) / Reunión extra> |
| **Cliente** | Jose Manuel Breñosa |
| **Grupo** | 4 |
| **Coordinación** | @Alejandracuesta |
| **Redacta el acta** | <nombre> |
| **Duración** | <hh:mm – hh:mm> |
| **Grabación** | <Sí / No · enlace o ubicación> |

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
| Alejandra Cuesta | ☐ |
| Ismael Cobo | ☐ |
| Alejandro de la Peña | ☐ |
| Juan Carlos Quintana | ☐ |
| José Luis de la Asunción | ☐ |
| Emilio Muciño | ☐ |
| Daniel Cotarelo | ☐ |
| **Total** | **<n>/7 (<%>)** |

</div>

## 2. Objetivo de la sesión

<!-- Qué queríamos conseguir al entrar a la reunión. Una o dos frases. -->

<Ejemplo: Validar con el cliente el modelo del dominio v0.2 y resolver las preguntas pendientes de la sesión anterior.>

**Material que llevamos:**
- <Modelo del dominio vX.Y>
- <Lista de preguntas de la sesión NN-1>

## 3. Respuestas a las preguntas pendientes

<!--
  Copiar aquí las preguntas del apartado 9 de la sesión anterior y apuntar la respuesta.
  Estado: ✅ resuelta · 🔶 parcial · ⏳ sin tratar (pasa a la siguiente sesión)
  Impacto: qué requisito, regla o clase cambia por la respuesta.
-->

| Nº | Pregunta (sesión <NN-1>) | Respuesta del cliente | Estado | Impacto |
|:-:|-|-|:-:|-|
| <1> | <pregunta> | <respuesta, con cita o minuto> | <✅/🔶/⏳> | <RF-xx pasa de Q a C · cambia la clase Tarea…> |
| <2> | | | | |

## 4. Información nueva del cliente

<!--
  Lo que el cliente contó por primera vez en esta sesión, agrupado por temas.
  Incluir citas literales cuando aporten matiz: > *"cita"* (mm:ss)
  Borrar los temas que no salieron.
-->

### 4.1. <Tema>

<Resumen en prosa de lo que dijo.>

> *"<cita literal>"* (<mm:ss>)

### 4.2. <Tema>

<…>

## 5. Cambios en los requisitos

<!--
  Solo lo que cambia respecto a la sesión anterior: requisitos nuevos, modificados o descartados.
  La lista completa y vigente vive en la sesión 1 más los cambios de cada sesión
  (o en un documento de requisitos consolidado, si lo creamos).
-->

### 5.1. Nuevos

| ID | | Requisito | Evidencia |
|-|:-:|-|-|
| RF-<xx> | <C/P/Q> | <enunciado> | <mm:ss> |
| RNF-<xx> | | | |
| RN-<xx> | | | |

### 5.2. Modificados

| ID | Antes | Ahora | Motivo / evidencia |
|-|-|-|-|
| <RF-xx> | <enunciado o etiqueta anterior> | <enunciado o etiqueta nueva> | <mm:ss> |

### 5.3. Descartados

| ID | Requisito | Motivo |
|-|-|-|
| <RF-xx> | <enunciado> | <el cliente dice que no hace falta…> |

## 6. Cambios en el alcance

<!-- Qué entra o sale del alcance en esta sesión. Si no hay cambios, escribir "Sin cambios". -->

| | Cambio | Motivo |
|-|-|-|
| <Entra / Sale> | <…> | <…> |

## 7. Modelado

### 7.1. Diagramas actualizados

<div align=center>

|![](../../imagenes/sesion<NN>-<nombre>.svg)
|-
|Código fuente: [sesion<NN>-<nombre>.puml](../../modelosUML/sesion<NN>-<nombre>.puml)

</div>

### 7.2. Cambios respecto a la versión anterior

<!-- Registro de cambios del modelo: qué se añade, quita o renombra y por qué. -->

| Cambio | Elemento | Motivo |
|-|-|-|
| <Añadido / Eliminado / Modificado> | <Clase / atributo / relación> | <Respuesta a la pregunta nº / requisito RF-xx> |

### 7.3. Decisiones de modelado del grupo

<!-- Continúa la numeración D-xx de sesiones anteriores. Indicar si el cliente ya las validó. -->

| ID | Decisión | Motivo | ¿Validada? |
|-|-|-|:-:|
| D-<xx> | <…> | <…> | <Sí / No / Pendiente> |

## 8. Glosario: términos nuevos o corregidos

| Término | Significado |
|-|-|
| **<término>** | <definición> |

## 9. Preguntas para la próxima sesión

<!--
  Incluir las que quedaron ⏳ o 🔶 en el apartado 3 más las nuevas.
  Agrupar por tema. Las que más afectan al modelo, primero.
-->

**<Tema>**
1. <pregunta>
2. <pregunta>

**<Tema>**

3. <pregunta>

## 10. Acuerdos y tareas del grupo

<!-- Quién hace qué antes de la próxima sesión. Marcar [x] al terminar. -->

| | Tarea | Responsable | Fecha límite |
|:-:|-|-|-|
| ☐ | <Actualizar el modelo del dominio con las respuestas> | <nombre> | <DD/MM> |
| ☐ | <Preparar el diagrama de casos de uso> | <nombre> | <DD/MM> |
| ☐ | <Subir el acta y los diagramas al repo> | <nombre> | <DD/MM> |

**Próxima sesión:** <DD/MM/AAAA · hora · lugar>

---

**Fuentes de esta sesión:** <grabación de la reunión del DD/MM/AAAA · documentos de apoyo>
