# Práctica 1. Investigación profunda para una decisión

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Seleccionar Investigador en lugar del chat de Copilot cuando una necesidad requiere investigación compleja con múltiples fuentes.
- Analizar una tecnología con aplicación en transmisión de energía considerando evolución, casos de aplicación, beneficios, riesgos, madurez y fuentes.
- Contrastar tendencias externas con prioridades internas del caso de ISA INTERCOLOMBIA.
- Identificar contradicciones entre fuentes y aspectos sin evidencia suficiente.

<img src="../../images/p01-objetivo.svg" alt="Mapa visual de la práctica 1" width="720"/>

## Duración aproximada:

- 20 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Investigador |
| Archivos de la práctica | [Prioridades_Internas_2027.docx](recursos/Prioridades_Internas_2027.docx) |
| Tecnología a investigar | Gemelos digitales para gestión de activos de transmisión |

## Instrucciones

La Gerencia de Gestión de Activos de ISA INTERCOLOMBIA (caso del curso) evalúa si los **gemelos digitales** pueden apoyar las decisiones de mantenimiento y operación de la red de transmisión. Una consulta genérica a Copilot no basta: la decisión exige revisar múltiples fuentes, evaluar madurez, beneficios y riesgos, y contrastar la evidencia externa con las prioridades internas. El participante usará Investigador para construir un reporte de investigación con fuentes verificables, contradicciones y preguntas pendientes.

### Tarea 1. Lanzar la investigación externa (5 min)

