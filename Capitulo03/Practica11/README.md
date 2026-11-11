# Práctica 11. Optimizar una solicitud compleja con Prompt Coach

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Comparar la respuesta a una solicitud inicial poco precisa con una versión mejorada.
- Diagnosticar un prompt mediante Prompt Coach atendiendo a objetivo, contexto, fuentes, criterios, restricciones y formato.
- Reformular la misma solicitud para una síntesis dirigida a liderazgo.

<img src="../../images/p11-objetivo.svg" alt="Mapa visual de la práctica 11" width="720"/>

## Duración aproximada:

- 15 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Servicio | Copilot Chat y agente Prompt Coach |
| Contexto | Proyecto `INT-MDV-2026`, intervención en Subestación Mirador del Valle |
| Archivos ya preparados | [Plan de intervención](../../Capitulo02/Practica04/recursos/Plan_Intervencion_Mirador_del_Valle.docx), [matriz de riesgos](../../Capitulo02/Practica04/recursos/Matriz_Riesgos_Intervencion.xlsx), [informe de avance](../../Capitulo02/Practica07/recursos/Evolucion_INT-MDV_Semanas44_45.docx) |
| Producto | `Comparacion_Prompts.docx` creado durante la práctica |

## Instrucciones

Se revisará una solicitud deliberadamente ambigua sobre riesgos del proyecto INT-MDV-2026. Se usarán las **mismas fuentes** en la revisión final para identificar qué mejoras provienen de la instrucción y cuáles del contexto adicional.

### Tarea 1. Ejecutar la solicitud inicial (3 min)

**Paso 1.** Abrir [Microsoft Copilot](https://www.microsoft365.com/) con la cuenta autorizada, seleccionar **Copilot Chat** y abrir **Nuevo chat**.

**Paso 2.** Pegar y ejecutar el siguiente texto **sin adjuntar fuentes**, para observar cómo interpreta la solicitud ambigua.

**Prompt 1 - Solicitud inicial**

```text
Revisa lo del proyecto de la subestación y dime los riesgos y qué hacer.
```

**Paso 3.** Leer la respuesta e identificar si reconoce el proyecto, aporta fuentes comprobables, prioriza riesgos o define una salida para liderazgo. No presuponer que será idéntica a la de otros participantes.

### Tarea 2. Diagnosticar con Prompt Coach (4 min)

**Paso 1.** Seleccionar **Agentes** en Copilot y abrir el agente **Prompt Coach** previamente habilitado.

**Paso 2.** Pegar el siguiente diagnóstico y revisar su explicación criterio por criterio.

**Prompt 2 - Diagnóstico**

```text
Evalúa esta indicación: "Revisa lo del proyecto de la subestación y dime los riesgos y qué hacer".
Necesito preparar recomendaciones para liderazgo sobre la intervención INT-MDV-2026.
Indica qué falta en objetivo, contexto, fuentes, criterios de análisis, restricciones y formato.
Propón cambios concretos; no inventes hechos del proyecto.
```

**Paso 3.** Comprobar que el diagnóstico propone identificar fuentes, fechas, criterios de prioridad, reglas contra suposiciones y formato ejecutivo.

### Tarea 3. Ejecutar la versión mejorada (5 min)

**Paso 1.** Abrir otro **Nuevo chat** en Copilot Chat; adjuntar desde OneDrive los archivos `Plan_Intervencion_Mirador_del_Valle.docx`, `Matriz_Riesgos_Intervencion.xlsx` e `Evolucion_INT-MDV_Semanas44_45.docx` (carpetas `Practica04` y `Practica07`).

**Paso 2.** Pegar la versión de referencia; modificarla únicamente si las recomendaciones de Prompt Coach exigen una precisión adicional.

**Prompt 3 - Solicitud mejorada**

```text
Actúa como analista de proyectos. A partir de los tres archivos adjuntos, analiza riesgos de INT-MDV-2026
para la intervención prevista desde el 28 de noviembre de 2026. Prioriza por probabilidad,
impacto y cercanía de fecha. Entrega una tabla: riesgo, dato fuente, estado confirmado/no confirmado,
prioridad, posible responsable y acción sugerida. Distingue los hechos observados de las recomendaciones,
no asumas permisos ni decisiones y termina con una síntesis de cinco líneas dirigida a un líder.
```

**Paso 3.** Comparar el resultado con la respuesta inicial en **precisión, estructura, profundidad y utilidad**, verificando las referencias a la ventana, el permiso ambiental, los clientes y el vocero; distinguir el efecto de **haber adjuntado fuentes** del efecto de **cambiar la redacción**.

**Paso 4.** Crear un Word nuevo en `Entregables/Comparacion_Prompts.docx` e incorporar el prompt inicial, el diagnóstico, la versión mejorada y un breve contraste de los cuatro criterios. Este documento es el producto de la actividad, no una plantilla de control.

### Tarea 4. Optimizar la solicitud para liderazgo (3 min)

**Paso 1.** Volver a Prompt Coach y ejecutar la siguiente segunda solicitud.

**Prompt 4 - Cambio de propósito**

```text
Conserva las fuentes, los criterios de prioridad y la prohibición de suponer datos del prompt mejorado,
pero cambia el resultado para obtener un solo párrafo de síntesis para el director. Indica exactamente
qué modificar y qué mantener sin rehacer el prompt desde cero.
```

**Paso 2.** Aplicar la recomendación al prompt mejorado, ejecutarlo en Copilot Chat con las mismas fuentes y guardar en Word la comparación del resultado ejecutivo con el informe detallado.

### Resultado esperado

<img src="../../images/p11-resultado.svg" alt="Resultado esperado de la práctica 11" width="720"/>


El documento de comparación contiene la solicitud inicial, su diagnóstico, una versión con contexto y fuentes verificables, las diferencias observadas en cuatro criterios y la adaptación para liderazgo. Ninguna afirmación sobre el proyecto se acepta sin contrastarla con un archivo de origen.
