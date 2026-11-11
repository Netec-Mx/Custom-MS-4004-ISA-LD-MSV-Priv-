# Práctica 14. Del entorno a la decisión

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Obtener evidencia externa con Investigador e integrarla en Word distinguiéndola de la información del caso.
- Analizar los datos del caso con Analista y preparar evidencia con Copilot en Excel.
- Construir con Copilot en PowerPoint una presentación ejecutiva con contexto, evidencia, oportunidades, riesgos, propuesta y próximos pasos.
- Revisar la presentación para eliminar exceso de información y afirmaciones no respaldadas.

<img src="../../images/p14-objetivo.svg" alt="Mapa visual de la práctica 14" width="720"/>

## Duración aproximada:

- 30 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot, Word, Excel y PowerPoint |
| Archivos de la práctica | [Caso_Monitoreo_Predictivo_Activos.docx](recursos/Caso_Monitoreo_Predictivo_Activos.docx)<br>[Datos_Activos_MPA.xlsx](recursos/Datos_Activos_MPA.xlsx) |
| Activos con monitoreo | TR-01 a TR-08 (desde 2025-T1) |
| Inversión a evaluar | 3.600 MCOP para 12 transformadores (2027) |

## Instrucciones

La iniciativa del caso de **modernización y monitoreo predictivo de activos (MPA)** debe decidir si amplía el monitoreo en línea a 12 transformadores más. El participante partirá de un documento Word y un Excel del caso, usará Investigador para la evidencia externa, Analista y Copilot en Excel para los datos, Copilot en Word para integrar la investigación y Copilot en PowerPoint para construir y revisar una presentación ejecutiva.

### Tarea 1. Lanzar la investigación externa (3 min)

**Paso 1.** Abrir en OneDrive `Laboratorio_Copilot_ISA > Practica14`. Seleccionar `Caso_Monitoreo_Predictivo_Activos.docx`, elegir **Copiar a > Entregables** y renombrar la copia como `Caso_MPA_[INICIALES].docx`. Repetir con `Datos_Activos_MPA.xlsx` y el nombre `Datos_MPA_[INICIALES].xlsx`.

- **Comprobación:** las dos copias en `Entregables`. En el resto de la práctica se trabaja solo con estas copias.

