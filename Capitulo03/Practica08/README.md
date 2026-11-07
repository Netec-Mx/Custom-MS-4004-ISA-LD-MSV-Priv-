# Práctica 8. Identificar cambios y novedades relevantes en la organización

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

⏱️ **Duración:** 12 min · 🛠️ **Herramienta:** Agente de resumen personal de noticias · 📄 **Entregable:** Panorama de novedades clasificado por temática, relevancia e implicaciones, con fuentes

## Descripción

Durante la semana se publicaron comunicaciones del liderazgo, un cambio de procedimiento, una iniciativa de sostenibilidad, una alerta de seguridad, una actualización operativa y un boletín recurrente (todas ficticias). El participante usará el Agente de resumen personal de noticias para entender qué es relevante para su trabajo, profundizar en un tema y ponerse al día tras simular varios días de ausencia.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Obtener un resumen de novedades de la última semana agrupado por temática.
- Diferenciar cambios importantes, información contextual y comunicaciones recurrentes.
- Profundizar en una temática para comprender antecedentes, alcance e implicaciones por área.
- Sintetizar lo ocurrido durante una ausencia con referencias a las fuentes originales.

<img src="../../images/p08-objetivo.svg" alt="Diagrama de la Práctica 8" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Resumen personal de noticias |
| Archivos de la práctica | [Comunicado_Liderazgo_Prioridades.docx](recursos/Comunicado_Liderazgo_Prioridades.docx)<br>[Cambio_Procedimiento_Consignaciones.docx](recursos/Cambio_Procedimiento_Consignaciones.docx)<br>[Iniciativa_Sostenibilidad_SF6.docx](recursos/Iniciativa_Sostenibilidad_SF6.docx)<br>[Alerta_Seguridad_Correo.docx](recursos/Alerta_Seguridad_Correo.docx)<br>[Actualizacion_Operacion_Infraestructura.docx](recursos/Actualizacion_Operacion_Infraestructura.docx)<br>[Boletin_Bienestar_Semanal.docx](recursos/Boletin_Bienestar_Semanal.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica08/` |
| Periodo | Semana del 2 al 6 de noviembre de 2026 |
| Nombre del entregable | `Panorama_Novedades_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Resumir las novedades de la semana por temática (4 min)

**Objetivo:** Obtener un panorama clasificado de la semana.

**Paso 1.** En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Resumen personal de noticias**.

**Paso 2.** Escribir:

```text
Resume las novedades organizativas y operativas de la última semana relevantes para mi trabajo en proyectos de infraestructura.
Agrúpalas por temática y clasifícalas como: cambio importante, información contextual o comunicación recurrente.
Incluye la fuente de cada novedad.
```

**Paso 3.** Verificar la clasificación esperada: cambio de procedimiento de consignaciones y alerta de seguridad = **cambio importante**; prioridades del liderazgo, sostenibilidad y actualización operativa = **contextual o importante según el área**; boletín de bienestar = **recurrente**.

---

## Tarea 2. Profundizar en una temática (4 min)

**Objetivo:** Comprender antecedentes, alcance e implicaciones de un cambio.

**Paso 1.** Escribir:

```text
Profundiza en el cambio del procedimiento de solicitud de consignaciones: antecedentes, qué cambia, desde cuándo,
a quién aplica e implicaciones para Operación, Proyectos y Comunicaciones.
```

**Paso 2.** Comprobar que mencione el paso de **15 a 20 días hábiles** de anticipación, el plan de comunicación aprobado y la vigencia desde el **1-dic-2026**.

**Paso 3.** Preguntar si el cambio afecta la intervención INT-MDV-2026 (28-nov) y verificar que el agente note que inicia antes de la vigencia.

---

## Tarea 3. Ponerse al día después de una ausencia (4 min)

**Objetivo:** Identificar lo que cambió durante varios días fuera.

**Paso 1.** Escribir:

```text
Estuve ausente del 2 al 6 de noviembre. ¿Qué cambió en ese periodo que debo conocer al volver? Prioriza lo que requiere acción
de mi parte e indica la fuente original para ampliar cada tema.
```

**Paso 2.** Copiar el panorama, la profundización y la síntesis a Word. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Panorama_Novedades_[INICIALES].docx`.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué alerta de seguridad hubo?" | Campaña de correos que suplanta proveedores, con fuente |
| Caso 2 | Preguntar desde cuándo aplica el cambio de consignaciones | 1 de diciembre de 2026 |
| Caso 3 | Pedir comunicaciones recurrentes | Boletín de bienestar |
| Caso adversarial | Preguntar: "¿Qué dijo el comunicado sobre despidos?" | El agente indica que no existe esa información |

## Resultado esperado

- Panorama de novedades clasificado por temática y relevancia.
- Análisis de implicaciones de un cambio.
- Síntesis de regreso con fuentes originales.

**Entregable:** panorama de novedades organizativas clasificado por temática, relevancia e implicaciones, con referencias a las fuentes originales (`Panorama_Novedades_[INICIALES].docx`).

<img src="../../images/p08-resultado.svg" alt="Resultado final de la Práctica 8" width="640"/>

## Solución de problemas

**El agente no encuentra las comunicaciones**
- *Síntoma:* Resumen vacío o genérico.
- *Causa:* Las noticias no se publicaron o no están indexadas.
- *Solución:* (1) Confirmar con el instructor la publicación en el sitio de noticias de laboratorio. (2) Referenciar los documentos con `/`. (3) Repetir la Tarea 1.

## Limpieza

- Conservar el entregable en `Entregables`.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Fácil · Nivel de Bloom: Comprender</sub>

---

[⬅ Anterior: Práctica 7](../../Capitulo02/Practica07/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 9 ➡](../../Capitulo03/Practica09/README.md)
