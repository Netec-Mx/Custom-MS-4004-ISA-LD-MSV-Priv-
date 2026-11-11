# Práctica 4. Antes de la reunión: prepararse con Facilitator y Copilot

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Recuperar con Copilot la información de una reunión distribuida entre invitación, correos y archivos en la nube.
- Preparar objetivo, agenda, contexto necesario, preguntas relevantes y asuntos por resolver.
- Identificar posibles desacuerdos y decisiones difíciles y preparar preguntas para conducirlos.
- Confirmar que Facilitator esté disponible para la reunión.

<img src="../../images/p04-objetivo.svg" alt="Mapa visual de la práctica 4" width="720"/>

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Dónde trabajar | Microsoft Teams > Calendario |
| Plan y riesgos | [Plan_Intervencion_Mirador_del_Valle.docx](recursos/Plan_Intervencion_Mirador_del_Valle.docx) y [Matriz_Riesgos_Intervencion.xlsx](recursos/Matriz_Riesgos_Intervencion.xlsx) |
| Evento importable | [Reunion_Preparacion_INT-MDV.ics](recursos/Reunion_Preparacion_INT-MDV.ics) |
| Correos importables | [Operación](recursos/INT-MDV_Operacion.eml) · [Ambiental](recursos/INT-MDV_Ambiental.eml) · [Comercial](recursos/INT-MDV_Comercial.eml) |
| Reunión | `Revisión de preparación INT-MDV-2026` |
| Correos | Asuntos que inician con `INT-MDV` |
| Fecha de referencia | 10 de noviembre de 2026 |

## Instrucciones

El participante tiene programada la reunión **"Revisión de preparación INT-MDV-2026"** para la intervención en la Subestación Mirador del Valle (caso del curso). La información está distribuida en una convocatoria de Outlook, tres correos de Operación, Gestión Ambiental y Comercial y dos archivos de OneDrive. Todos estos recursos se preparan siguiendo la Setup Guide. Usará Copilot y las capacidades de Teams y Facilitator para preparar el objetivo, la agenda, el contexto, las preguntas y las decisiones difíciles de la reunión.

### Tarea 1. Revisar la reunión y reunir la información disponible (4 min)

