# Práctica 12. Diseñar un agente para dar seguimiento a una necesidad recurrente

**Capítulo 4. Combinar capacidades para resolver una necesidad completa**

⏱️ **Duración:** 10 min · 🛠️ **Herramienta:** Diseño de agentes personalizados (Agent Builder) · 📄 **Entregable:** Prompt de creación del agente con propósito, instrucciones, criterios, formato y límites

## Descripción

Laura, líder de un equipo (ficticia), revisa cada semana el avance de 5 iniciativas con solicitudes distintas a Copilot y obtiene análisis inconsistentes. El participante decidirá si la necesidad se resuelve mejor con Copilot Chat, un agente disponible o un agente personalizado y, tras compararlos, diseñará el prompt de creación de un agente que aplique siempre los mismos criterios: avance, desviaciones, riesgos, bloqueos, decisiones requeridas y próximos pasos.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Comparar Copilot Chat, un agente disponible y un agente personalizado para una necesidad recurrente.
- Definir propósito, información de entrada, criterios, estructura de respuesta y situaciones prioritarias del agente.
- Definir qué no debe asumir el agente y cómo actuar ante información incompleta o contradictoria.
- Redactar el prompt de creación del agente con propósito, instrucciones, criterios, formato y límites.

<img src="../../images/p12-objetivo.svg" alt="Diagrama de la Práctica 12" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Microsoft Word (plantilla de diseño) |
| Archivos de la práctica | [Escenario_Lider_Iniciativas.docx](recursos/Escenario_Lider_Iniciativas.docx)<br>[Plantilla_Diseno_Agente.docx](recursos/Plantilla_Diseno_Agente.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica12/` |
| Criterios de Laura | Avance, desviaciones, riesgos, bloqueos, decisiones requeridas, próximos pasos |
| Nombre del entregable | `Diseno_Agente_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

> **Nota:** Antes de esta práctica el instructor dedica 5 minutos (tiempo del temario) a explicar cuándo una actividad recurrente justifica crear un agente personalizado.

---

## Tarea 1. Elegir la alternativa adecuada (3 min)

**Objetivo:** Tener completa la tabla comparativa y la justificación de por qué la necesidad requiere un agente personalizado.

**Por qué:** Crear un agente toma tiempo; solo conviene cuando la tarea es recurrente y necesita los mismos criterios cada vez.

**Paso 1.** Abrir `Escenario_Lider_Iniciativas.docx` y leer la necesidad de Laura. En OneDrive, copiar `Plantilla_Diseno_Agente.docx` a `Entregables` con el nombre `Diseno_Agente_[INICIALES].docx` y abrirlo.

**Paso 2.** Completar en la plantilla una comparación breve:

| Alternativa | ¿Aplica los mismos criterios cada vez? | ¿Requiere repetir instrucciones? | Conclusión |
|---|---|---|---|
| Copilot Chat | No garantizado | Sí | |
| Agente disponible | No conoce los criterios de Laura | Sí | |
| Agente personalizado | Sí | No | |

**Paso 3.** Registrar la alternativa elegida y su justificación en la primera fila de la plantilla.

**Al terminar esta tarea debes tener:**

- ✔ La tabla comparativa completa.
- ✔ La alternativa elegida y su justificación.

---

## Tarea 2. Definir el comportamiento del agente (4 min)

**Objetivo:** Tener completa la tabla de diseño: propósito, entradas, criterios, estructura, prioridades, lo que no debe asumir, conducta ante datos incompletos y límites.

**Por qué:** Un agente se comporta según lo que se le define; lo que no se define queda a su criterio.

**Paso 1.** Completar en la plantilla: propósito específico, información que podrá recibir (reportes de avance en texto o documentos), criterios de análisis (los 6 de Laura) y estructura de la respuesta (una tabla con los 6 criterios y un resumen).

**Paso 2.** Definir las situaciones prioritarias: desviación de plazo mayor a 10 días hábiles, bloqueo sin responsable y decisión con fecha límite en los próximos 7 días.

**Paso 3.** Definir lo que el agente no debe asumir (fechas, responsables, cifras ausentes) y su conducta ante información incompleta, contradictoria o insuficiente: señalarla y pedir el dato antes de concluir.

**Paso 4.** Definir límites: no tomar decisiones por la líder y responder solo sobre seguimiento de iniciativas.

**Al terminar esta tarea debes tener:**

- ✔ Las 9 filas de la tabla de diseño completas.

---

## Tarea 3. Redactar el prompt de creación (3 min)

**Objetivo:** Tener el prompt de creación completo en la plantilla, listo para la Práctica 13.

**Por qué:** Este texto se pegará tal cual en Agent Builder, así que debe contener todo el diseño.

**Paso 1.** Redactar el prompt en la sección final de la plantilla. Ejemplo de referencia:

```text
Crea un agente llamado "Revisor de Avance de Iniciativas" que ayude a una líder a revisar reportes de avance de las iniciativas de su equipo.
Cada vez que reciba un reporte debe analizar siempre: avance frente a lo planeado, desviaciones de plazo, costo o alcance, riesgos,
bloqueos, decisiones requeridas y próximos pasos. Debe responder con una tabla de esos 6 criterios (criterio, hallazgo, evidencia del reporte)
y un resumen de 3 líneas. Debe marcar como PRIORITARIO: desviaciones mayores a 10 días hábiles, bloqueos sin responsable y decisiones
con fecha límite en los próximos 7 días. No debe asumir fechas, responsables ni cifras que no estén en el reporte: si falta información
o hay contradicciones, debe señalarlas y pedir el dato antes de concluir. No toma decisiones en nombre de la líder y, si recibe solicitudes
ajenas al seguimiento de iniciativas, debe explicar su propósito.
```

**Paso 2.** Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Diseno_Agente_[INICIALES].docx`. Se usará en la Práctica 13.

**Al terminar esta tarea debes tener:**

- ✔ El prompt de creación con propósito, criterios, formato, prioridades y límites.
- ✔ `Diseno_Agente_[INICIALES].docx` guardado.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Revisar la plantilla | Todos los elementos del diseño están completos |
| Caso 2 | Revisar el prompt | Incluye propósito, criterios, formato, prioridades y límites |
| Caso 3 | Revisar la justificación | Explica por qué la recurrencia y la consistencia requieren un agente personalizado |
| Caso adversarial | Verificar si el prompt dice qué hacer ante datos contradictorios | El prompt indica señalarlos antes de concluir |

## Resultado esperado

- Alternativa elegida y justificada.
- Diseño completo del agente.
- Prompt de creación listo para la Práctica 13.

**Entregable:** prompt de creación del agente, incluyendo propósito, instrucciones, criterios de análisis, formato esperado y límites (`Diseno_Agente_[INICIALES].docx`).

<img src="../../images/p12-resultado.svg" alt="Resultado final de la Práctica 12" width="640"/>

## Solución de problemas

**El diseño es demasiado general**
- *Síntoma:* El propósito admite cualquier tarea.
- *Causa:* No se delimitó el alcance.
- *Solución:* (1) Limitar el propósito al seguimiento de iniciativas. (2) Agregar qué hacer con solicitudes fuera de propósito.

## Limpieza

- Conservar la plantilla completada; es insumo de la Práctica 13.

## Recursos opcionales

- [Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder)
- [Crear agentes con Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder-build-agents)

<sub>Complejidad: Intermedia · Nivel de Bloom: Crear</sub>

---

[⬅ Anterior: Práctica 11](../../Capitulo03/Practica11/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 13 ➡](../../Capitulo04/Practica13/README.md)