**Paso 2.** Abrir **Microsoft Edge**, ingresar a [m365.cloud.microsoft](https://m365.cloud.microsoft/) e iniciar sesión con su cuenta corporativa si se solicita.

- **Alternativa:** Si no aparece el chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

Después, abrir el agente **Investigador** (panel izquierdo **Agentes** > buscar `Investigador`).

**Paso 3.** Pegar el siguiente prompt (insertar `/Caso_MPA_[INICIALES]` con el selector de archivos) y enviarlo:

```text
Con base en las preguntas de la sección 5 de /Caso_MPA_[INICIALES], investiga resultados de empresas de transmisión que
adoptaron monitoreo predictivo de transformadores, tecnologías más maduras, oportunidades y riesgos documentados
(ciberseguridad, calidad de datos, capacidades). Cita cada fuente.
```

- **Cómo insertar los archivos:** cada texto que empieza con `/` es un archivo: borrarlo, escribir `/` y las primeras letras del nombre, y elegir el archivo en la lista. Si no aparece, usar **+** > **Cargar desde OneDrive** > `Laboratorio_Copilot_ISA/Practica14`.
- **Comprobación:** posibles preguntas de aclaración y luego el indicador de progreso de la investigación.

**Paso 4.** Responder las preguntas de aclaración (por ejemplo: *"Empresas de transmisión de energía; enfoque en transformadores de potencia"*) y **dejar la pestaña abierta**: continuar con la Tarea 2 mientras Investigador trabaja.

### Tarea 2. Analizar los datos con Analista (7 min)

**Paso 1.** Abrir una pestaña nueva con [m365.cloud.microsoft](https://m365.cloud.microsoft/), seleccionar **Agentes** y abrir **Analista**. Adjuntar `Datos_MPA_[INICIALES].xlsx` con el botón **+** desde `Entregables`.

**Paso 2.** Pegar el siguiente prompt y enviarlo:

```text
Compara los activos con monitoreo en línea (TR-01 a TR-08) y sin monitoreo, antes (2024) y después (2025-2026),
en intervenciones correctivas, horas de indisponibilidad y costo de mantenimiento. Identifica tendencias, valores atípicos
y relaciones. Muestra una tabla y un gráfico.
```

- **Comprobación:** una tabla comparativa y un gráfico. Puede tardar entre 1 y 3 minutos.

**Paso 3.** Verificar los hallazgos: en los activos **con monitoreo** las intervenciones correctivas bajan de **2,16 a 0,96** por trimestre y las horas de indisponibilidad de **28,8 a 17,1**; en los activos **sin monitoreo** no mejoran; **TR-14** (sin monitoreo) es atípico por costos altos en 2026.

- **Si no aparece:** escribir: *"Muestra los promedios por grupo y periodo que usaste"*.

**Paso 4.** Escribir: *"¿Qué información faltaría para atribuir la mejora al monitoreo y no a otros factores?"* y copiar la respuesta en una nota.

### Tarea 3. Preparar la evidencia en Excel (5 min)

**Paso 1.** Abrir `Datos_MPA_[INICIALES].xlsx` desde `Entregables` en Excel (escritorio o web) y seleccionar **Copilot** en la pestaña **Inicio**.

**Paso 2.** Escribir en el panel de Copilot: *"Agrega una columna Grupo con Con monitoreo para TR-01 a TR-08 y Sin monitoreo para el resto, y una columna Periodo con 2024 o 2025-2026 según el trimestre"*. Revisar la vista previa y seleccionar **Insertar**.

- **Comprobación:** dos columnas nuevas en la hoja `Desempeno_Trimestral`.

**Paso 3.** Escribir: *"Crea una tabla dinámica con el promedio de intervenciones correctivas y horas de indisponibilidad por Grupo y Periodo"* y seleccionar **Agregar a una hoja nueva**.

**Paso 4.** Seleccionar la tabla dinámica y escribir: *"Crea un gráfico de columnas a partir de esta tabla"*. Guardar con **Ctrl+S**.

- **Comprobación:** un gráfico con cuatro barras por indicador (con o sin monitoreo, antes o después).
- **Alternativa:** Si Copilot no crea el gráfico, seleccionar la tabla dinámica > **Insertar > Gráfico de columnas**.

### Tarea 4. Integrar la investigación en Word (6 min)

**Paso 1.** Volver a la pestaña de Investigador. Cuando termine, leer el informe y abrir al menos una fuente citada para verificarla. Copiar el resumen del informe (botón **Copiar**).

- **Alternativa:** Si aún no termina, avanzar a la Tarea 5 y volver después.

**Paso 2.** Abrir `Caso_MPA_[INICIALES].docx` desde `Entregables`, ubicar la sección **6. Hallazgos de la investigación externa**, pegar allí el resumen obtenido de Investigador con sus citas y seleccionar solamente el texto pegado. Abrir **Copilot** en la pestaña **Inicio** de Word.

**Paso 3.** Pegar en el panel de Copilot el siguiente prompt para trabajar sobre el texto seleccionado:

```text
Reestructura y resume el texto seleccionado de la sección 6 para contrastar la investigación con los objetivos y
la situación del caso. Distingue cada afirmación como [Evidencia externa] o [Información del caso], conserva
las referencias a las fuentes originales y marca los datos sin confirmación. No inventes fuentes ni resultados.
```

- **Comprobación:** una propuesta de texto con etiquetas [Evidencia externa] e [Información del caso]. Seleccionar **Conservar** o **Insertar** si la propuesta está sustentada; de lo contrario, editar directamente el texto pegado.

**Paso 4.** Escribir debajo de la sección 6 el título **7. Hallazgos de los datos** y pegar los resultados de Analista (Tarea 2). Guardar con **Ctrl+S**.

### Tarea 5. Construir la presentación ejecutiva (6 min)

**Paso 1.** Abrir PowerPoint (escritorio o [office.com](https://www.office.com/) > **PowerPoint**), crear una **Presentación en blanco** y seleccionar **Copilot** en la pestaña **Inicio**.

**Paso 2.** Pegar el siguiente prompt en el panel de Copilot y, donde dice `/Caso_MPA_[INICIALES]`, borrar el texto, escribir `/` y seleccionar su documento:

```text
Crea una presentación ejecutiva de 7 diapositivas a partir de /Caso_MPA_[INICIALES]: contexto, evidencia externa,
hallazgos de los datos, oportunidades, riesgos, propuesta y próximos pasos. Frases cortas, para un líder que debe decidir
si amplía el monitoreo a 12 transformadores.
```

- **Comprobación:** Copilot genera 7 diapositivas con títulos y viñetas. Puede tardar 1 o 2 minutos.
- **Alternativa:** Si Copilot no encuentra el documento, comprobar que esté guardado en OneDrive y volver a referenciarlo.

**Paso 3.** Seleccionar en Excel el gráfico de la Tarea 3, copiarlo (**Ctrl+C**) y pegarlo (**Ctrl+V**) en la diapositiva de **hallazgos de los datos**. Ajustar su tamaño.

**Paso 4.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Presentacion_MPA_[INICIALES].pptx`: en PowerPoint de escritorio, **Archivo > Guardar como**; en PowerPoint para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

### Tarea 6. Revisar la presentación con Copilot (3 min)

**Paso 1.** Pegar en el panel de Copilot de PowerPoint el siguiente prompt:

```text
Revisa esta presentación e identifica diapositivas con exceso de información, afirmaciones no respaldadas por la investigación
o los datos, y aspectos que deberían enfatizarse para una audiencia ejecutiva.
```

- **Comprobación:** una lista de diapositivas con sugerencias (texto excesivo, afirmaciones sin respaldo y puntos para enfatizar).

**Paso 2.** Aplicar al menos dos sugerencias. Por ejemplo: reducir una diapositiva a 3 viñetas o eliminar una cifra sin fuente. Guardar con **Ctrl+S**.

### Resultado esperado

<img src="../../images/p14-resultado.svg" alt="Resultado esperado de la práctica 14" width="720"/>


- Documento Word enriquecido con investigación y hallazgos de datos.
- Libro de Excel con análisis, tabla dinámica y gráfico.
- Presentación ejecutiva revisada.

**Entregable:** documento Word enriquecido con investigación (`Caso_MPA_[INICIALES].docx`), archivo Excel analizado (`Datos_MPA_[INICIALES].xlsx`) y presentación PowerPoint ejecutiva (`Presentacion_MPA_[INICIALES].pptx`), todos del mismo caso del curso.
