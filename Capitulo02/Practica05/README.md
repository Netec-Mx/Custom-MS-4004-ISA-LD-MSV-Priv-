# Práctica 5. Consolidar acuerdos y compromisos de múltiples reuniones

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Microsoft 365 Copilot, Facilitator (Loop) y Galería de indicaciones · 📄 **Entregable:** Vista consolidada de acuerdos y compromisos con origen, responsable, fecha, estado, prioridad y acción

## Descripción

Durante la planeación de INT-MDV-2026 se realizaron tres reuniones (20-oct, 27-oct y 03-nov). Los acuerdos y compromisos quedaron repartidos entre notas de Facilitator en Loop y una transcripción. El instructor mostrará cómo un **prompt reutilizable** permite a Copilot consolidar acuerdos, decisiones, responsables, fechas y pendientes, detectar duplicados y guardar la indicación en la Galería de indicaciones para ejecutarla periódicamente.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Consolidar con un prompt reutilizable los acuerdos y compromisos de varias reuniones, conservando la reunión de origen.
- Distinguir compromisos propios, asignados a otras personas y sin responsable o fecha.
- Organizar los compromisos por estado y prioridad e identificar atrasos y próximos vencimientos.
- Detectar compromisos duplicados entre reuniones y guardar el prompt en la Galería de indicaciones.

