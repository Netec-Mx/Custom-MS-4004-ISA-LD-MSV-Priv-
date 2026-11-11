# Práctica 3. Cuestionar una posible decisión

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Utilizar el Entrenador de ideas para analizar críticamente una propuesta antes de presentarla.
- Identificar supuestos débiles y riesgos de la propuesta.
- Formular las objeciones de diferentes áreas afectadas.
- Refinar la propuesta con riesgos, supuestos y aspectos que requieren validación.

<img src="../../images/p03-objetivo.svg" alt="Mapa visual de la práctica 3" width="720"/>

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Entrenador de ideas |
| Archivos de la práctica | [Propuesta_Coordinacion_Intervencion.docx](recursos/Propuesta_Coordinacion_Intervencion.docx) |
| Áreas afectadas | Operación, Mantenimiento, Gestión Ambiental, Comercial, Comunicaciones |

## Instrucciones

Para la intervención programada INT-MDV-2026 en la Subestación Mirador del Valle (caso del curso), un equipo propone un nuevo esquema de coordinación entre Operación, Mantenimiento, Gestión Ambiental, Comercial y Comunicaciones. Antes de presentarlo, el participante usará el Entrenador de ideas para cuestionar sus supuestos, detectar riesgos, adoptar la perspectiva de cada área afectada y fortalecer la propuesta.

### Tarea 1. Presentar la propuesta al agente (3 min)

**Paso 1.** Abrir **Microsoft Edge**, ingresar a [m365.cloud.microsoft](https://m365.cloud.microsoft/) e iniciar sesión con su cuenta corporativa si se solicita.

- **Alternativa:** Si no aparece el chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** Seleccionar en el panel izquierdo **Agentes**, escribir `Entrenador de ideas` en la búsqueda y abrir el agente (en inglés: **Idea Coach**).

- **Comprobación:** el nombre **Entrenador de ideas** encima del cuadro de mensaje.
- **Si no aparece:** buscarlo en **Todos los agentes**; si no aparece, solicitar apoyo a quien administra el entorno.

**Paso 3.** Pegar el siguiente prompt y, antes de enviarlo, adjuntar la propuesta con el botón **+** > `Laboratorio_Copilot_ISA > Practica03 > Propuesta_Coordinacion_Intervencion.docx`:

```text
Voy a presentar la propuesta adjunta para mejorar la coordinación entre áreas durante una intervención
programada en una subestación. Resume en 4 líneas qué propone y qué beneficios promete. No la evalúes todavía.
```

- **Comprobación:** un resumen de 4 líneas que menciona el grupo de mensajería de 45 personas, la autoridad única de Mantenimiento, la eliminación de la reunión go/no-go, el aviso a clientes solo si se excede la duración y los beneficios prometidos (50 % menos tiempo de confirmaciones y terminar 2 horas antes).

**Paso 4.** Abrir el documento si el agente no puede leer el archivo, seleccionar con el cursor las secciones 1 a 4, copiarlas con **Ctrl+C**, pegarlas en el cuadro de mensaje después del prompt y enviarlo de nuevo.

### Tarea 2. Cuestionar supuestos y detectar riesgos (4 min)

**Paso 1.** Pegar el siguiente prompt:

```text
Cuestiona cada supuesto de la propuesta: por qué podría no cumplirse y qué riesgo genera.
Propón al menos dos perspectivas alternativas para lograr el mismo objetivo.
```

- **Comprobación:** una lista de supuestos; cada uno con la razón por la que podría no cumplirse, el riesgo que genera y, al final, al menos dos perspectivas alternativas.

**Paso 2.** Marcar en la respuesta los cuatro supuestos de la sección 3 de la propuesta: lectura en tiempo real del grupo, ventana del operador sin cambios, clientes sin aviso previo y permiso ambiental aprobado a tiempo. Comprobar además que se cuestionen la eliminación del go/no-go y la autoridad única.

- **Si no aparece:** preguntar por el que falte. Ejemplo: *"¿Qué pasa si el permiso de aceite no llega antes del inicio?"*

### Tarea 3. Adoptar la perspectiva de las áreas afectadas (4 min)

**Paso 1.** Pegar el siguiente prompt:

```text
Adopta sucesivamente la perspectiva de Operación, Mantenimiento, Gestión Ambiental, Comercial y Comunicaciones.
Para cada área formula su principal objeción y qué necesitaría para apoyar la propuesta.
```

- **Comprobación:** cinco bloques, uno por área (Operación, Mantenimiento, Gestión Ambiental, Comercial y Comunicaciones), cada uno con su objeción principal y lo que necesitaría para apoyar la propuesta.

**Paso 2.** Elegir la objeción más difícil de responder (por ejemplo, la de Comercial sobre avisar tarde a los clientes) y escribir: *"¿Cómo respondo a la objeción de [área]? Dame una respuesta y qué cambiaría en la propuesta"*.

- **Comprobación:** una respuesta argumentada y un cambio concreto a la propuesta.

### Tarea 4. Refinar la propuesta (4 min)

**Paso 1.** Pegar el siguiente prompt:

```text
Reescribe la propuesta incorporando lo anterior. Incluye: propuesta refinada, supuestos que se mantienen,
riesgos con medida de mitigación y aspectos que requieren validación antes de presentarla, con el área responsable.
```

- **Comprobación:** la propuesta reescrita con cuatro bloques: propuesta refinada, supuestos que se mantienen, riesgos con mitigación y aspectos por validar con área responsable.

**Paso 2.** Leer la propuesta refinada y decidir un ajuste propio (por ejemplo, conservar la reunión go/no-go en 30 minutos o avisar a clientes con 10 días hábiles). Escribirlo así: *"Ajusta la propuesta: [cambio]"*.

- **Comprobación:** la versión final con su ajuste incorporado.

**Paso 3.** Crear un **Documento en blanco** en Word (escritorio o [office.com](https://www.office.com/)). En Copilot, seleccionar **Copiar** debajo de la versión final de la propuesta y pegar en Word con **Ctrl+V**.

- **Alternativa:** Si una tabla se pega como texto plano, pegar con **Ctrl+Shift+V** o pedir a Copilot: *"Entrega la tabla en formato de tabla"*.

**Paso 4.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Propuesta_Refinada_[INICIALES].docx`: en Word de escritorio, **Archivo > Guardar como**; en Word para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

### Resultado esperado

<img src="../../images/p03-resultado.svg" alt="Resultado esperado de la práctica 3" width="720"/>


- Supuestos cuestionados con su riesgo.
- Objeciones de cinco áreas.
- Propuesta refinada con aspectos por validar.

**Entregable:** versión refinada de la propuesta con riesgos, supuestos y aspectos que requieren validación (`Propuesta_Refinada_[INICIALES].docx`).
