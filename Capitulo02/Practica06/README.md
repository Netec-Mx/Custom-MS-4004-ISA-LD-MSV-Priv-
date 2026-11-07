# Práctica 6. Convertir la actividad de Microsoft 365 en una actualización ejecutiva de estado

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Agente de actualización de estado · 📄 **Entregable:** Informe de estado semanal, alineación con OKR y documento de logros en Word

## Descripción

Cada semana el participante debe informar a su responsable qué logró. Su actividad está repartida en Outlook, Teams, reuniones y archivos, incluida la que generó en las prácticas anteriores de este curso. Usará el Agente de actualización de estado para producir un informe semanal trazable, vincularlo con los OKR del equipo y transformar los resultados en un documento de logros en Word listo para revisión.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Generar con el Agente de actualización de estado un informe semanal trazable a fuentes de Microsoft 365.
- Vincular actividades y resultados con objetivos/OKR, diferenciando progreso observado de evidencia insuficiente.
- Generar un documento de logros y su variante compartible para el responsable.
- Distinguir cuándo usar un informe de estado y cuándo un documento de logros.

<img src="../../images/p06-objetivo.svg" alt="Diagrama de la Práctica 6" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Agente de actualización de estado |
| Archivos de la práctica | [OKR_Equipo_T4_2026.docx](recursos/OKR_Equipo_T4_2026.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica06/` |
| Periodo a analizar | Últimos 7 días |
| Nombre del entregable | `Informe_Estado_[INICIALES].docx` y `Documento_Logros_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Generar el informe de estado semanal (5 min)

**Objetivo:** Obtener un informe trazable de la actividad de la semana.

**Paso 1.** En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Agente de actualización de estado**.

**Paso 2.** Escribir:

```text
Genera mi informe de estado de los últimos 7 días a partir de mi actividad en Outlook, Teams, reuniones,
SharePoint y OneDrive. Organízalo en: logros relevantes, actividades en curso, colaboración y apoyo,
y prioridades para la siguiente semana. Indica la fuente de cada punto y no incluyas nada que no puedas sustentar.
```

**Paso 3.** Abrir al menos dos fuentes citadas para comprobar que respaldan lo afirmado.

**Paso 4.** Si el agente incluye algo sin fuente, pedirle que lo elimine o lo marque como no verificable.

---

## Tarea 2. Alinear actividades con los OKR (4 min)

**Objetivo:** Relacionar el trabajo realizado con los objetivos del equipo.

**Paso 1.** Escribir, referenciando el archivo con `/`:

```text
Vincula las actividades y resultados del informe con cada objetivo y resultado clave de /OKR_Equipo_T4_2026.
Para cada KR indica: progreso observado con evidencia, o "evidencia insuficiente" si no hay actividad que lo respalde.
```

**Paso 2.** Verificar que KR2.1 (análisis de desviaciones) y KR3.1 (prompts en la galería) tengan evidencia de las prácticas 2 y 5, y que KR3.2 aparezca con evidencia insuficiente.

---

## Tarea 3. Crear el documento de logros y su variante compartible (4 min)

**Objetivo:** Transformar los resultados en logros con impacto y colaboración.

**Paso 1.** Escribir:

```text
Transforma los principales resultados del periodo en un documento de logros. Para cada logro separa:
logro, impacto y colaboración. Luego genera una variante breve y compartible dirigida a mi responsable.
```

**Paso 2.** Copiar el informe de estado y la alineación con OKR a Word con el nombre `Informe_Estado_[INICIALES].docx`. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/`.

**Paso 3.** Copiar el documento de logros y su variante a Word con el nombre `Documento_Logros_[INICIALES].docx` y guardarlo en la misma carpeta, sin compartirlo todavía.

---

## Tarea 4. Comparar formatos (2 min)

**Objetivo:** Reconocer cuándo conviene cada formato.

**Paso 1.** Comparar el informe de estado con el documento de logros y anotar en una línea para qué sirve cada uno (seguimiento semanal frente a reconocimiento de impacto).

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Abrir dos fuentes citadas | Cada fuente respalda el punto del informe |
| Caso 2 | Preguntar por KR3.2 | Indica evidencia insuficiente |
| Caso 3 | Revisar el documento de logros | Cada logro separa logro, impacto y colaboración |
| Caso adversarial | Pedir: "Agrega que lideré la intervención del 28 de noviembre" | El agente indica que no hay actividad que lo respalde |

## Resultado esperado

- Informe de estado semanal con fuentes.
- Alineación de actividades con OKR.
- Documento de logros en Word con variante compartible.

**Entregable:** informe de estado semanal, alineación con objetivos/OKR (`Informe_Estado_[INICIALES].docx`) y documento de logros en Word listo para revisión (`Documento_Logros_[INICIALES].docx`).

<img src="../../images/p06-resultado.svg" alt="Resultado final de la Práctica 6" width="640"/>

## Solución de problemas

**El informe sale casi vacío**
- *Síntoma:* Pocas actividades listadas.
- *Causa:* Poca actividad en el periodo o datos aún no indexados.
- *Solución:* (1) Ampliar el periodo a 14 días. (2) Confirmar con el instructor que se sembró la actividad. (3) Repetir la Tarea 1.

**El agente incluye actividades no realizadas**
- *Síntoma:* Aparecen logros sin fuente.
- *Causa:* Inferencia del modelo.
- *Solución:* (1) Pedir la fuente de cada punto. (2) Solicitar eliminar lo no verificable. (3) Revisar manualmente antes de compartir.

## Limpieza

- No compartir el documento de logros; queda para revisión.
- Conservar los archivos en `Entregables`.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Aplicar</sub>

---

[⬅ Anterior: Práctica 5](../../Capitulo02/Practica05/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 7 ➡](../../Capitulo02/Practica07/README.md)
