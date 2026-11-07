# Práctica 11. Optimizar una solicitud compleja con Prompt Coach

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Prompt Coach · 📄 **Entregable:** Prompt inicial, diagnóstico, prompt optimizado y comparación de resultados

## Descripción

Un analista necesita identificar los riesgos de INT-MDV-2026, priorizarlos y preparar recomendaciones para su líder. Su primera solicitud a Copilot es vaga. El participante ejecutará esa solicitud, usará Prompt Coach para diagnosticarla, construirá una versión optimizada, comparará los resultados y pedirá una segunda optimización para cambiar el propósito a una síntesis para liderazgo.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Ejecutar una solicitud compleja mejorable y evaluar su resultado.
- Usar Prompt Coach para diagnosticar claridad, contexto, fuentes, criterios, restricciones y formato.
- Construir y ejecutar un prompt optimizado y comparar resultados.
- Ajustar el prompt para un propósito distinto sin reconstruirlo desde cero.

<img src="../../images/p11-objetivo.svg" alt="Diagrama de la Práctica 11" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Prompt Coach |
| Archivos de la práctica | [Plantilla_Comparacion_Prompts.docx](recursos/Plantilla_Comparacion_Prompts.docx)<br>[Plan_Intervencion_Mirador_del_Valle.docx](../../Capitulo02/Practica04/recursos/Plan_Intervencion_Mirador_del_Valle.docx) — Fuente del análisis (Práctica 4)<br>[Matriz_Riesgos_Intervencion.xlsx](../../Capitulo02/Practica04/recursos/Matriz_Riesgos_Intervencion.xlsx) — Fuente del análisis (Práctica 4)<br>[Informe_Avance_INT-MDV_Semana45.docx](../../Capitulo02/Practica07/recursos/Informe_Avance_INT-MDV_Semana45.docx) — Fuente del análisis (Práctica 7) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica11/` |
| Fuentes del análisis | `Plan_Intervencion_Mirador_del_Valle`, `Matriz_Riesgos_Intervencion`, `Informe_Avance_INT-MDV_Semana45` |
| Nombre del entregable | `Comparacion_Prompts_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

> **Nota:** Al terminar esta práctica, el instructor dedica 3 minutos (tiempo del temario) al cierre del módulo: cuándo conviene un agente especializado para mantenerse actualizado, comunicar, preparar información ejecutiva u optimizar solicitudes.

---

## Tarea 1. Ejecutar la solicitud original (3 min)

**Objetivo:** Tener registrados el prompt original y su resultado en la plantilla.

**Por qué:** El resultado de un prompt vago es el punto de comparación para medir la mejora.

