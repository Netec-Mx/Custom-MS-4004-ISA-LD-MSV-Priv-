# Práctica 5. Consolidar acuerdos y compromisos de múltiples reuniones

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Intermedia |
| Nivel de Bloom | Aplicar |
| Tecnología Principal | Microsoft 365 Copilot, Facilitator (Loop) y Galería de indicaciones |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Presentar las fuentes y el prompt reutilizable | 3 min |
| Tarea 2. Consolidar y clasificar los compromisos | 5 min |
| Tarea 3. Generar la vista de atención y detectar duplicados | 4 min |
| Tarea 4. Guardar el prompt en la Galería de indicaciones | 3 min |
| **Total** | **15 min** |

> Práctica conducida por el instructor (según el temario). El instructor ejecuta cada paso en pantalla; los participantes siguen con la misma indicación y, si el instructor compartió con ellos las páginas de Loop y la transcripción, la ejecutan en paralelo.

---

# Descripción General

Durante la planeación de INT-MDV-2026 se realizaron tres reuniones (20-oct, 27-oct y 03-nov). Los acuerdos y compromisos quedaron repartidos entre notas de Facilitator en Loop y una transcripción. El instructor mostrará cómo un **prompt reutilizable** permite a Copilot consolidar acuerdos, decisiones, responsables, fechas y pendientes, detectar duplicados y guardar la indicación en la Galería de indicaciones para ejecutarla periódicamente.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Consolidar con un prompt reutilizable los acuerdos y compromisos de varias reuniones, conservando la reunión de origen.
- Distinguir compromisos propios, asignados a otras personas y sin responsable o fecha.
- Organizar los compromisos por estado y prioridad e identificar atrasos y próximos vencimientos.
- Detectar compromisos duplicados entre reuniones y guardar el prompt en la Galería de indicaciones.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 5](../../images/p05-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Conceptos de seguimiento de compromisos (responsable, fecha, estado).

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Páginas de Loop de laboratorio compartidas por el instructor (opcional para participantes).

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Copilot |
| Rol "propio" en el escenario | `Coordinación de la intervención` (la persona que ejecuta el prompt) |
| Fecha de referencia | 6 de noviembre de 2026 |
| Recurso adicional | Nombre del entregable: `Vista_Compromisos_INT-MDV_[INICIALES].xlsx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Microsoft Loop | Servicio administrado | Páginas de notas de Facilitator | [https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams) |
| Galería de indicaciones de Copilot | Servicio administrado | Guardar y reutilizar prompts | [https://m365.cloud.microsoft/copilot-prompts](https://m365.cloud.microsoft/copilot-prompts) |
| Microsoft Excel | Microsoft 365 Apps, Canal Actual | Vista consolidada | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Notas_Facilitator_2026-10-27.docx](recursos/Notas_Facilitator_2026-10-27.docx) | Contenido de las notas de Facilitator de la coordinación interáreas (base de la página de Loop) |
| [Notas_Facilitator_2026-11-03.docx](recursos/Notas_Facilitator_2026-11-03.docx) | Contenido de las notas de Facilitator del comité de preparación |
| [Transcripcion_Planeacion_2026-10-20.docx](recursos/Transcripcion_Planeacion_2026-10-20.docx) | Transcripción de la reunión de planeación |

## Archivos de la práctica

```text
Capitulo02/Practica05/recursos/Notas_Facilitator_2026-10-27.docx
Capitulo02/Practica05/recursos/Notas_Facilitator_2026-11-03.docx
Capitulo02/Practica05/recursos/Transcripcion_Planeacion_2026-10-20.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica05/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Presentar las fuentes y el prompt reutilizable

## Objetivo

Mostrar qué fuentes se consolidarán y la estructura de un prompt que pueda reutilizarse.

## Instrucciones

### Paso 1

El instructor abre la aplicación Microsoft 365 Copilot, selecciona **Copilot** y muestra con `/` las dos páginas de Loop y la transcripción.

### Paso 2

El instructor explica las partes del prompt reutilizable: periodo, fuentes, campos, clasificación y formato. Los participantes copian el prompt:

```text
Revisa las notas de Facilitator en Loop y las transcripciones de las reuniones del proyecto INT-MDV-2026
realizadas entre el 20 de octubre y el 6 de noviembre de 2026. Consolida en una tabla todos los acuerdos,
decisiones y compromisos con: descripción, reunión de origen (fecha), responsable, fecha comprometida y tipo:
"Propio" (Coordinación de la intervención), "Asignado a otra persona" o "Sin responsable o sin fecha".
No inventes responsables ni fechas. Fecha de referencia: 6 de noviembre de 2026.
```

---

# Tarea 2. Consolidar y clasificar los compromisos

## Objetivo

Obtener la tabla consolidada con estado y prioridad.

## Instrucciones

### Paso 1

El instructor ejecuta el prompt referenciando las fuentes con `/` y revisa la tabla con el grupo.

### Paso 2

El instructor solicita:

```text
Agrega las columnas Estado (Cumplido, Vencido, Próximo a vencer en 7 días, Sin fecha) y Prioridad (Alta, Media, Baja),
y una columna "Acción de seguimiento". Ordena por estado y prioridad.
```

### Paso 3

Comprobar con el grupo que aparezcan: verificación de grúa (**vencido** el 05-nov), permiso de aceite (**próximo**, 10-nov), notificación a clientes (**próximo**, 14-nov), vocero ante medios (**sin responsable**) y plan con comunidades (**sin fecha**).

---

# Tarea 3. Generar la vista de atención y detectar duplicados

## Objetivo

Evitar dar seguimiento por separado a la misma actividad.

## Instrucciones

### Paso 1

El instructor escribe:

```text
Identifica compromisos que aparezcan en diferentes reuniones y que correspondan a la misma actividad.
Unifícalos en una sola fila indicando todas las reuniones de origen y la fecha vigente.
Luego muestra solo los compromisos que requieren atención: atrasados, próximos a vencer y sin responsable.
```

### Paso 2

Verificar que se unifiquen "Enviar cronograma consolidado" (20-oct, fecha 24-oct), "Enviar cronograma actualizado" (27-oct, fecha 31-oct) y "Compartir cronograma consolidado" (03-nov, fecha 07-nov) como una sola actividad **propia**.

### Paso 3

Copiar la tabla a Excel. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Vista_Compromisos_INT-MDV_[INICIALES].xlsx`.

---

# Tarea 4. Guardar el prompt en la Galería de indicaciones

## Objetivo

Dejar el prompt listo para ejecutarse periódicamente.

## Instrucciones

### Paso 1

El instructor pasa el puntero sobre su mensaje con el prompt de la Tarea 1 y selecciona la opción **Guardar indicación** (el nombre puede variar).

### Paso 2

Asignar el nombre `Consolidar compromisos INT-MDV` y guardar.

### Paso 3

Abrir la [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts), localizar la indicación en **Mis indicaciones** y mostrar cómo volver a ejecutarla cambiando el periodo.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué compromisos son propios?" | Solo los de Coordinación de la intervención, unificados |
| Caso 2 | Preguntar: "¿Qué venció antes del 6 de noviembre?" | Verificación de grúa (vencida el 05-nov); el cronograma aparece reprogramado al 07-nov y no vencido |
| Caso 3 | Abrir la Galería de indicaciones | La indicación guardada aparece en Mis indicaciones |
| Caso adversarial | Pedir: "Asigna tú un responsable al vocero" | Copilot indica que la fuente no define responsable y lo marca como pendiente |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Tabla consolidada con reunión de origen, responsable, fecha, estado, prioridad y acción.
- Duplicados unificados.
- Prompt guardado en la Galería de indicaciones.

**Entregable:** vista consolidada de acuerdos y compromisos con reunión de origen, responsable, fecha, estado, prioridad y acción de seguimiento (`Vista_Compromisos_INT-MDV_[INICIALES].xlsx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 5](../../images/p05-resultado.svg)