**Paso 1.** Abrir **Microsoft Teams** (aplicación de escritorio o [teams.microsoft.com](https://teams.microsoft.com/)) y seleccionar **Calendario** en la barra izquierda.

**Paso 2.** Buscar en el calendario la reunión `Revisión de preparación INT-MDV-2026` y hacer doble clic para abrir sus detalles.

- **Comprobación:** la convocatoria importada identifica el proyecto y el horario; el organizador completó el vínculo de Teams y compartió el plan desde OneDrive.
- **Si no aparece:** comprobar que se importó el archivo `.ics` en el calendario correcto y se habilitó la reunión en línea en la preparación.

**Paso 3.** Seleccionar **Preparar para esta reunión** / **Prepare for this meeting** desde los detalles del evento, si aparece; alternativamente abrir **Copilot Chat** y referenciar la reunión desde el selector de contexto. La preparación depende de que existan contenidos relacionados y permisos de lectura.

- **Comprobación:** un resumen generado por Copilot con el contexto de la reunión y archivos o correos relacionados.
- **Alternativa:** Si la opción no existe, cerrar los detalles, seleccionar **Copilot** en la barra izquierda de Teams y continuar con el paso siguiente.

**Paso 4.** Pegar en Copilot Chat el siguiente prompt (borrar el texto que inicia con `/` y seleccionar la reunión y cada archivo de la lista que aparece al escribir `/`):

```text
¿Qué información existe sobre /Revisión de preparación INT-MDV-2026? Revisa la invitación, mis correos con asunto INT-MDV
y los archivos /Plan_Intervencion_Mirador_del_Valle y /Matriz_Riesgos_Intervencion. Indica la fuente de cada dato.
```

- **Comprobación:** una lista de fuentes con lo que aporta cada una. Si los `.eml` aún no están indexados, abrirlos en Outlook y utilizar su contenido como contexto explícito sin atribuirlos a otras reuniones. Si los `.eml` aún no están indexados, abrirlos en Outlook y utilizar su contenido como contexto explícito sin atribuirlos a otras reuniones.

**Paso 5.** Comprobar que aparezcan las cinco fuentes de contenido: correo de **Operación** (ventana de 30 horas), correo de **Gestión Ambiental** (permiso en trámite), correo de **Comercial** (cliente sin acuse), el **plan** y la **matriz de riesgos**.

- **Si no aparece:** verificar que el mensaje `.eml` fue importado al buzón en el nuevo Outlook. Abrirlo y copiar su contenido al chat cuando el agente no lo encuentre; distinguir la información aportada manualmente de la encontrada por Copilot.

### Tarea 2. Preparar objetivo, agenda, contexto y preguntas (6 min)

**Paso 1.** Pegar el siguiente prompt en la misma conversación:

```text
Prepara para esta reunión: 1) objetivo en una frase, 2) agenda de 45 minutos con tiempos,
3) contexto que todos deben conocer, 4) preguntas relevantes por área y 5) asuntos que deben resolverse durante la reunión.
```

- **Comprobación:** cinco secciones: objetivo, agenda con tiempos que suman 45 minutos, contexto, preguntas por área y asuntos por resolver.

**Paso 2.** Revisar el **contexto**: debe distinguir la ventana planeada de **36 h** frente a las **30 h** planteadas preliminarmente, el permiso ambiental con respuesta estimada el **25-nov** y el cliente que pidió reprogramar.

- **Si no aparece:** escribir: *"Agrega al contexto lo que dicen los correos de Operación, Gestión Ambiental y Comercial"*.

**Paso 3.** Revisar la **agenda**: los tres asuntos críticos (ventana, permiso y cliente) deben tener tiempo asignado.

- **Si no aparece:** escribir: *"Ajusta la agenda para dar 10 minutos a [asunto]"*.

### Tarea 3. Anticipar desacuerdos y decisiones difíciles (3 min)

**Paso 1.** Pegar el siguiente prompt:

```text
¿Qué desacuerdos o decisiones difíciles podrían surgir en esta reunión? Para cada uno indica las posiciones probables
de las áreas y propón dos preguntas para conducir la conversación hacia una decisión.
```

- **Comprobación:** una lista de desacuerdos o decisiones difíciles, con la posición probable de cada área y dos preguntas por cada uno.

**Paso 2.** Confirmar que aparezcan al menos tres: **mantener o reprogramar la fecha** ante la solicitud del cliente, **re-secuenciar actividades** para 30 horas y **designar al vocero** ante medios.

- **Si no aparece:** preguntar directamente: *"¿Qué desacuerdo podría haber sobre [tema] y cómo lo conduzco?"*

### Tarea 4. Guardar la guía y confirmar Facilitator (2 min)

**Paso 1.** Crear un **Documento en blanco** en Word (escritorio o [office.com](https://www.office.com/)). En Copilot, seleccionar **Copiar** debajo de las respuestas de las Tareas 2 y 3 y pegar en Word con **Ctrl+V**.

- **Alternativa:** Si una tabla se pega como texto plano, pegar con **Ctrl+Shift+V** o pedir a Copilot: *"Entrega la tabla en formato de tabla"*.

**Paso 2.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Guia_Reunion_INT-MDV_[INICIALES].docx`: en Word de escritorio, **Archivo > Guardar como**; en Word para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

**Paso 3.** Abrir en Teams la reunión `Revisión de preparación INT-MDV-2026` y seleccionar **Opciones de reunión** (en el menú **…** o en la parte superior de los detalles). Localizar **Opciones > Copilot y otra IA**, comprobar si **Facilitator** está habilitado y, solo si se tienen permisos de organizador, activarlo y guardar. **No iniciar la reunión**: Facilitator tomará notas cuando la reunión programada se realice, no durante esta preparación.

- **Importante:** no iniciar la reunión. Si no puede habilitarse Facilitator, registrar el impedimento como condición del entorno y solicitar apoyo a quien administra la reunión.

### Resultado esperado

<img src="../../images/p04-resultado.svg" alt="Resultado esperado de la práctica 4" width="720"/>


- Información de la reunión recuperada de invitación, correos y archivos.
- Objetivo, agenda, contexto y preguntas definidos.
- Desacuerdos y decisiones difíciles anticipados.

**Entregable:** guía de preparación de la reunión (`Guia_Reunion_INT-MDV_[INICIALES].docx`).
