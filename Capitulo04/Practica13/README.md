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

**Paso 1.** Abrir **Microsoft Edge**, escribir [m365.cloud.microsoft](https://m365.cloud.microsoft/) en la barra de direcciones y presionar **Enter**. Si se solicita, iniciar sesión con su cuenta corporativa.

- **Qué verás:** la página de inicio de Microsoft 365 Copilot con un cuadro de mensaje al centro y un panel a la izquierda.
- **Alternativa:** Si aparece la página de inicio de Microsoft 365 sin chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Agentes > Crear agente** (o **Nuevo agente**).

- **Qué verás:** el asistente de creación con las pestañas **Describir** y **Configurar**, y un panel de prueba a la derecha.
- **Alternativa:** Si no aparece la opción, avisar al instructor: la creación de agentes no está habilitada para su cuenta.

**Paso 3.** Permanecer en la pestaña **Describir**. Abrir `Diseno_Agente_[INICIALES].docx`, copiar el **prompt de creación** y pegarlo en el cuadro de conversación del asistente. Enviar.

- **Qué verás:** el asistente confirma lo que entendió y puede hacer preguntas (por ejemplo, el nombre o el tono).
- **Importante:** no usar la pestaña Configurar en esta práctica.

**Paso 4.** Responder las preguntas del asistente. Si propone un nombre, escribir: *"Nombre: Revisor de Avance de Iniciativas - [INICIALES]"*.

**Paso 5.** Seleccionar **Crear** (arriba a la derecha). Si se pregunta con quién compartir, elegir **Solo yo**.

- **Qué verás:** un mensaje de confirmación y el agente disponible en **Agentes**.

**Al terminar esta tarea debes tener:**

- ✔ El agente creado y visible en **Agentes**.

---

## Tarea 2. Probar el comportamiento del agente (6 min)

**Objetivo:** Tener documentado el resultado de las 4 pruebas: completa, incompleta, contradictoria y fuera de propósito.

**Por qué:** Un agente se valida con casos difíciles; si solo se prueba con datos completos, fallará con reportes reales.

**Paso 1.** Abrir el agente creado. Abrir `Reporte_Iniciativa_Completo.docx` (en `Laboratorio_Copilot_ISA/Practica13`), seleccionar todo (**Ctrl+A**), copiar (**Ctrl+C**) y, en el agente, escribir *"Revisa este reporte:"* y pegar el contenido. Enviar.

- **Qué verás:** una tabla con los 6 criterios y la **decisión del 13-nov** marcada como **prioritaria** (vence dentro de los próximos 7 días).

**Paso 2.** Repetir con `Reporte_Iniciativa_Incompleto.docx`.

- **Qué verás:** el agente indica que faltan datos (avance, fechas, costos, responsables) y los pide en lugar de concluir el estado.
- **Si no ocurre así:** anotar la prueba como "no cumple"; se corregirá en la Tarea 3.

**Paso 3.** Repetir con `Reporte_Iniciativa_Contradictorio.docx`.

- **Qué verás:** el agente señala que el estado "en verde" contradice el avance de **45 % frente a 60 %** y que el hito "cumplido" contradice la instalación en **5 de 8** subestaciones.

**Paso 4.** Escribir en el agente: *"Escríbeme un poema sobre la energía"*.

- **Qué verás:** el agente explica que su propósito es revisar el avance de iniciativas y no atiende la solicitud.

**Paso 5.** Crear un **Documento en blanco** de Word con una tabla de 4 filas y 4 columnas (**Prueba**, **Resultado esperado**, **Resultado obtenido** y **¿Cumple?**) y registrar las cuatro pruebas.

**Paso 6.** Guardar el archivo: en Word de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Pruebas_Agente_[INICIALES].docx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Word para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Pruebas_Agente_[INICIALES].docx` en la barra de título y el estado **Guardado**.

**Al terminar esta tarea debes tener:**

- ✔ Las 4 pruebas registradas con su resultado.

---

## Tarea 3. Ajustar las instrucciones y volver a probar (3 min)

**Objetivo:** Tener una instrucción mejorada y evidencia de que la prueba más débil mejoró.

**Por qué:** Los agentes se ajustan de forma iterativa con base en lo observado.

**Paso 1.** Elegir la prueba con el resultado más débil según su tabla (por ejemplo, la incompleta, si el agente supuso datos).

**Paso 2.** En **Agentes**, pasar el puntero sobre su agente, seleccionar **…** > **Editar**. En la pestaña **Describir**, escribir el ajuste en lenguaje natural. Ejemplos: *"Si falta un dato, pídelo y no concluyas el estado"* o *"Antes de la tabla, agrega una sección Alertas con las inconsistencias detectadas"*. Seleccionar **Actualizar**.

- **Qué verás:** un mensaje de que el agente se actualizó.

**Paso 3.** Repetir la prueba elegida y registrar el resultado en su tabla en una nueva columna **Después del ajuste**.

**Al terminar esta tarea debes tener:**

- ✔ El ajuste realizado y el resultado antes y después.

---

## Tarea 4. Comparar con Copilot Chat (2 min)

**Objetivo:** Poder explicar qué aporta el agente frente a Copilot Chat.

**Por qué:** Justificar el agente frente al chat ayuda a decidir cuándo vale la pena crear otros.

**Paso 1.** En el panel izquierdo, seleccionar **Copilot** (el chat general, no un agente) y seleccionar **Nuevo chat**.

- **Qué verás:** un chat vacío sin el nombre de ningún agente encima del cuadro de mensaje.

**Paso 2.** Pegar *"Revisa este reporte:"* seguido del contenido de `Reporte_Iniciativa_Contradictorio.docx` y enviar.

**Paso 3.** Comparar con la respuesta del agente y escribir en `Pruebas_Agente_[INICIALES].docx` una sección **Comparación con Copilot Chat** con al menos dos diferencias. Por ejemplo: *"El agente siempre usa la tabla de 6 criterios; el chat cambia la estructura"* o *"El agente marca prioridades y alertas"*. Guardar.

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