---

# Solución de Problemas

## Problema 1: Copilot no encuentra las páginas de Loop

### Síntomas

Al escribir `/` no aparecen las notas.

### Causa

Las páginas no están compartidas o indexadas.

### Solución

1. Abrir cada página de Loop una vez.
2. Confirmar que estén compartidas con el usuario.
3. Volver a ejecutar el prompt.

---

## Problema 2: No aparece la opción para guardar la indicación

### Síntomas

No se muestra Guardar indicación en el mensaje.

### Causa

Función no disponible en el cliente o en la versión.

### Solución

1. Probar en la aplicación web de Microsoft 365 Copilot.
2. Abrir la Galería de indicaciones y crear la indicación desde allí.
3. Registrar la limitación.

---

# Limpieza

1. Conservar la indicación guardada; se reutiliza en la Práctica 6 (KR3.1 del OKR).
2. Conservar la vista en `Entregables`.

---

# Resumen

Durante esta práctica se realizó:

- Consolidación de compromisos de tres reuniones con un prompt reutilizable.
- Detección de duplicados y vista de atención.
- Guardado del prompt en la Galería de indicaciones.

Como resultado se obtuvo:

- Una vista consolidada de compromisos lista para dar seguimiento.
- Un prompt reutilizable para actualizar la vista periódicamente.

---

# Recursos Opcionales

- [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts)
- [Facilitator en Microsoft Teams](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams)
- [Copilot en reuniones de Teams](https://support.microsoft.com/es-es/teams/copilot/catch-up-on-meetings-with-microsoft-365-copilot-in-teams)

---

[⬅ Anterior: Práctica 4](../../Capitulo02/Practica04/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 6 ➡](../../Capitulo02/Practica06/README.md)
