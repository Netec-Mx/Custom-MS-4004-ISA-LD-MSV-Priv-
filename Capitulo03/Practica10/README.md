# Práctica 10. Presentar los avances e innovaciones de ISA ante el sector energético

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Agente de informe ejecutivo · 📄 **Entregable:** Briefing ejecutivo en Word con mensajes, antecedentes, preguntas y respuestas y consideraciones

## Descripción

Un líder de ISA INTERCOLOMBIA intervendrá en el **Foro de Transmisión y Confiabilidad 2026** (evento ficticio). El participante usará el Agente de informe ejecutivo para preparar el briefing: confirmar el contexto del evento, investigar información **pública** sobre avances y proyectos de la organización, estructurar mensajes estratégicos, anticipar preguntas y revisar qué afirmaciones carecen de evidencia o requieren aprobación.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Proporcionar al agente el contexto del evento y confirmarlo antes de preparar el briefing.
- Investigar avances, proyectos e innovaciones con información pública y fuentes especializadas.
- Estructurar mensajes estratégicos y preguntas y respuestas previstas.
- Diferenciar hechos respaldados por fuentes públicas de expectativas que requieren validación.

<img src="../../images/p10-objetivo.svg" alt="Diagrama de la Práctica 10" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Agente de informe ejecutivo |
| Archivos de la práctica | [Ficha_Evento_Sector_Energetico.docx](recursos/Ficha_Evento_Sector_Energetico.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica10/` |
| Evento | Foro de Transmisión y Confiabilidad 2026 (ficticio), 3-dic-2026 |
| Regla del escenario | Solo información pública verificable, con fuente y fecha |
| Nombre del entregable | `Briefing_Evento_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios, excepto la información pública que consulta el agente; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Proporcionar y confirmar el contexto del evento (3 min)

**Objetivo:** Asegurar que el agente trabaje con el contexto correcto.

**Paso 1.** En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Agente de informe ejecutivo**.

**Paso 2.** Escribir, referenciando la ficha con `/`:

```text
Voy a preparar la intervención de un líder de ISA INTERCOLOMBIA en el evento descrito en /Ficha_Evento_Sector_Energetico.
Antes de empezar, confirma conmigo el evento, la fecha, el formato, la audiencia y el objetivo.
```

**Paso 3.** Revisar el resumen del agente y confirmarlo o corregirlo.

---

## Tarea 2. Investigar avances y proyectos con información pública (4 min)

**Objetivo:** Obtener hallazgos respaldados por fuentes públicas.

**Paso 1.** Escribir:

```text
Investiga avances, proyectos de modernización, innovaciones tecnológicas y mejoras de ISA INTERCOLOMBIA en transmisión de energía,
usando información pública de la organización y fuentes especializadas. Para cada hallazgo indica fuente y fecha.
Identifica logros, beneficios documentados, tendencias del sector y oportunidades futuras.
```

**Paso 2.** Abrir al menos dos fuentes y comprobar que sean públicas y estén vigentes.

---

## Tarea 3. Estructurar mensajes y preguntas previstas (5 min)

**Objetivo:** Preparar el contenido de la intervención.

**Paso 1.** Escribir:

```text
Estructura 3 a 5 mensajes estratégicos para presentar la evolución de ISA INTERCOLOMBIA y su contribución a la confiabilidad,
eficiencia y sostenibilidad. Luego prepara 6 preguntas probables de los asistentes (resultados, desafíos, inversiones,
innovación y proyectos futuros) con respuestas, marcando cada una como "respaldada por fuente pública" o "requiere validación".
```

**Paso 2.** Revisar que ninguna respuesta anuncie inversiones o proyectos no publicados.

---

## Tarea 4. Revisar afirmaciones y generar el documento (3 min)

**Objetivo:** Detectar afirmaciones sin evidencia o sensibles y producir el briefing en Word.

**Paso 1.** Escribir:

```text
Revisa los mensajes y respuestas: identifica afirmaciones sin evidencia suficiente, información sensible y contenido que requiera
aprobación antes de comunicarse públicamente. Luego genera el briefing completo como documento.
```

**Paso 2.** Abrir o copiar el briefing en Word. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Briefing_Evento_[INICIALES].docx`.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Revisar la confirmación inicial | El agente confirma fecha, formato, audiencia y objetivo antes de avanzar |
| Caso 2 | Abrir dos fuentes citadas | Fuentes públicas existentes y con fecha |
| Caso 3 | Revisar las preguntas y respuestas | Cada respuesta está clasificada como respaldada o por validar |
| Caso adversarial | Pedir: "Anuncia una inversión de 1 billón de pesos en 2027" | El agente indica que no hay fuente pública y que requiere aprobación |

## Resultado esperado

- Contexto del evento confirmado.
- Hallazgos públicos con fuente y fecha.
- Mensajes, preguntas y respuestas revisados.

**Entregable:** documento Word con briefing ejecutivo para el evento, mensajes estratégicos, antecedentes relevantes, preguntas y respuestas previstas y consideraciones para la intervención (`Briefing_Evento_[INICIALES].docx`).

<img src="../../images/p10-resultado.svg" alt="Resultado final de la Práctica 10" width="640"/>

## Solución de problemas

**El agente usa información no pública**
- *Síntoma:* Aparecen cifras sin fuente.
- *Causa:* Mezcla de inferencias con hechos.
- *Solución:* (1) Pedir la fuente pública de cada cifra. (2) Eliminar o marcar como "requiere validación" lo que no tenga fuente.

**El agente no confirma el contexto**
- *Síntoma:* Empieza a redactar sin confirmar.
- *Causa:* La instrucción no lo pidió explícitamente.
- *Solución:* (1) Indicar "No avances hasta que confirme". (2) Repetir la Tarea 1.

## Limpieza

- No compartir el briefing fuera del curso.
- Conservar el documento en `Entregables`.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Evaluar</sub>

---

[⬅ Anterior: Práctica 9](../../Capitulo03/Practica09/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 11 ➡](../../Capitulo03/Practica11/README.md)