**Paso 1.** Abrir **Microsoft Edge**, ingresar a [m365.cloud.microsoft](https://m365.cloud.microsoft/) e iniciar sesión con su cuenta corporativa si se solicita.

- **Alternativa:** Si no aparece el chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** Seleccionar en el panel izquierdo **Agentes**, escribir `Investigador` en la búsqueda y abrir el agente (en inglés: **Researcher**).

- **Comprobación:** el nombre **Investigador** encima del cuadro de mensaje.
- **Si no aparece:** buscarlo en **Todos los agentes**; si no aparece, solicitar apoyo a quien administra el entorno.

**Paso 3.** Hacer clic en el cuadro de mensaje del agente y pegar el siguiente prompt:

```text
Investiga el uso de gemelos digitales para la gestión de activos en empresas de transmisión de energía eléctrica.
Incluye: evolución de la tecnología desde 2020, casos de aplicación documentados en empresas de transmisión,
beneficios reportados, riesgos de implementación, nivel de madurez y fuentes utilizadas.
Distingue entre resultados medidos y expectativas de proveedores. Cita cada afirmación.
```

- **Comprobación:** Investigador puede responder primero con preguntas de aclaración (por ejemplo, sobre el alcance geográfico o el uso del resultado) antes de empezar a investigar.

**Paso 4.** Responder las preguntas de aclaración en el cuadro de mensaje. Usar estas respuestas: para el alcance geográfico, *"Latinoamérica, Europa y Norteamérica"*; para el uso del resultado, *"Decidir si proponer un piloto en 2027"*; para cualquier otra pregunta, *"Prioriza empresas de transmisión de energía"*.

- **Comprobación:** un indicador de progreso con las búsquedas y fuentes que el agente va consultando. La investigación tarda entre 3 y 10 minutos.
- **Importante:** no cerrar ni recargar la pestaña mientras el agente trabaja.

**Paso 5.** Abrir una pestaña nueva mientras Investigador trabaja, seleccionar el icono de **OneDrive** en Microsoft 365, entrar a `Laboratorio_Copilot_ISA > Practica01` y abrir `Prioridades_Internas_2027.docx`.

**Paso 6.** Leer las secciones **2. Prioridades** y **3. Restricciones** y anotar en una nota rápida las 4 metas (por ejemplo, "-15 % desconexiones") y las 4 restricciones (2.500 MCOP, 40 % de datos no integrados, 3 personas con experiencia en analítica, evaluación de ciberseguridad OT).

- **Importante:** estas cifras se usarán en la Tarea 2 para comprobar que el agente las tomó en cuenta.

### Tarea 2. Contrastar tendencias externas con prioridades internas (6 min)

**Paso 1.** Regresar a la pestaña de Investigador. Esperar a que el indicador de progreso desaparezca y se muestre el informe completo.

- **Comprobación:** un informe con un resumen inicial y secciones sobre evolución, casos de aplicación, beneficios, riesgos y madurez, con números de cita entre corchetes.
- **Alternativa:** Si el informe no aparece después de 10 minutos, actualizar la página y abrir la conversación desde el historial del panel izquierdo; la investigación continúa en segundo plano.

**Paso 2.** Localizar en el informe dos números de cita entre corchetes (por ejemplo, [1] y [4]) de secciones diferentes y hacer clic en cada uno. La fuente se abre en una pestaña nueva o en un panel lateral.

- **Comprobación:** la página de origen. Buscar en ella (**Ctrl+F**) una palabra clave de la afirmación citada.
- **Alternativa:** Si la página no menciona el dato, anotar *"Cita [n] no respalda: …"* para la sección Fuentes del entregable.

**Paso 3.** Regresar al chat de Investigador y pegar el siguiente prompt en la misma conversación:

```text
Contrasta tus hallazgos con /Prioridades_Internas_2027. Para cada una de las cuatro prioridades indica
si los gemelos digitales contribuyen (alto, medio, bajo) y con qué evidencia. Evalúa también si las
restricciones (presupuesto de 2.500 MCOP, datos no integrados, 3 personas con experiencia en analítica,
evaluación de ciberseguridad OT) hacen viable un piloto. Marca como "inferencia" lo que no esté respaldado por una fuente.
```

- **Cómo insertar los archivos:** cada texto que empieza con `/` es un archivo: borrarlo, escribir `/` y las primeras letras del nombre, y elegir el archivo en la lista. Si no aparece, usar **+** > **Cargar desde OneDrive** > `Laboratorio_Copilot_ISA/Practica01`.
- **Comprobación:** una tabla o lista con las 4 prioridades del documento, un nivel de contribución (alto, medio o bajo) por prioridad, la evidencia y comentarios sobre las restricciones.

**Paso 4.** Comparar la respuesta con su nota de la Tarea 1: debe haber **4 filas** (una por prioridad) y las restricciones deben mencionar los **datos no integrados**.

- **Si no aparece:** escribir: *"¿Cómo afecta al piloto que el 40 % de los datos esté en hojas de cálculo?"* y revisar la nueva respuesta.

### Tarea 3. Identificar contradicciones y evidencia insuficiente (5 min)

**Paso 1.** Pegar en la misma conversación el siguiente prompt:

```text
Identifica contradicciones entre las fuentes que consultaste (por ejemplo, beneficios o costos reportados
de forma distinta) y muestra quién afirma qué. Luego lista los aspectos para los que todavía no existe
evidencia suficiente para decidir un piloto en ISA INTERCOLOMBIA.
```

- **Comprobación:** una lista de contradicciones con el nombre de cada fuente y lo que afirma, seguida de una lista de aspectos sin evidencia suficiente.
- **Alternativa:** Si el agente responde que no hay contradicciones, escribir: *"Compara específicamente los beneficios y costos reportados por cada fuente"*.

**Paso 2.** Revisar si cada fuente aparece identificada como **caso documentado** de una empresa de transmisión o como **material de un proveedor**.

- **Si no aparece:** escribir: *"Clasifica cada fuente como caso documentado o material de proveedor"*.

**Paso 3.** Anotar al menos tres preguntas que el equipo debe responder antes de proponer un piloto. Pueden tomarse de la respuesta del agente o redactarse a partir de ella. Ejemplos: *¿qué calidad de datos se necesita?*, *¿cuánto costaría un piloto en una subestación?*, *¿qué evaluación de ciberseguridad OT aplica?*

### Tarea 4. Consolidar el reporte de investigación (4 min)

**Paso 1.** Crear un **Documento en blanco** en Word (escritorio o [office.com](https://www.office.com/)). En Copilot, seleccionar **Copiar** debajo del informe de Investigador y pegar en Word con **Ctrl+V**.

- **Alternativa:** Si una tabla se pega como texto plano, pegar con **Ctrl+Shift+V** o pedir a Copilot: *"Entrega la tabla en formato de tabla"*.

**Paso 2.** Repetir la acción **Copiar > Ctrl+V** con la respuesta de la Tarea 2 (tabla de prioridades) y la de la Tarea 3 (contradicciones). Al final del documento, escribir las tres preguntas pendientes que anotó.

**Paso 3.** Escribir estos títulos con el estilo **Título 1** (**Inicio > Estilos**): **Fuentes**, **Hallazgos**, **Oportunidades**, **Riesgos**, **Contradicciones entre fuentes** y **Preguntas pendientes**. Mover cada contenido debajo del título que le corresponde (**Ctrl+X** y **Ctrl+V**).

**Paso 4.** Conservar en la sección **Fuentes** la lista de citas del informe y agregar las notas de verificación de la Tarea 2 (por ejemplo, *"Cita [4] verificada"*).

**Paso 5.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Reporte_Investigacion_[INICIALES].docx`: en Word de escritorio, **Archivo > Guardar como**; en Word para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

### Resultado esperado

<img src="../../images/p01-resultado.svg" alt="Resultado esperado de la práctica 1" width="720"/>


- Informe de Investigador con citas verificadas.
- Contraste explícito con las prioridades internas del caso.
- Lista de contradicciones entre fuentes y de evidencia insuficiente.

**Entregable:** reporte de investigación con fuentes, hallazgos, oportunidades, riesgos y preguntas pendientes (`Reporte_Investigacion_[INICIALES].docx`).
