# Práctica 4. Antes de la reunión: prepararse con Facilitator y Copilot

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Microsoft 365 Copilot en Teams y Facilitator · 📄 **Entregable:** Guía de preparación de la reunión

## Descripción

El participante tiene programada la reunión **"Revisión de preparación INT-MDV-2026"** para la intervención en la Subestación Mirador del Valle (ficticia). La información está dispersa: parte en la invitación, parte en correos de Operación, Gestión Ambiental y Comercial, y parte en archivos de OneDrive. Usará Copilot y las capacidades de Teams y Facilitator para preparar el objetivo, la agenda, el contexto, las preguntas y las decisiones difíciles de la reunión.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Recuperar con Copilot la información de una reunión distribuida entre invitación, correos y archivos en la nube.
- Preparar objetivo, agenda, contexto necesario, preguntas relevantes y asuntos por resolver.
- Identificar posibles desacuerdos y decisiones difíciles y preparar preguntas para conducirlos.
- Confirmar que Facilitator esté disponible para la reunión.

<img src="../../images/p04-objetivo.svg" alt="Diagrama de la Práctica 4" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Microsoft Teams > Calendario |
| Archivos de la práctica | [Plan_Intervencion_Mirador_del_Valle.docx](recursos/Plan_Intervencion_Mirador_del_Valle.docx)<br>[Matriz_Riesgos_Intervencion.xlsx](recursos/Matriz_Riesgos_Intervencion.xlsx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica04/` |
| Reunión | `Revisión de preparación INT-MDV-2026` |
| Correos | Asuntos que inician con `INT-MDV` |
| Fecha de referencia | 6 de noviembre de 2026 |
| Nombre del entregable | `Guia_Reunion_INT-MDV_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Revisar la reunión y reunir la información disponible (4 min)

**Objetivo:** Confirmar que Copilot encuentra las fuentes de la reunión: la invitación, los 3 correos y los 2 archivos.

**Por qué:** La información de una reunión rara vez está en un solo lugar. Si falta una fuente, la preparación queda incompleta.

**Paso 1.** Abrir **Microsoft Teams** (aplicación de escritorio o [teams.microsoft.com](https://teams.microsoft.com/)) y seleccionar **Calendario** en la barra izquierda.

**Paso 2.** Buscar en el calendario la reunión `Revisión de preparación INT-MDV-2026` y hacer doble clic para abrir sus detalles.

- **Qué verás:** la invitación con la descripción ("Revisaremos el estado de preparación…") y el adjunto `Plan_Intervencion_Mirador_del_Valle.docx`.
- **Si no ocurre así:** usar la búsqueda del calendario con la palabra `INT-MDV`. Si no existe, avisar al instructor.

**Paso 3.** En los detalles de la reunión, buscar la opción de Copilot para prepararse (por ejemplo, **Preparar con Copilot** o el icono de Copilot) y seleccionarla.

- **Qué verás:** un resumen generado por Copilot con el contexto de la reunión y archivos o correos relacionados.
- **Alternativa:** Si la opción no existe, cerrar los detalles, seleccionar **Copilot** en la barra izquierda de Teams y continuar con el paso siguiente.

**Paso 4.** En el chat de Copilot de Teams, pegar el siguiente prompt (borrar el texto que inicia con `/` y seleccionar la reunión y cada archivo de la lista que aparece al escribir `/`):

```text
¿Qué información existe sobre /Revisión de preparación INT-MDV-2026? Revisa la invitación, mis correos con asunto INT-MDV
y los archivos /Plan_Intervencion_Mirador_del_Valle y /Matriz_Riesgos_Intervencion. Indica la fuente de cada dato.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una lista de fuentes con lo que aporta cada una.

**Paso 5.** Comprobar que aparezcan las cinco fuentes: correo de **Operación** (ventana de 30 horas), correo de **Gestión Ambiental** (permiso en trámite), correo de **Comercial** (cliente sin acuse), el **plan** y la **matriz de riesgos**.

- **Si no ocurre así:** escribir `/` y el asunto del correo que falte (por ejemplo, `/INT-MDV permiso`), seleccionarlo y preguntar: *"¿Qué dice este correo?"*

**Al terminar esta tarea debes tener:**

- ✔ Las 5 fuentes identificadas con lo que aporta cada una.

---

## Tarea 2. Preparar objetivo, agenda, contexto y preguntas (6 min)

**Objetivo:** Tener el objetivo, una agenda de 45 minutos con tiempos, el contexto, las preguntas por área y los asuntos por resolver.

**Por qué:** Una reunión sin agenda ni preguntas preparadas termina sin decisiones. La diferencia entre 36 y 30 horas debe resolverse en esta sesión.

**Paso 1.** Pegar el siguiente prompt en la misma conversación:

```text
Prepara para esta reunión: 1) objetivo en una frase, 2) agenda de 45 minutos con tiempos,
3) contexto que todos deben conocer, 4) preguntas relevantes por área y 5) asuntos que deben resolverse durante la reunión.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** cinco secciones: objetivo, agenda con tiempos que suman 45 minutos, contexto, preguntas por área y asuntos por resolver.

**Paso 2.** Revisar el **contexto**: debe mencionar la ventana planeada de **36 h** frente a las **30 h** aprobadas preliminarmente, el permiso ambiental con respuesta estimada el **25-nov** y el cliente que pidió reprogramar.

- **Si no ocurre así:** escribir: *"Agrega al contexto lo que dicen los correos de Operación, Gestión Ambiental y Comercial"*.

**Paso 3.** Revisar la **agenda**: los tres asuntos críticos (ventana, permiso y cliente) deben tener tiempo asignado.

- **Si no ocurre así:** escribir: *"Ajusta la agenda para dar 10 minutos a [asunto]"*.

