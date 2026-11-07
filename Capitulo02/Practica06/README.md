# Práctica 6. Convertir la actividad de Microsoft 365 en una actualización ejecutiva de estado

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Agente de actualización de estado · 📄 **Entregable:** Informe de estado semanal, alineación con OKR y documento de logros en Word

## Descripción

Cada semana el participante debe informar a su responsable qué logró. Su actividad está repartida en Outlook, Teams, reuniones y archivos, incluida la que generó en las prácticas anteriores de este curso. Usará el Agente de actualización de estado para producir un informe semanal trazable, vincularlo con los OKR del equipo y transformar los resultados en un documento de logros en Word listo para revisión.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Generar con el Agente de actualización de estado un informe semanal trazable a fuentes de Microsoft 365.
- Vincular actividades y resultados con objetivos/OKR, diferenciando progreso observado de evidencia insuficiente.
- Generar un documento de logros y su variante compartible para el responsable.
- Distinguir cuándo usar un informe de estado y cuándo un documento de logros.

<img src="../../images/p06-objetivo.svg" alt="Diagrama de la Práctica 6" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Agente de actualización de estado |
| Archivos de la práctica | [OKR_Equipo_T4_2026.docx](recursos/OKR_Equipo_T4_2026.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica06/` |
| Periodo a analizar | Últimos 7 días |
| Nombre del entregable | `Informe_Estado_[INICIALES].docx` y `Documento_Logros_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Generar el informe de estado semanal (5 min)

**Objetivo:** Tener un informe de los últimos 7 días con logros, actividades en curso, colaboración y prioridades, y la fuente de cada punto.

**Por qué:** Escribir un informe de estado de memoria toma tiempo y omite cosas. El agente lo construye desde la actividad real, pero hay que verificarlo.

**Paso 1.** Abrir **Microsoft Edge**, escribir [m365.cloud.microsoft](https://m365.cloud.microsoft/) en la barra de direcciones y presionar **Enter**. Si se solicita, iniciar sesión con su cuenta corporativa.

- **Qué verás:** la página de inicio de Microsoft 365 Copilot con un cuadro de mensaje al centro y un panel a la izquierda.
- **Alternativa:** Si aparece la página de inicio de Microsoft 365 sin chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Agentes**. Escribir `Agente de actualización de estado` en el cuadro de búsqueda de agentes y hacer clic en el resultado.

- **Qué verás:** el nombre **Agente de actualización de estado** encima del cuadro de mensaje y, a veces, sugerencias de inicio. A partir de aquí, todo lo que escriba lo procesa este agente.
- **Si no ocurre así:** seleccionar **Todos los agentes** (u **Obtener agentes**) y buscarlo de nuevo. Si sigue sin aparecer, avisar al instructor: el agente no está habilitado para su cuenta.

**Paso 3.** Pegar el siguiente prompt y enviarlo:

```text
Genera mi informe de estado de los últimos 7 días a partir de mi actividad en Outlook, Teams, reuniones,
SharePoint y OneDrive. Organízalo en: logros relevantes, actividades en curso, colaboración y apoyo,
y prioridades para la siguiente semana. Indica la fuente de cada punto y no incluyas nada que no puedas sustentar.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** un informe con cuatro secciones (logros relevantes, actividades en curso, colaboración y apoyo, y prioridades) y referencias a correos, chats, reuniones o archivos.

**Paso 4.** Hacer clic en dos referencias del informe (correo, chat o archivo) y comprobar que lo que dice el informe coincide con la fuente.

- **Alternativa:** Si un punto no tiene fuente o la fuente no lo respalda, escribir: *"Elimina o marca como no verificable el punto sobre [tema]"*.

**Al terminar esta tarea debes tener:**

- ✔ Informe con 4 secciones.
- ✔ Dos fuentes abiertas y verificadas.
- ✔ Nada incluido sin fuente.

---

## Tarea 2. Alinear actividades con los OKR (4 min)

**Objetivo:** Tener una tabla con los 6 resultados clave (KR) del equipo, el progreso observado y su evidencia, o "evidencia insuficiente".

**Por qué:** Un informe de actividades no dice si se avanza en los objetivos. Vincularlos muestra dónde falta evidencia.

**Paso 1.** Pegar el siguiente prompt (insertar `/OKR_Equipo_T4_2026` con el selector de archivos):

```text
Vincula las actividades y resultados del informe con cada objetivo y resultado clave de /OKR_Equipo_T4_2026.
Para cada KR indica: progreso observado con evidencia, o "evidencia insuficiente" si no hay actividad que lo respalde.
```

- **Cómo insertar los archivos:** en el prompt, cada texto que empieza con `/` es un archivo. Borrar ese texto, escribir `/` seguido de las primeras letras del nombre del archivo y seleccionarlo en la lista que aparece; el archivo queda resaltado como un vínculo. Si no aparece en la lista, seleccionar el botón **+** (Agregar) > **Cargar desde OneDrive** > `Laboratorio_Copilot_ISA/Practica06` y elegirlo.
- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una tabla con los 3 objetivos y sus 6 resultados clave (KR1.1 a KR3.2), con el progreso observado y la evidencia, o "evidencia insuficiente".

**Paso 2.** Comprobar tres resultados: **KR2.1** (análisis de desviaciones) con evidencia de la Práctica 2, **KR3.1** (prompts en la galería) con evidencia de la Práctica 5 y **KR3.2** (agente personalizado) con **evidencia insuficiente**, porque ese agente se crea en la Práctica 13.

- **Si no ocurre así:** preguntar: *"¿Qué evidencia tienes para KR3.2?"*

**Al terminar esta tarea debes tener:**

- ✔ Los 6 KR en una tabla.
- ✔ KR2.1 y KR3.1 con evidencia; KR3.2 con evidencia insuficiente.

---

## Tarea 3. Crear el documento de logros y su variante compartible (4 min)

**Objetivo:** Tener guardados dos documentos: el informe de estado con la alineación a OKR y el documento de logros con su variante para el responsable.

**Por qué:** El documento de logros comunica impacto, no tareas, y sirve para evaluaciones y reconocimiento.

**Paso 1.** Pegar el siguiente prompt:

```text
Transforma los principales resultados del periodo en un documento de logros. Para cada logro separa:
logro, impacto y colaboración. Luego genera una variante breve y compartible dirigida a mi responsable.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** un documento de logros con tres partes por logro (logro, impacto, colaboración) y, al final, una versión breve dirigida al responsable.

**Paso 2.** Abrir una pestaña nueva, ingresar a [office.com](https://www.office.com/) y seleccionar **Word > Documento en blanco** (o abrir Word de escritorio > **Documento en blanco**). Regresar a Copilot y, debajo de el informe de estado (Tarea 1) y la tabla de OKR (Tarea 2), seleccionar el icono **Copiar**. Volver a Word, hacer clic en el documento y pegar con **Ctrl+V**.

- **Qué verás:** el texto con su formato (títulos, tablas y viñetas) dentro del documento.
- **Alternativa:** Si la tabla se pega como texto plano, pegar con **Ctrl+Shift+V** > **Mantener formato de origen**, o pedir a Copilot: *"Entrega la tabla en formato de tabla"* y copiarla de nuevo.

**Paso 3.** Guardar el archivo: en Word de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Informe_Estado_[INICIALES].docx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Word para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Informe_Estado_[INICIALES].docx` en la barra de título y el estado **Guardado**.

**Paso 4.** Crear otro **Documento en blanco** en Word, copiar y pegar el documento de logros y su variante compartible y repetir el guardado con el nombre `Documento_Logros_[INICIALES].docx`.

- **Importante:** no compartir el documento; queda listo para revisión.

**Al terminar esta tarea debes tener:**

- ✔ `Informe_Estado_[INICIALES].docx` guardado.
- ✔ `Documento_Logros_[INICIALES].docx` con logro, impacto y colaboración, y la variante para el responsable.

---

## Tarea 4. Comparar formatos (2 min)

**Objetivo:** Poder explicar en una línea cuándo conviene cada formato.

**Por qué:** Elegir el formato correcto evita enviar detalle operativo a quien solo necesita conocer el impacto.

**Paso 1.** Abrir `Informe_Estado_[INICIALES].docx` y, al final, agregar el título **Cuándo usar cada formato** con dos líneas: una para el **informe de estado** (seguimiento semanal de actividades y prioridades) y otra para el **documento de logros** (comunicar impacto y colaboración, por ejemplo en evaluaciones). Guardar con **Ctrl+S**.

**Al terminar esta tarea debes tener:**

- ✔ La sección "Cuándo usar cada formato" agregada.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Abrir dos fuentes citadas | Cada fuente respalda el punto del informe |
| Caso 2 | Preguntar por KR3.2 | Indica evidencia insuficiente |
| Caso 3 | Revisar el documento de logros | Cada logro separa logro, impacto y colaboración |
| Caso adversarial | Pedir: "Agrega que lideré la intervención del 28 de noviembre" | El agente indica que no hay actividad que lo respalde |

## Resultado esperado

- Informe de estado semanal con fuentes.
- Alineación de actividades con OKR.
- Documento de logros en Word con variante compartible.

**Entregable:** informe de estado semanal, alineación con objetivos/OKR (`Informe_Estado_[INICIALES].docx`) y documento de logros en Word listo para revisión (`Documento_Logros_[INICIALES].docx`).

<img src="../../images/p06-resultado.svg" alt="Resultado final de la Práctica 6" width="640"/>

## Solución de problemas

**El informe sale casi vacío**
- *Síntoma:* Pocas actividades listadas.
- *Causa:* Poca actividad en el periodo o datos aún no indexados.
- *Solución:* (1) Ampliar el periodo a 14 días. (2) Confirmar con el instructor que se sembró la actividad. (3) Repetir la Tarea 1.

**El agente incluye actividades no realizadas**
- *Síntoma:* Aparecen logros sin fuente.
- *Causa:* Inferencia del modelo.
- *Solución:* (1) Pedir la fuente de cada punto. (2) Solicitar eliminar lo no verificable. (3) Revisar manualmente antes de compartir.

## Limpieza

- No compartir el documento de logros; queda para revisión.
- Conservar los archivos en `Entregables`.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Aplicar</sub>

---

[⬅ Anterior: Práctica 5](../../Capitulo02/Practica05/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 7 ➡](../../Capitulo02/Practica07/README.md)
