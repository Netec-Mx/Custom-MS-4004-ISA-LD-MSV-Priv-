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

**Paso 1.** En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Analista**.

**Paso 2.** Adjuntar `Indicadores_Proyectos_2026.xlsx` con el botón **+** o escribiendo `/`.

**Paso 3.** Escribir:

```text
Describe la estructura del archivo: hojas, columnas, periodo y número de proyectos.
Usa la hoja Diccionario para explicar cada indicador. No hagas análisis todavía.
```

**Paso 4.** Verificar que el agente reporte **12 proyectos** y **9 meses** (2026-01 a 2026-09). Si no coincide, pedirle que muestre el conteo.

**Al terminar esta tarea debes tener:**

- ✔ Analista reporta 12 proyectos y el periodo 2026-01 a 2026-09.
- ✔ La explicación de los indicadores coincide con la hoja `Diccionario`.

---

## Tarea 2. Analizar tendencias, desviaciones y valores atípicos (6 min)

**Objetivo:** Obtener una tabla con los 5 proyectos más desviados y dos gráficos: brecha de avance y comportamiento anómalo por mes.

**Por qué:** Los indicadores sueltos no muestran prioridades. La tabla y los gráficos permiten ver en segundos qué proyectos requieren atención.

**Paso 1.** Escribir:

```text
Con los datos al cierre de 2026-09, calcula para cada proyecto la brecha de avance (real - planeado),
la relación ejecutado/planeado del presupuesto y los hitos pendientes. Muestra una tabla con los
5 proyectos más desviados y un gráfico de barras de la brecha de avance.
```

**Paso 2.** Escribir:

```text
Identifica valores atípicos en incidencias mensuales y tendencias en los días de ciclo de aprobación.
Muestra un gráfico de líneas por mes para los proyectos con comportamiento anómalo.
```

**Paso 3.** Comprobar los hallazgos esperados: **PRY-07** y **PRY-09** con -13 puntos de avance, **PRY-03** con 27 % más ejecución que lo planeado, un pico de **14 incidencias** en PRY-07 en 2026-06 y días de aprobación de **PRY-10** que crecen de 9 a 33.

**Paso 4.** Guardar cada gráfico: pasar el puntero sobre la imagen y seleccionar el icono de descarga (o clic derecho > **Copiar imagen**). Pegarlos en un **Documento en blanco** de Word que será el entregable.

**Al terminar esta tarea debes tener:**

- ✔ Tabla de los 5 proyectos más desviados.
- ✔ Gráfico de barras de brecha de avance.
- ✔ Gráfico de líneas con el pico de PRY-07 y la tendencia de PRY-10.

---

## Tarea 3. Profundizar distinguiendo hechos, explicaciones y faltantes (4 min)

**Objetivo:** Obtener una tabla de tres columnas (dato observado, posible explicación, información faltante) para los 3 hallazgos principales.

**Por qué:** Un dato muestra qué pasó, no por qué. Confundir ambos lleva a culpar a un equipo o a corregir la causa equivocada.

**Paso 1.** Escribir:

```text
Para los tres hallazgos más relevantes, separa la respuesta en tres columnas:
"Dato observado", "Posible explicación" e "Información faltante para confirmar la causa".
No presentes una explicación como hecho.
```

**Paso 2.** Revisar la columna "Posible explicación": ninguna debe estar redactada como hecho confirmado (por ejemplo, "el retraso se debe a…"). Si alguna lo está, escribir: *"Reclasifica como hipótesis la explicación de [proyecto]"*.

**Al terminar esta tarea debes tener:**

- ✔ La tabla de tres columnas.
- ✔ Ninguna explicación presentada como hecho.

---

## Tarea 4. Incorporar un segundo conjunto de datos (4 min)

**Objetivo:** Saber, para cada conclusión inicial, si el segundo archivo la fortalece, la modifica o la descarta, y tener el reporte guardado.

**Por qué:** Las conclusiones cambian con más contexto: el pico de incidencias de PRY-07 parecía un problema técnico y la sobreejecución de PRY-03 parecía mala gestión.

**Paso 1.** Adjuntar `Datos_Complementarios_2026.xlsx` y escribir:

```text
Cruza este segundo archivo con el análisis anterior por proyecto y mes. Para cada conclusión inicial indica si
se fortalece, se modifica o se descarta, y por qué.
```

**Paso 2.** Verificar que el agente detecte que el pico de PRY-07 coincide con un **cambio de contratista** y que la sobreejecución de PRY-03 se explica por un **cambio de alcance aprobado** sin actualizar la línea base.

**Paso 3.** Pegar en el documento de Word las tablas, los gráficos y la respuesta de esta tarea. Seleccionar **Archivo > Guardar como**, elegir **OneDrive > Laboratorio_Copilot_ISA > Entregables** y guardar con el nombre `Reporte_Analitico_[INICIALES].docx`.

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
