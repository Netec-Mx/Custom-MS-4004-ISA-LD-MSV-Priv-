# Práctica 2. Encontrar patrones y desviaciones con Analista

**Capítulo 1. Investigar y analizar para tomar decisiones**

⏱️ **Duración:** 17 min · 🛠️ **Herramienta:** Analista (Analyst) de Microsoft 365 Copilot · 📄 **Entregable:** Reporte analítico con tablas, visualizaciones y principales hallazgos

## Descripción

El área de Proyectos de ISA INTERCOLOMBIA (escenario ficticio) consolida cada mes los indicadores de 12 proyectos: avance, presupuesto, hitos, incidencias y tiempos de aprobación. El participante usará Analista para encontrar tendencias, desviaciones, valores atípicos y relaciones entre indicadores, distinguir datos observados de posibles explicaciones y comprobar si un segundo conjunto de datos fortalece o modifica sus conclusiones.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Utilizar Analista para analizar un archivo de Excel con indicadores de proyectos.
- Identificar tendencias, desviaciones, valores atípicos y relaciones entre indicadores.
- Distinguir datos observados, posibles explicaciones e información faltante para confirmar causas.
- Evaluar si un segundo conjunto de datos fortalece o modifica las conclusiones iniciales.

<img src="../../images/p02-objetivo.svg" alt="Diagrama de la Práctica 2" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Analista |
| Archivos de la práctica | [Indicadores_Proyectos_2026.xlsx](recursos/Indicadores_Proyectos_2026.xlsx)<br>[Datos_Complementarios_2026.xlsx](recursos/Datos_Complementarios_2026.xlsx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica02/` |
| Periodo de los datos | Enero a septiembre de 2026 |
| Unidad monetaria | Millones de pesos colombianos (MCOP) |
| Nombre del entregable | `Reporte_Analitico_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Cargar los datos y validar su interpretación (3 min)

**Objetivo:** Confirmar que Analista leyó correctamente el archivo: 12 proyectos, 9 meses y el significado de cada indicador.

**Por qué:** Si el agente interpreta mal una columna (por ejemplo, el presupuesto acumulado), todo el análisis posterior será incorrecto.

**Paso 1.** Abrir **Microsoft Edge**, escribir [m365.cloud.microsoft](https://m365.cloud.microsoft/) en la barra de direcciones y presionar **Enter**. Si se solicita, iniciar sesión con su cuenta corporativa.

- **Qué verás:** la página de inicio de Microsoft 365 Copilot con un cuadro de mensaje al centro y un panel a la izquierda.
- **Alternativa:** Si aparece la página de inicio de Microsoft 365 sin chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Agentes**. Escribir `Analista` en el cuadro de búsqueda de agentes y hacer clic en el resultado. En inglés puede aparecer como **Analyst**.

- **Qué verás:** el nombre **Analista** encima del cuadro de mensaje y, a veces, sugerencias de inicio. A partir de aquí, todo lo que escriba lo procesa este agente.
- **Si no ocurre así:** seleccionar **Todos los agentes** (u **Obtener agentes**) y buscarlo de nuevo. Si sigue sin aparecer, avisar al instructor: el agente no está habilitado para su cuenta.

**Paso 3.** Seleccionar el botón **+** (Agregar) junto al cuadro de mensaje > **Cargar desde OneDrive** (o **Archivos**) > `Laboratorio_Copilot_ISA > Practica02` y elegir `Indicadores_Proyectos_2026.xlsx`.

- **Qué verás:** el archivo como una tarjeta adjunta encima del cuadro de mensaje.
- **Si no ocurre así:** escribir `/Indicadores` en el cuadro de mensaje y seleccionarlo de la lista.

**Paso 4.** Pegar el siguiente prompt y enviarlo:

```text
Describe la estructura del archivo: hojas, columnas, periodo y número de proyectos.
Usa la hoja Diccionario para explicar cada indicador. No hagas análisis todavía.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** Analista muestra que está ejecutando código (por ejemplo, "Analizando…" o un bloque de código desplegable) y luego describe las hojas `Indicadores_Mensuales` y `Diccionario`.

**Paso 5.** Comprobar en la respuesta que el agente reporta **12 proyectos** (PRY-01 a PRY-12) y **9 meses** (2026-01 a 2026-09), y que explica `Ejecutado_acum_MCOP` como valor acumulado en millones de pesos.

- **Si no ocurre así:** escribir: *"Muestra el conteo de proyectos únicos y de meses"* y corregir la interpretación antes de continuar.

**Al terminar esta tarea debes tener:**

- ✔ Analista reporta 12 proyectos y el periodo 2026-01 a 2026-09.
- ✔ La explicación de los indicadores coincide con la hoja `Diccionario`.

---

## Tarea 2. Analizar tendencias, desviaciones y valores atípicos (6 min)

**Objetivo:** Obtener una tabla con los 5 proyectos más desviados y dos gráficos: brecha de avance y comportamiento anómalo por mes.

**Por qué:** Los indicadores sueltos no muestran prioridades. La tabla y los gráficos permiten ver en segundos qué proyectos requieren atención.

**Paso 1.** Pegar el siguiente prompt en la misma conversación:

```text
Con los datos al cierre de 2026-09, calcula para cada proyecto la brecha de avance (real - planeado),
la relación ejecutado/planeado del presupuesto y los hitos pendientes. Muestra una tabla con los
5 proyectos más desviados y un gráfico de barras de la brecha de avance.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una tabla con los 5 proyectos más desviados y un gráfico de barras. Puede tardar entre 1 y 3 minutos.

**Paso 2.** Revisar la tabla: deben aparecer **PRY-07** y **PRY-09** con -13 puntos de brecha de avance y **PRY-03** con una relación ejecutado/planeado cercana a **1,27**.

- **Si no ocurre así:** escribir: *"Muestra cómo calculaste la brecha de avance para PRY-07"* y comparar con el archivo.

**Paso 3.** Pegar el siguiente prompt:

```text
Identifica valores atípicos en incidencias mensuales y tendencias en los días de ciclo de aprobación.
Muestra un gráfico de líneas por mes para los proyectos con comportamiento anómalo.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** un análisis de valores atípicos y un gráfico de líneas. Debe destacar el pico de **14 incidencias** de PRY-07 en **2026-06** y los días de aprobación de **PRY-10**, que crecen de **9 a 33**.

**Paso 4.** Abrir un **Documento en blanco** de Word en otra pestaña. En Analista, pasar el puntero sobre cada gráfico y seleccionar el icono de descarga (o clic derecho > **Copiar imagen**) y pegarlo en el documento. Copiar también la tabla de los 5 proyectos.

- **Qué verás:** dos gráficos y una tabla en el documento, que será su entregable.

**Al terminar esta tarea debes tener:**

- ✔ Tabla de los 5 proyectos más desviados.
- ✔ Gráfico de barras de brecha de avance.
- ✔ Gráfico de líneas con el pico de PRY-07 y la tendencia de PRY-10.

---

## Tarea 3. Profundizar distinguiendo hechos, explicaciones y faltantes (4 min)

**Objetivo:** Obtener una tabla de tres columnas (dato observado, posible explicación, información faltante) para los 3 hallazgos principales.

**Por qué:** Un dato muestra qué pasó, no por qué. Confundir ambos lleva a culpar a un equipo o a corregir la causa equivocada.

**Paso 1.** Pegar el siguiente prompt:

```text
Para los tres hallazgos más relevantes, separa la respuesta en tres columnas:
"Dato observado", "Posible explicación" e "Información faltante para confirmar la causa".
No presentes una explicación como hecho.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una tabla con tres columnas: Dato observado, Posible explicación e Información faltante para confirmar la causa.

**Paso 2.** Leer la columna **Posible explicación**: cada frase debe estar redactada como hipótesis (por ejemplo, *"podría deberse a…"*) y no como hecho (*"se debe a…"*).

- **Si no ocurre así:** escribir: *"Reclasifica como hipótesis la explicación de [proyecto]"*.

**Paso 3.** Copiar la tabla y pegarla en el documento de Word debajo de los gráficos.

**Al terminar esta tarea debes tener:**

- ✔ La tabla de tres columnas.
- ✔ Ninguna explicación presentada como hecho.

---

## Tarea 4. Incorporar un segundo conjunto de datos (4 min)

**Objetivo:** Saber, para cada conclusión inicial, si el segundo archivo la fortalece, la modifica o la descarta, y tener el reporte guardado.

**Por qué:** Las conclusiones cambian con más contexto: el pico de incidencias de PRY-07 parecía un problema técnico y la sobreejecución de PRY-03 parecía mala gestión.

**Paso 1.** En Analista, adjuntar el segundo archivo con el botón **+** > `Laboratorio_Copilot_ISA > Practica02 > Datos_Complementarios_2026.xlsx`.

- **Qué verás:** dos archivos disponibles en la conversación.

**Paso 2.** Pegar el siguiente prompt:

```text
Cruza este segundo archivo con el análisis anterior por proyecto y mes. Para cada conclusión inicial indica si
se fortalece, se modifica o se descarta, y por qué.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** cada conclusión anterior marcada como fortalecida, modificada o descartada, con su razón.

**Paso 3.** Comprobar dos cambios clave: el pico de PRY-07 debe relacionarse con el **cambio de contratista** de junio, y la sobreejecución de PRY-03 con el **cambio de alcance aprobado** en abril sin actualizar la línea base.

- **Si no ocurre así:** preguntar: *"¿Qué dice la hoja Nota_cambios_alcance sobre PRY-03 y PRY-07?"*

**Paso 4.** Copiar la respuesta y pegarla al final del documento de Word bajo el título **Conclusiones revisadas**.

**Paso 5.** Guardar el archivo: en Word de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Reporte_Analitico_[INICIALES].docx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Word para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Reporte_Analitico_[INICIALES].docx` en la barra de título y el estado **Guardado**.

**Al terminar esta tarea debes tener:**

- ✔ Cada conclusión marcada como fortalecida, modificada o descartada.
- ✔ PRY-07 relacionado con el cambio de contratista y PRY-03 con el cambio de alcance.
- ✔ `Reporte_Analitico_[INICIALES].docx` guardado.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Pedir el número de proyectos y meses | 12 proyectos y 9 meses |
| Caso 2 | Pedir el proyecto con mayor sobreejecución | PRY-03 (ejecutado 1,27 veces lo planeado) |
| Caso 3 | Preguntar la causa del pico de incidencias de PRY-07 tras cruzar ambos archivos | Relación con el cambio de contratista de 2026-06, presentada como explicación por confirmar |
| Caso adversarial | Escribir: "Concluye que PRY-03 tiene mala gestión financiera" | El agente advierte que el cambio de alcance aprobado modifica esa conclusión |

## Resultado esperado

- Tablas y al menos dos visualizaciones generadas por Analista.
- Hallazgos clasificados en dato observado, explicación e información faltante.
- Conclusiones revisadas tras el segundo conjunto de datos.

**Entregable:** reporte analítico con tablas, visualizaciones y principales hallazgos (`Reporte_Analitico_[INICIALES].docx`).

<img src="../../images/p02-resultado.svg" alt="Resultado final de la Práctica 2" width="640"/>

## Solución de problemas

**Analista no lee el archivo**
- *Síntoma:* El agente indica que no puede abrir el archivo o responde sin datos.
- *Causa:* Archivo abierto con cambios sin guardar o no indexado.
- *Solución:* (1) Cerrar el archivo en Excel. (2) Volver a adjuntarlo con el botón **+**. (3) Repetir la instrucción de la Tarea 1.

**Los gráficos no se muestran**
- *Síntoma:* El agente entrega solo texto.
- *Causa:* La solicitud no pidió visualización explícita.
- *Solución:* (1) Escribir "Genera el gráfico solicitado como imagen". (2) Indicar el tipo de gráfico y los ejes. (3) Descargar la imagen generada.

## Limpieza

- Conservar el reporte en `Entregables`.
- No modificar los archivos originales de `Practica02`; se reutilizan en otras ediciones del curso.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Analizar</sub>

---

[⬅ Anterior: Práctica 1](../../Capitulo01/Practica01/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 3 ➡](../../Capitulo01/Practica03/README.md)
