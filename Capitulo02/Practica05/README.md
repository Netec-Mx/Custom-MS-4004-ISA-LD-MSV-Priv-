# Práctica 5. Consolidar acuerdos y compromisos de múltiples reuniones

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Consolidar con un prompt reutilizable los acuerdos y compromisos de varias reuniones, conservando la reunión de origen.
- Distinguir compromisos propios, asignados a otras personas y sin responsable o fecha.
- Organizar los compromisos por estado y prioridad e identificar atrasos y próximos vencimientos.
- Detectar compromisos duplicados entre reuniones y guardar el prompt en la Galería de indicaciones.

<img src="../../images/p05-objetivo.svg" alt="Mapa visual de la práctica 5" width="720"/>

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Copilot |
| Documento de fuentes | [Actas_Reuniones_INT-MDV.docx](recursos/Actas_Reuniones_INT-MDV.docx) (tres reuniones, compromisos y transcripción) |
| Rol "propio" en el escenario | `Coordinación de la intervención` (la persona que ejecuta el prompt) |
| Fecha de referencia | 10 de noviembre de 2026 |

## Instrucciones

Durante la planeación de INT-MDV-2026 se realizaron tres reuniones (20-oct, 27-oct y 03-nov). Los acuerdos y compromisos están distribuidos entre actas de reunión y una transcripción; antes del curso se disponen en Loop para su consulta conjunta. Un **prompt reutilizable** permite a Copilot consolidar acuerdos, decisiones, responsables, fechas y pendientes, detectar duplicados y guardar la indicación en la Galería de indicaciones para ejecutarla periódicamente.

### Tarea 1. Presentar las fuentes y el prompt reutilizable (3 min)