<img src="../../images/p05-objetivo.svg" alt="Diagrama de la Práctica 5" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Copilot |
| Archivos de la práctica | [Notas_Facilitator_2026-10-27.docx](recursos/Notas_Facilitator_2026-10-27.docx)<br>[Notas_Facilitator_2026-11-03.docx](recursos/Notas_Facilitator_2026-11-03.docx)<br>[Transcripcion_Planeacion_2026-10-20.docx](recursos/Transcripcion_Planeacion_2026-10-20.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica05/` |
| Rol "propio" en el escenario | `Coordinación de la intervención` (la persona que ejecuta el prompt) |
| Fecha de referencia | 6 de noviembre de 2026 |
| Nombre del entregable | `Vista_Compromisos_INT-MDV_[INICIALES].xlsx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

> **Nota:** Práctica conducida por el instructor (según el temario). El instructor ejecuta cada paso en pantalla; los participantes siguen con la misma indicación y, si el instructor compartió con ellos las páginas de Loop y la transcripción, la ejecutan en paralelo.

---

## Tarea 1. Presentar las fuentes y el prompt reutilizable (3 min)

**Objetivo:** Que todos tengan copiado el prompt reutilizable y entiendan sus 5 partes: periodo, fuentes, campos, clasificación y formato.

**Por qué:** Un prompt bien estructurado puede reutilizarse cada semana cambiando solo el periodo. **Rol del participante:** copiar el prompt en un documento propio.

**Paso 1.** **Instructor:** abrir [m365.cloud.microsoft](https://m365.cloud.microsoft/), seleccionar **Copilot** > **Nuevo chat** y proyectar la pantalla. **Participantes:** abrir un **Documento en blanco** de Word para copiar el prompt.

**Paso 2.** **Instructor:** escribir `/` y mostrar que aparecen las páginas de Loop `Notas Facilitator INT-MDV 27-oct` y `Notas Facilitator INT-MDV 03-nov` y el archivo `Transcripcion_Planeacion_2026-10-20.docx`.

- **Qué verás:** las tres fuentes en la lista de sugerencias.
- **Si no ocurre así:** abrir cada página de Loop una vez desde su enlace para que se indexe y repetir.

**Paso 3.** Explicar las cinco partes del prompt reutilizable: **periodo** (20-oct a 6-nov), **fuentes** (notas de Loop y transcripciones), **campos** (descripción, reunión, responsable, fecha), **clasificación** (propio, asignado o sin responsable) y **formato** (tabla). **Participantes:** copiar el siguiente prompt en su documento:

```text
Revisa las notas de Facilitator en Loop y las transcripciones de las reuniones del proyecto INT-MDV-2026
realizadas entre el 20 de octubre y el 6 de noviembre de 2026. Consolida en una tabla todos los acuerdos,
decisiones y compromisos con: descripción, reunión de origen (fecha), responsable, fecha comprometida y tipo:
"Propio" (Coordinación de la intervención), "Asignado a otra persona" o "Sin responsable o sin fecha".
No inventes responsables ni fechas. Fecha de referencia: 6 de noviembre de 2026.
```

**Al terminar esta tarea debes tener:**

- ✔ El prompt copiado en un documento propio.
- ✔ Identificadas sus 5 partes.

---

## Tarea 2. Consolidar y clasificar los compromisos (5 min)

**Objetivo:** Ver la tabla consolidada con estado, prioridad y acción de seguimiento de cada compromiso.

**Por qué:** Revisar reunión por reunión oculta los atrasos; consolidar muestra qué está vencido y qué vence pronto. **Rol del participante:** comprobar en la pantalla del instructor (o en su propia ejecución) los 5 compromisos esperados.

**Paso 1.** **Instructor:** pegar el prompt de la Tarea 1 en el chat, insertar las tres fuentes con `/` al final del prompt y enviarlo. **Participantes con acceso a las páginas de Loop:** hacer lo mismo en su propio chat.

- **Qué verás:** una tabla con todos los acuerdos y compromisos de las tres reuniones, con su reunión de origen.

**Paso 2.** **Instructor:** pegar el siguiente prompt en la misma conversación:

```text
Agrega las columnas Estado (Cumplido, Vencido, Próximo a vencer en 7 días, Sin fecha) y Prioridad (Alta, Media, Baja),
y una columna "Acción de seguimiento". Ordena por estado y prioridad.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** la tabla con tres columnas nuevas (Estado, Prioridad y Acción de seguimiento), ordenada por estado.

**Paso 3.** Revisar en grupo los cinco casos esperados: **verificación de grúa** (vencida el 05-nov), **permiso de aceite** (vence el 10-nov), **notificación a clientes** (vence el 14-nov), **vocero ante medios** (sin responsable) y **plan con comunidades** (sin fecha).

- **Si no ocurre así:** preguntar: *"¿Qué estado tiene la verificación de la grúa al 6 de noviembre?"*

**Al terminar esta tarea debes tener:**

- ✔ Identificados el compromiso vencido, los dos próximos a vencer y los dos sin responsable o sin fecha.

---

## Tarea 3. Generar la vista de atención y detectar duplicados (4 min)

**Objetivo:** Tener una sola fila por actividad y una vista que muestre solo lo atrasado, próximo a vencer o sin responsable.

**Por qué:** La misma tarea registrada en tres reuniones parece tres pendientes distintos; unificar evita duplicar el seguimiento. **Rol del participante:** guardar la vista final en su carpeta `Entregables`.

**Paso 1.** **Instructor:** pegar el siguiente prompt:

```text
Identifica compromisos que aparezcan en diferentes reuniones y que correspondan a la misma actividad.
Unifícalos en una sola fila indicando todas las reuniones de origen y la fecha vigente.
Luego muestra solo los compromisos que requieren atención: atrasados, próximos a vencer y sin responsable.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una sola fila para la actividad del cronograma con sus tres reuniones de origen (20-oct, 27-oct y 03-nov) y la fecha vigente del 07-nov, seguida de la vista de atención.

**Paso 2.** Comprobar que la actividad unificada aparezca como compromiso **propio** de Coordinación de la intervención y que la vista de atención solo muestre lo atrasado, lo próximo a vencer o lo que no tiene responsable.

**Paso 3.** **Todos:** seleccionar **Copiar** debajo de la tabla final, abrir Excel (escritorio o [office.com](https://www.office.com/) > **Excel > Libro en blanco**), hacer clic en la celda **A1** y pegar con **Ctrl+V**.

- **Qué verás:** la tabla en columnas de Excel.
- **Alternativa:** Si todo queda en una sola columna, usar **Datos > Texto en columnas** o pegar con **Ctrl+Shift+V**.

**Paso 4.** Guardar el archivo: en Excel de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Vista_Compromisos_INT-MDV_[INICIALES].xlsx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Excel para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Vista_Compromisos_INT-MDV_[INICIALES].xlsx` en la barra de título y el estado **Guardado**.

**Al terminar esta tarea debes tener:**

- ✔ La actividad del cronograma unificada en una fila.
- ✔ `Vista_Compromisos_INT-MDV_[INICIALES].xlsx` guardada.

---

## Tarea 4. Guardar el prompt en la Galería de indicaciones (3 min)

**Objetivo:** Tener el prompt guardado como `Consolidar compromisos INT-MDV` en **Mis indicaciones**.

**Por qué:** Guardarlo permite actualizar la vista cada semana en segundos. **Rol del participante:** guardar también el prompt en su propia galería.

**Paso 1.** **Instructor:** en el chat, subir hasta el mensaje con el prompt de la Tarea 1, pasar el puntero sobre él y seleccionar la opción **Guardar indicación** (puede mostrarse como un icono de marcador o en el menú **…**).

- **Qué verás:** un cuadro para nombrar la indicación.

**Paso 2.** Escribir el nombre `Consolidar compromisos INT-MDV` y seleccionar **Guardar**. **Participantes:** repetir en su propio chat con el prompt que copiaron.

**Paso 3.** Abrir la [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts), seleccionar **Mis indicaciones** y localizar `Consolidar compromisos INT-MDV`. Mostrar cómo seleccionarla, cambiar el periodo en el texto (por ejemplo, *"entre el 7 y el 13 de noviembre"*) y ejecutarla de nuevo.

- **Qué verás:** la indicación guardada lista para reutilizarse.
- **Alternativa:** Si no existe la opción Guardar indicación, crearla desde la galería con **Crear indicación** y pegar el texto.

**Al terminar esta tarea debes tener:**

- ✔ La indicación visible en la Galería de indicaciones.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué compromisos son propios?" | Solo los de Coordinación de la intervención, unificados |
| Caso 2 | Preguntar: "¿Qué venció antes del 6 de noviembre?" | Verificación de grúa (vencida el 05-nov); el cronograma aparece reprogramado al 07-nov y no vencido |
| Caso 3 | Abrir la Galería de indicaciones | La indicación guardada aparece en Mis indicaciones |
| Caso adversarial | Pedir: "Asigna tú un responsable al vocero" | Copilot indica que la fuente no define responsable y lo marca como pendiente |

## Resultado esperado

- Tabla consolidada con reunión de origen, responsable, fecha, estado, prioridad y acción.
- Duplicados unificados.
- Prompt guardado en la Galería de indicaciones.

**Entregable:** vista consolidada de acuerdos y compromisos con reunión de origen, responsable, fecha, estado, prioridad y acción de seguimiento (`Vista_Compromisos_INT-MDV_[INICIALES].xlsx`).

<img src="../../images/p05-resultado.svg" alt="Resultado final de la Práctica 5" width="640"/>

## Solución de problemas

**Copilot no encuentra las páginas de Loop**
- *Síntoma:* Al escribir `/` no aparecen las notas.
- *Causa:* Las páginas no están compartidas o indexadas.
- *Solución:* (1) Abrir cada página de Loop una vez. (2) Confirmar que estén compartidas con el usuario. (3) Volver a ejecutar el prompt.

**No aparece la opción para guardar la indicación**
- *Síntoma:* No se muestra Guardar indicación en el mensaje.
- *Causa:* Función no disponible en el cliente o en la versión.
- *Solución:* (1) Probar en la aplicación web de Microsoft 365 Copilot. (2) Abrir la Galería de indicaciones y crear la indicación desde allí. (3) Registrar la limitación.

## Limpieza

- Conservar la indicación guardada; se reutiliza en la Práctica 6 (KR3.1 del OKR).
- Conservar la vista en `Entregables`.

## Recursos opcionales

- [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts)
- [Facilitator en Microsoft Teams](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams)
- [Copilot en reuniones de Teams](https://support.microsoft.com/es-es/teams/copilot/catch-up-on-meetings-with-microsoft-365-copilot-in-teams)

<sub>Complejidad: Intermedia · Nivel de Bloom: Aplicar</sub>

---

[⬅ Anterior: Práctica 4](../../Capitulo02/Practica04/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 6 ➡](../../Capitulo02/Practica06/README.md)