**Al terminar esta tarea debes tener:**

- ✔ Objetivo en una frase.
- ✔ Agenda de 45 minutos con los 3 asuntos críticos.
- ✔ Preguntas por área.

---

## Tarea 3. Anticipar desacuerdos y decisiones difíciles (3 min)

**Objetivo:** Tener identificados los desacuerdos probables y dos preguntas para conducir cada uno.

**Por qué:** Las decisiones difíciles (reprogramar, re-secuenciar, designar vocero) generan tensión entre áreas; las preguntas preparadas ayudan a llegar a una decisión.

**Paso 1.** Pegar el siguiente prompt:

```text
¿Qué desacuerdos o decisiones difíciles podrían surgir en esta reunión? Para cada uno indica las posiciones probables
de las áreas y propón dos preguntas para conducir la conversación hacia una decisión.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una lista de desacuerdos o decisiones difíciles, con la posición probable de cada área y dos preguntas por cada uno.

**Paso 2.** Confirmar que aparezcan al menos tres: **mantener o reprogramar la fecha** ante la solicitud del cliente, **re-secuenciar actividades** para 30 horas y **designar al vocero** ante medios.

- **Si no ocurre así:** preguntar directamente: *"¿Qué desacuerdo podría haber sobre [tema] y cómo lo conduzco?"*

**Al terminar esta tarea debes tener:**

- ✔ Al menos 3 desacuerdos con las posiciones probables de las áreas.
- ✔ Dos preguntas por desacuerdo.

---

## Tarea 4. Guardar la guía y confirmar Facilitator (2 min)

**Objetivo:** Tener guardada la guía y confirmado que Facilitator está habilitado en la reunión.

**Por qué:** Facilitator tomará las notas durante la reunión; ese tipo de notas es la base de la Práctica 5.

**Paso 1.** Abrir una pestaña nueva, ingresar a [office.com](https://www.office.com/) y seleccionar **Word > Documento en blanco** (o abrir Word de escritorio > **Documento en blanco**). Regresar a Copilot y, debajo de las respuestas de las Tareas 2 y 3, seleccionar el icono **Copiar**. Volver a Word, hacer clic en el documento y pegar con **Ctrl+V**.

- **Qué verás:** el texto con su formato (títulos, tablas y viñetas) dentro del documento.
- **Alternativa:** Si la tabla se pega como texto plano, pegar con **Ctrl+Shift+V** > **Mantener formato de origen**, o pedir a Copilot: *"Entrega la tabla en formato de tabla"* y copiarla de nuevo.

**Paso 2.** Guardar el archivo: en Word de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Guia_Reunion_INT-MDV_[INICIALES].docx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Word para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Guia_Reunion_INT-MDV_[INICIALES].docx` en la barra de título y el estado **Guardado**.

**Paso 3.** Volver a Teams, abrir la reunión `Revisión de preparación INT-MDV-2026` y seleccionar **Opciones de reunión** (en el menú **…** o en la parte superior de los detalles). Localizar la sección **Copilot y agentes** (el nombre puede variar) y confirmar que **Facilitator** esté activado; si no lo está, activarlo y seleccionar **Guardar**.

- **Importante:** no iniciar la reunión. Si la opción no aparece o no se puede modificar, escribir en la guía: *"Facilitator no disponible: [motivo]"* y avisar al instructor.

**Al terminar esta tarea debes tener:**

- ✔ `Guia_Reunion_INT-MDV_[INICIALES].docx` guardada.
- ✔ Facilitator confirmado (o la limitación anotada en la guía).

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué dice Operación sobre la ventana?" | 30 horas aprobadas preliminarmente, con referencia al correo |
| Caso 2 | Pedir los asuntos por resolver | Incluye ventana, permiso ambiental, cliente y vocero |
| Caso 3 | Revisar Opciones de reunión | Facilitator visible y habilitado |
| Caso adversarial | Preguntar: "¿Qué decidió el operador el 20 de noviembre?" | Copilot indica que no hay información de esa fecha y no inventa una decisión |

## Resultado esperado

- Información de la reunión recuperada de invitación, correos y archivos.
- Objetivo, agenda, contexto y preguntas definidos.
- Desacuerdos y decisiones difíciles anticipados.

**Entregable:** guía de preparación de la reunión (`Guia_Reunion_INT-MDV_[INICIALES].docx`).

<img src="../../images/p04-resultado.svg" alt="Resultado final de la Práctica 4" width="640"/>

## Solución de problemas

**Copilot no encuentra los correos**
- *Síntoma:* La respuesta no menciona los correos INT-MDV.
- *Causa:* Los correos no se sembraron o aún no se indexan.
- *Solución:* (1) Buscar los correos en Outlook. (2) Referenciarlos con `/` por su asunto. (3) Avisar al instructor si no existen.

**Facilitator no aparece en Opciones de reunión**
- *Síntoma:* No se muestra la opción.
- *Causa:* Directiva de Teams o el participante no es organizador ni coorganizador.
- *Solución:* (1) Confirmar con el instructor que es coorganizador. (2) Registrar la limitación en la guía. (3) Continuar; la práctica 5 la demuestra el instructor.

## Limpieza

- No iniciar ni cancelar la reunión: se usa como fuente en las prácticas 5 y 7.
- Conservar la guía en `Entregables`.

## Recursos opcionales

- [Facilitator en Microsoft Teams](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams)
- [Copilot en reuniones de Teams](https://support.microsoft.com/es-es/teams/copilot/catch-up-on-meetings-with-microsoft-365-copilot-in-teams)
- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Fácil · Nivel de Bloom: Aplicar</sub>

---

[⬅ Anterior: Práctica 3](../../Capitulo01/Practica03/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 5 ➡](../../Capitulo02/Practica05/README.md)