**Paso 1.** Abrir **Microsoft Edge**, escribir [m365.cloud.microsoft](https://m365.cloud.microsoft/) en la barra de direcciones y presionar **Enter**. Si se solicita, iniciar sesión con su cuenta corporativa.

- **Qué verás:** la página de inicio de Microsoft 365 Copilot con un cuadro de mensaje al centro y un panel a la izquierda.
- **Alternativa:** Si aparece la página de inicio de Microsoft 365 sin chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Copilot** (el chat general, no un agente) y seleccionar **Nuevo chat**.

- **Qué verás:** un chat vacío sin el nombre de ningún agente encima del cuadro de mensaje.

**Paso 3.** Pegar exactamente este prompt, sin cambios, y enviarlo:

```text
Revisa lo del proyecto de la subestación y dime los riesgos y qué hacer.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una respuesta general, probablemente sin fuentes concretas, sin prioridades claras o que pregunta a qué proyecto se refiere. Ese es el comportamiento esperado de un prompt vago.

**Paso 4.** En OneDrive, abrir `Laboratorio_Copilot_ISA > Practica11`, seleccionar `Plantilla_Comparacion_Prompts.docx`, elegir **Copiar a > Entregables** y cambiar el nombre de la copia a `Comparacion_Prompts_[INICIALES].docx`. Abrir la copia.

**Paso 5.** En la sección **1. Prompt inicial**, pegar el prompt. En la tabla de la sección **4**, columna **Resultado con prompt inicial**, escribir una frase por criterio. Por ejemplo, Precisión: *"no menciona riesgos concretos del proyecto"*.

**Al terminar esta tarea debes tener:**

- ✔ Prompt y resultado registrados en la plantilla.

---

## Tarea 2. Diagnosticar la solicitud con Prompt Coach (4 min)

**Objetivo:** Tener el diagnóstico de Prompt Coach sobre objetivo, contexto, fuentes, criterios, restricciones y formato.

**Por qué:** Saber qué le faltaba al prompt permite corregirlo con intención, no por prueba y error.

**Paso 1.** En otra pestaña, abrir **Agentes** y buscar `Prompt Coach`. Hacer clic en el agente.

- **Qué verás:** el nombre **Prompt Coach** encima del cuadro de mensaje.
- **Si no ocurre así:** buscar en **Todos los agentes** o avisar al instructor.

**Paso 2.** Pegar el siguiente prompt y enviarlo:

```text
Evalúa este prompt y dime cómo mejorarlo en claridad del objetivo, contexto, fuentes, criterios de análisis,
restricciones y formato de respuesta: "Revisa lo del proyecto de la subestación y dime los riesgos y qué hacer."
Contexto: soy analista y debo preparar recomendaciones priorizadas para mi líder sobre el proyecto INT-MDV-2026.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** recomendaciones organizadas por aspecto (objetivo, contexto, fuentes, criterios, restricciones y formato) y, a veces, una versión sugerida del prompt.

**Paso 3.** Copiar el diagnóstico y pegarlo en la sección **2. Diagnóstico de Prompt Coach** de su documento.

**Al terminar esta tarea debes tener:**

- ✔ El diagnóstico pegado en la sección 2.

---

## Tarea 3. Construir el prompt optimizado y comparar (5 min)

**Objetivo:** Tener el prompt optimizado, su resultado y la tabla de comparación completa.

**Por qué:** Comparar muestra qué cambios en la instrucción producen mejores resultados.

**Paso 1.** Construir el prompt optimizado con las recomendaciones. Puede partir de este ejemplo y ajustarlo:

```text
Actúa como analista de proyectos. Con base en /Plan_Intervencion_Mirador_del_Valle, /Matriz_Riesgos_Intervencion e
/Informe_Avance_INT-MDV_Semana45, identifica los riesgos del proyecto INT-MDV-2026, priorízalos por probabilidad e impacto
y por fecha de la intervención (28-nov-2026), y propone una recomendación por riesgo con responsable sugerido.
No incluyas riesgos sin fuente. Entrega una tabla y un resumen de 5 líneas para mi líder.
```

**Paso 2.** Volver al chat de **Copilot** (no a Prompt Coach), seleccionar **Nuevo chat**, pegar el prompt optimizado y reemplazar cada texto que inicia con `/` por el archivo correspondiente: escribir `/` y seleccionar `Plan_Intervencion_Mirador_del_Valle`, `Matriz_Riesgos_Intervencion` e `Informe_Avance_INT-MDV_Semana45`. Enviar.

- **Qué verás:** una tabla de riesgos priorizada con recomendación y responsable, seguida de un resumen de 5 líneas.
- **Alternativa:** Si algún archivo no aparece, adjuntarlo con **+** desde `Laboratorio_Copilot_ISA/Practica04` o `Practica07`.

**Paso 3.** Pegar el prompt optimizado en la sección **3** y completar la tabla de la sección **4**: para cada criterio (precisión, estructura, profundidad y utilidad), describir el resultado optimizado y el **cambio del prompt** que explica la diferencia. Por ejemplo: *"Estructura: tabla priorizada; cambio: se pidió formato de tabla"*.

**Al terminar esta tarea debes tener:**

- ✔ El prompt optimizado en la sección 3.
- ✔ La tabla de la sección 4 completa, con el cambio que explica cada diferencia.

---

## Tarea 4. Solicitar una segunda optimización (3 min)

**Objetivo:** Saber qué elementos del prompt cambiar para pasar del análisis detallado a una síntesis para liderazgo.

**Por qué:** Un buen prompt se adapta cambiando pocos elementos, sin reescribirlo.

**Paso 1.** Volver a **Prompt Coach** y pegar el siguiente prompt:

```text
Quiero usar el prompt optimizado para producir una síntesis de un párrafo para liderazgo en lugar del análisis detallado.
¿Qué elementos debo modificar y cuáles conservar?
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una lista de elementos para cambiar (por ejemplo, el formato y la extensión) y elementos para conservar (fuentes y criterios).

**Paso 2.** Copiar la respuesta en la sección **5. Segunda optimización** de su documento.

**Paso 3.** Guardar el documento con **Ctrl+S** (o, en Word para la web, comprobar que diga **Guardado**). El archivo debe llamarse `Comparacion_Prompts_[INICIALES].docx` y estar en `Entregables`.

**Al terminar esta tarea debes tener:**

- ✔ La sección 5 completa.
- ✔ `Comparacion_Prompts_[INICIALES].docx` guardado.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Comparar ambos resultados | El prompt optimizado produce una tabla priorizada con fuentes |
| Caso 2 | Revisar el diagnóstico | Cubre objetivo, contexto, fuentes, criterios, restricciones y formato |
| Caso 3 | Revisar la segunda optimización | Cambia formato y extensión y conserva fuentes y criterios |
| Caso adversarial | Pedir a Prompt Coach: "Responde tú los riesgos del proyecto" | El agente se enfoca en mejorar el prompt o aclara su propósito |

## Resultado esperado

- Prompt inicial y su resultado.
- Diagnóstico de Prompt Coach.
- Prompt optimizado con comparación de resultados y segunda optimización.

**Entregable:** prompt inicial, diagnóstico de Prompt Coach, prompt optimizado y comparación de resultados (`Comparacion_Prompts_[INICIALES].docx`).

<img src="../../images/p11-resultado.svg" alt="Resultado final de la Práctica 11" width="640"/>

## Solución de problemas

**Copilot no usa las fuentes indicadas**
- *Síntoma:* El resultado es genérico.
- *Causa:* Los archivos no se referenciaron con `/`.
- *Solución:* (1) Escribir `/` y seleccionar cada archivo. (2) Volver a ejecutar el prompt optimizado.

## Limpieza

- Conservar la plantilla completada en `Entregables`.
- Opcional: guardar el prompt optimizado en la Galería de indicaciones.

## Recursos opcionales

- [Galería de indicaciones](https://m365.cloud.microsoft/copilot-prompts)
- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Evaluar</sub>

---

[⬅ Anterior: Práctica 10](../../Capitulo03/Practica10/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 12 ➡](../../Capitulo04/Practica12/README.md)
