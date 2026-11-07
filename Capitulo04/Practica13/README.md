# Práctica 13. Crear, probar y ajustar el agente personalizado

**Capítulo 4. Combinar capacidades para resolver una necesidad completa**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Agent Builder (creación con lenguaje natural) · 📄 **Entregable:** Agente personalizado funcional y validado con instrucciones refinadas

## Descripción

A partir del prompt diseñado en la Práctica 12, el participante creará su agente con lenguaje natural (sin configuración manual), lo probará con reportes completos, incompletos y contradictorios y con una solicitud fuera de propósito, ajustará sus instrucciones y comparará su resultado con Copilot Chat.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Crear un agente personalizado mediante lenguaje natural a partir de un prompt de diseño.
- Validar su comportamiento con información completa, incompleta, contradictoria y fuera de propósito.
- Ajustar las instrucciones según los resultados y comprobar la mejora.
- Comparar el agente con Copilot Chat para reconocer el valor de la especialización y la consistencia.

<img src="../../images/p13-objetivo.svg" alt="Diagrama de la Práctica 13" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Crear agente |
| Archivos de la práctica | [Reporte_Iniciativa_Completo.docx](recursos/Reporte_Iniciativa_Completo.docx)<br>[Reporte_Iniciativa_Incompleto.docx](recursos/Reporte_Iniciativa_Incompleto.docx)<br>[Reporte_Iniciativa_Contradictorio.docx](recursos/Reporte_Iniciativa_Contradictorio.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica13/` |
| Nombre del agente | `Revisor de Avance de Iniciativas - [INICIALES]` |
| Modo de creación | Pestaña **Describir** (lenguaje natural); no usar **Configurar** |
| Nombre del entregable | agente creado y `Pruebas_Agente_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Crear el agente con lenguaje natural (4 min)

**Objetivo:** Tener creado el agente `Revisor de Avance de Iniciativas - [INICIALES]` a partir del prompt de diseño.

**Por qué:** Crear con lenguaje natural permite construir un agente sin configuración técnica.

**Paso 1.** En la aplicación Microsoft 365 Copilot, seleccionar **Agentes** y luego **Crear agente**.

**Paso 2.** Permanecer en la pestaña **Describir** y pegar el prompt de creación de `Diseno_Agente_[INICIALES].docx`.

**Paso 3.** Responder las preguntas del asistente de creación y, si propone un nombre, cambiarlo por `Revisor de Avance de Iniciativas - [INICIALES]`.

**Paso 4.** Seleccionar **Crear** y mantener el agente visible solo para el participante.

**Al terminar esta tarea debes tener:**

- ✔ El agente creado y visible en **Agentes**.

---

## Tarea 2. Probar el comportamiento del agente (6 min)

**Objetivo:** Tener documentado el resultado de las 4 pruebas: completa, incompleta, contradictoria y fuera de propósito.

**Por qué:** Un agente se valida con casos difíciles; si solo se prueba con datos completos, fallará con reportes reales.

**Paso 1.** Abrir `Reporte_Iniciativa_Completo.docx`, copiar su contenido y pegarlo en el agente con el texto "Revisa este reporte:". Verificar los 6 criterios y que la **decisión del 13-nov** aparezca como prioritaria.

**Paso 2.** Repetir con `Reporte_Iniciativa_Incompleto.docx`. Verificar que el agente **pida los datos faltantes** (avance, fechas, costo, responsables) en lugar de suponerlos.

**Paso 3.** Repetir con `Reporte_Iniciativa_Contradictorio.docx`. Verificar que señale que el estado "en verde" contradice el avance de **45 % frente a 60 %** y que el hito "cumplido" contradice la instalación en **5 de 8** subestaciones.

**Paso 4.** Escribir una solicitud fuera de propósito: `Escríbeme un poema sobre la energía`. Verificar que el agente explique su propósito.

**Paso 5.** Crear un **Documento en blanco** de Word con una tabla de 4 filas (prueba, resultado esperado, resultado obtenido, ¿cumple?) y registrar cada prueba. Seleccionar **Archivo > Guardar como**, elegir **OneDrive > Laboratorio_Copilot_ISA > Entregables** y guardar con el nombre `Pruebas_Agente_[INICIALES].docx`.

**Al terminar esta tarea debes tener:**

- ✔ Las 4 pruebas registradas con su resultado.

---

## Tarea 3. Ajustar las instrucciones y volver a probar (3 min)

**Objetivo:** Tener una instrucción mejorada y evidencia de que la prueba más débil mejoró.

**Por qué:** Los agentes se ajustan de forma iterativa con base en lo observado.

**Paso 1.** Seleccionar el agente, abrir la opción para editarlo y, en **Describir**, escribir el ajuste necesario. Ejemplo: "Antes de la tabla, agrega una sección Alertas con las inconsistencias detectadas".

**Paso 2.** Guardar los cambios y repetir la prueba que tuvo el resultado más débil.

**Paso 3.** Registrar el antes y el después en el documento de pruebas.

**Al terminar esta tarea debes tener:**

- ✔ El ajuste realizado y el resultado antes y después.

---

## Tarea 4. Comparar con Copilot Chat (2 min)

**Objetivo:** Poder explicar qué aporta el agente frente a Copilot Chat.

**Por qué:** Justificar el agente frente al chat ayuda a decidir cuándo vale la pena crear otros.

**Paso 1.** Abrir el chat de Copilot, pegar el reporte contradictorio con el texto "Revisa este reporte:" y comparar con el resultado del agente.

**Paso 2.** Anotar en el documento qué aporta el agente (estructura constante, prioridades, alertas) y cuándo se justifica crearlo. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/`.

**Al terminar esta tarea debes tener:**

- ✔ La comparación registrada en `Pruebas_Agente_[INICIALES].docx`.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Reporte completo | Tabla con 6 criterios y decisión del 13-nov marcada como prioritaria |
| Caso 2 | Reporte incompleto | El agente pide los datos faltantes y no concluye el estado |
| Caso 3 | Reporte contradictorio | Señala las contradicciones antes de concluir |
| Caso adversarial | "Escríbeme un poema sobre la energía" | El agente explica su propósito y no atiende la solicitud |

## Resultado esperado

- Agente personalizado creado con lenguaje natural.
- Cuatro pruebas documentadas.
- Instrucciones refinadas y comparación con Copilot Chat.

**Entregable:** agente personalizado funcional y validado, con instrucciones refinadas a partir de las pruebas (evidencia en `Pruebas_Agente_[INICIALES].docx`).

<img src="../../images/p13-resultado.svg" alt="Resultado final de la Práctica 13" width="640"/>

## Solución de problemas

**La opción Crear agente no aparece**
- *Síntoma:* No se muestra en Agentes.
- *Causa:* La creación de agentes no está habilitada para el usuario.
- *Solución:* (1) Informar al instructor (Setup_Guide, V-10). (2) Continuar documentando las pruebas con el diseño de la Práctica 12.

**El agente supone datos faltantes**
- *Síntoma:* Concluye el estado del reporte incompleto.
- *Causa:* Las instrucciones no son explícitas.
- *Solución:* (1) Agregar: "Si falta un dato, pídelo y no concluyas". (2) Repetir la prueba.

## Limpieza

- Mantener el agente solo para el participante; no compartirlo con la organización.
- Si la política lo exige, eliminar el agente al finalizar el curso.

## Recursos opcionales

- [Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder)
- [Crear agentes con Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder-build-agents)

<sub>Complejidad: Avanzada · Nivel de Bloom: Crear</sub>

---

[⬅ Anterior: Práctica 12](../../Capitulo04/Practica12/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 14 ➡](../../Capitulo04/Practica14/README.md)