**Paso 1.** Abrir [Microsoft Copilot](https://www.microsoft365.com/), seleccionar **Copilot Chat > Nuevo chat** y comprobar que se tiene acceso a las páginas de Loop de las reuniones del escenario. El documento de fuentes permite crear páginas de Loop antes de la sesión; esas páginas no equivalen a notas emitidas por Facilitator durante una reunión.

**Paso 2.** Escribir `/` en el cuadro de mensaje y localizar, si se han compartido con tu cuenta, las páginas de Loop `Notas INT-MDV 27-oct` y `Notas INT-MDV 03-nov` y el documento `Actas_Reuniones_INT-MDV.docx`.

- **Comprobación:** las tres fuentes en la lista de sugerencias.
- **Si no aparece:** abrir cada página de Loop una vez desde su enlace para que se indexe y repetir.

**Paso 3.** Identificar las cinco partes del prompt reutilizable: **periodo** (20-oct a 10-nov), **fuentes** (notas de Loop y transcripciones), **campos** (descripción, reunión, responsable, fecha), **clasificación** (propio, asignado o sin responsable) y **formato** (tabla). copiar el siguiente prompt para ejecutarlo en Copilot Chat:

```text
Revisa las páginas de notas en Loop y la transcripción de las reuniones del proyecto INT-MDV-2026
realizadas entre el 20 de octubre y el 10 de noviembre de 2026. Consolida en una tabla todos los acuerdos,
decisiones y compromisos con: descripción, reunión de origen (fecha), responsable, fecha comprometida y tipo:
"Propio" (Coordinación de la intervención), "Asignado a otra persona" o "Sin responsable o sin fecha".
No inventes responsables ni fechas. Fecha de referencia: 10 de noviembre de 2026.
```

### Tarea 2. Consolidar y clasificar los compromisos (5 min)

**Paso 1.** Pegar el prompt de la Tarea 1 en Copilot Chat, adjuntar con `/` las dos páginas Loop de la preparación y el documento de fuentes, y enviarlo. Si una página no está accesible, consultar el documento de fuentes y distinguir el texto proporcionado del recuperado desde Loop.

- **Comprobación:** una tabla con todos los acuerdos y compromisos de las tres reuniones, con su reunión de origen.

**Paso 2.** Pegar el siguiente prompt en la misma conversación:

```text
Agrega las columnas Estado (Cumplido, Vencido, Próximo a vencer en 7 días, Sin fecha) y Prioridad (Alta, Media, Baja),
y una columna "Acción de seguimiento". Ordena por estado y prioridad.
```

- **Comprobación:** la tabla con tres columnas nuevas (Estado, Prioridad y Acción de seguimiento), ordenada por estado.

**Paso 3.** Revisar en grupo al menos estos cinco casos del material: **verificación de grúa** (vencida el 05-nov), **permiso de aceite** (vence el 10-nov), **notificación a clientes** (vence el 14-nov), **vocero ante medios** (sin responsable) y **plan con comunidades** (sin fecha).

- **Si no aparece:** preguntar: *"¿Qué estado tiene la verificación de la grúa al 10 de noviembre?"*

### Tarea 3. Generar la vista de atención y detectar duplicados (4 min)

**Paso 1.** Pegar el siguiente prompt:

```text
Identifica compromisos que aparezcan en diferentes reuniones y que correspondan a la misma actividad.
Unifícalos en una sola fila indicando todas las reuniones de origen y la fecha vigente.
Luego muestra solo los compromisos que requieren atención: atrasados, próximos a vencer y sin responsable.
```

- **Comprobación:** una sola fila para el cronograma compartido en varias reuniones, verificando la fecha vigente del 07-nov contra las fuentes, seguida de la vista de atención.

**Paso 2.** Comprobar si la actividad unificada corresponde al rol del caso de **Coordinación de la intervención**, sin atribuirla automáticamente al usuario real y que la vista de atención solo muestre lo atrasado, lo próximo a vencer o lo que no tiene responsable.

**Paso 3.** Seleccionar **Copiar** debajo de la tabla final, abrir Excel (escritorio o [office.com](https://www.office.com/) > **Excel > Libro en blanco**), hacer clic en la celda **A1** y pegar con **Ctrl+V**.

- **Comprobación:** la tabla en columnas de Excel.
- **Alternativa:** Si todo queda en una sola columna, usar **Datos > Texto en columnas** o pegar con **Ctrl+Shift+V**.

**Paso 4.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Vista_Compromisos_INT-MDV_[INICIALES].xlsx`: en Excel de escritorio, **Archivo > Guardar como**; en Excel para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

### Tarea 4. Guardar el prompt en la Galería de indicaciones (3 min)

**Paso 1.** Localizar en el chat el mensaje con el prompt de la Tarea 1, pasar el puntero sobre él y seleccionar la opción **Guardar indicación** (puede mostrarse como un icono de marcador o en el menú **…**).

- **Comprobación:** un cuadro para nombrar la indicación.

**Paso 2.** Escribir el nombre `Consolidar compromisos INT-MDV` y seleccionar **Guardar**; comprobar la confirmación del servicio.

**Paso 3.** Abrir la [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts), seleccionar **Tus indicaciones / Your prompts** y localizar `Consolidar compromisos INT-MDV`. Seleccionarla, cambiar el periodo en el texto (por ejemplo, *"entre el 7 y el 13 de noviembre"*) y ejecutarla de nuevo.

- **Comprobación:** la indicación guardada lista para reutilizarse.
- **Alternativa:** Si no existe la opción Guardar indicación, crearla desde la galería con **Crear indicación** y pegar el texto.

### Resultado esperado

<img src="../../images/p05-resultado.svg" alt="Resultado esperado de la práctica 5" width="720"/>


- Tabla consolidada con reunión de origen, responsable, fecha, estado, prioridad y acción.
- Duplicados unificados.
- Prompt guardado en la Galería de indicaciones.

**Entregable:** vista consolidada de acuerdos y compromisos con reunión de origen, responsable, fecha, estado, prioridad y acción de seguimiento (`Vista_Compromisos_INT-MDV_[INICIALES].xlsx`).
