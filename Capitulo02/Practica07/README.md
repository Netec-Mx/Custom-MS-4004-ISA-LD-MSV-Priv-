# Práctica 7. Obtener una visión integral del estado de un proyecto

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Project Delta Digest · 📄 **Entregable:** Resumen ejecutivo del proyecto, vista para PM y agenda de seguimiento

## Descripción

El proyecto **INT-MDV-2026** tiene señales en correos, archivos, conversaciones y reuniones. El participante usará Project Delta Digest para obtener una revisión integral del proyecto, generar una vista para liderazgo y otra para el gerente del proyecto (PM), distinguir información confirmada de la incompleta y preparar la agenda de la próxima reunión de seguimiento. Al final comparará este agente con el Agente de actualización de estado.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Consultar con Project Delta Digest el estado de un proyecto con avances, hitos, bloqueadores, riesgos y decisiones, con sus fuentes.
- Generar una vista para liderazgo y otra para el PM y comparar cómo cambia el nivel de detalle.
- Diferenciar información confirmada de la incompleta, desactualizada o no verificable.
- Preparar una agenda de seguimiento basada en bloqueadores y decisiones pendientes, previa confirmación.

<img src="../../images/p07-objetivo.svg" alt="Diagrama de la Práctica 7" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Project Delta Digest |
| Archivos de la práctica | [Informe_Avance_INT-MDV_Semana44.docx](recursos/Informe_Avance_INT-MDV_Semana44.docx)<br>[Informe_Avance_INT-MDV_Semana45.docx](recursos/Informe_Avance_INT-MDV_Semana45.docx)<br>[Registro_Decisiones_INT-MDV.xlsx](recursos/Registro_Decisiones_INT-MDV.xlsx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica07/` |
| Código del proyecto | `INT-MDV-2026` |
| Palabras clave | Mirador del Valle, INT-MDV |
| Nombre del entregable | `Estado_Proyecto_INT-MDV_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Consultar el estado del proyecto (4 min)

**Objetivo:** Tener la revisión del proyecto INT-MDV-2026 con avances, hitos, bloqueadores, elementos estancados, riesgos y decisiones, cada uno con su fuente.

**Por qué:** La información del proyecto está repartida en correos, informes, notas y reuniones. El agente la reúne en un solo lugar.

**Paso 1.** Abrir **Microsoft Edge**, ingresar a [m365.cloud.microsoft](https://m365.cloud.microsoft/) e iniciar sesión con su cuenta corporativa si se solicita.

- **Alternativa:** Si no aparece el chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Agentes**, escribir `Project Delta Digest` en la búsqueda y abrir el agente.

- **Qué verás:** el nombre **Project Delta Digest** encima del cuadro de mensaje.
- **Si no ocurre así:** buscarlo en **Todos los agentes**; si no aparece, avisar al instructor.

**Paso 3.** Pegar el siguiente prompt y enviarlo:

```text
Revisa el estado actual del proyecto INT-MDV-2026 (Mirador del Valle). Identifica avances, entregables completados,
actividades en progreso, próximos hitos, bloqueadores, elementos estancados, riesgos y decisiones recientes.
Indica la fuente de cada hallazgo.
```

- **Qué verás:** una revisión del proyecto organizada en avances, entregables completados, actividades en progreso, próximos hitos, bloqueadores, elementos estancados, riesgos y decisiones recientes, con referencias a sus fuentes.

**Paso 4.** Comprobar que aparezcan los cuatro hallazgos clave: ventana de **30 h** frente a 36 h planeadas, permiso ambiental con respuesta el **25-nov**, cliente que pide **reprogramar a diciembre** y **plan con comunidades** sin avance desde hace 2 semanas.

- **Alternativa:** Si el agente no encuentra el proyecto, repetir con la palabra clave "Mirador del Valle" o insertar `/Informe_Avance_INT-MDV_Semana45` y avisar al instructor si sigue sin resultados.

**Al terminar esta tarea debes tener:**

- ✔ La revisión con fuentes.
- ✔ Los 4 hallazgos clave identificados (ventana, permiso, cliente, plan con comunidades).

---

## Tarea 2. Generar la vista para liderazgo y revisar bloqueadores (4 min)

**Objetivo:** Tener una vista breve para liderazgo y cada bloqueador clasificado como seguimiento, escalación o decisión, y como información confirmada o incompleta.

**Por qué:** Liderazgo necesita saber qué decidir, no el detalle operativo, y debe saber qué información es confiable.

**Paso 1.** Pegar el siguiente prompt:

```text
Genera una vista para liderazgo: resultados, riesgos, hitos, fechas y aspectos que requieren atención, con poco detalle operativo.
```

- **Qué verás:** una vista más corta centrada en resultados, riesgos, hitos y fechas, con poco detalle operativo.

**Paso 2.** Pegar el siguiente prompt:

```text
Para cada bloqueador y riesgo indica si requiere seguimiento, escalación o decisión, y clasifica la información como
confirmada, incompleta, desactualizada o no verificable.
```

- **Qué verás:** cada bloqueador y riesgo con dos etiquetas: una acción (seguimiento, escalación o decisión) y la calidad de la información (confirmada, incompleta, desactualizada o no verificable).

**Paso 3.** Revisar que el permiso ambiental y la ventana del operador estén marcados como **escalación** o **decisión**, que la solicitud del cliente de reprogramar a diciembre aparezca como asunto que requiere **decisión**, y que el plan con comunidades se marque como **estancado** o **incompleto**.

**Al terminar esta tarea debes tener:**

- ✔ La vista para liderazgo.
- ✔ La clasificación de cada bloqueador y riesgo.

---

## Tarea 3. Generar la vista para el PM y comparar (3 min)

**Objetivo:** Tener la vista para el PM y tres diferencias anotadas frente a la vista de liderazgo.

**Por qué:** El mismo proyecto se comunica distinto según quién debe actuar.

**Paso 1.** Pegar el siguiente prompt:

```text
Genera ahora una versión para el gerente del proyecto (PM), con el detalle operativo necesario para gestionar las actividades.
```

- **Qué verás:** una versión más extensa con actividades, responsables y fechas operativas.

**Paso 2.** Abrir un **Documento en blanco** de Word y escribir tres diferencias entre la vista de liderazgo y la del PM. Por ejemplo: **extensión** (número de líneas), **nivel de detalle** (decisiones frente a tareas) y **tipo de acción** (escalar frente a ejecutar).

**Al terminar esta tarea debes tener:**

- ✔ La vista para el PM.
- ✔ Tres diferencias anotadas.

---

## Tarea 4. Preparar la agenda de seguimiento y comparar con el Agente de actualización de estado (4 min)

**Objetivo:** Tener la agenda confirmada y el entregable guardado con la comparación entre agentes.

**Por qué:** Los bloqueadores solo se resuelven si se tratan en la siguiente reunión con un responsable.

**Paso 1.** Pegar el siguiente prompt:

```text
Con base en los bloqueadores y decisiones pendientes, propón la agenda para la próxima reunión de seguimiento.
Muéstramela primero para confirmarla antes de darla por final.
```

- **Qué verás:** una propuesta de agenda y una pregunta del agente para que usted la confirme o la ajuste.

**Paso 2.** Revisar la agenda: debe incluir la ventana del operador, el permiso ambiental, la respuesta al cliente y el vocero. Responder *"Confirmo la agenda"* o pedir un ajuste concreto (por ejemplo, *"Agrega 10 minutos para el plan con comunidades"*).

**Paso 3.** En el documento de Word de la Tarea 3, copiar y pegar la vista de liderazgo, la vista para el PM y la agenda confirmada. Al final, agregar una línea: *"Agente de actualización de estado: actividad de una persona o equipo. Project Delta Digest: seguimiento integral de un proyecto."*

**Paso 4.** Guardar el archivo en **OneDrive > Laboratorio_Copilot_ISA > Entregables** con el nombre `Estado_Proyecto_INT-MDV_[INICIALES].docx`: en Word de escritorio, **Archivo > Guardar como**; en Word para la web, hacer clic en el nombre del documento en la parte superior y elegir la carpeta.

**Al terminar esta tarea debes tener:**

- ✔ La agenda confirmada por usted.
- ✔ La línea de comparación entre agentes.
- ✔ `Estado_Proyecto_INT-MDV_[INICIALES].docx` guardado.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué elemento está estancado?" | Plan de comunicación con comunidades, con fuente |
| Caso 2 | Comparar vistas | La vista de liderazgo es más corta y prioriza decisiones |
| Caso 3 | Pedir la agenda | El agente muestra la agenda para confirmación antes de cerrarla |
| Caso adversarial | Preguntar: "¿Ya se aprobó la ventana de 36 horas?" | El agente indica que solo hay aprobación preliminar de 30 horas |

## Resultado esperado

- Resumen ejecutivo del estado del proyecto con fuentes.
- Vista para PM.
- Agenda de seguimiento confirmada.

**Entregable:** resumen ejecutivo del estado del proyecto, vista para PM y agenda de seguimiento basada en bloqueadores y decisiones pendientes (`Estado_Proyecto_INT-MDV_[INICIALES].docx`).

<img src="../../images/p07-resultado.svg" alt="Resultado final de la Práctica 7" width="640"/>

## Solución de problemas

**El agente no encuentra el proyecto**
- *Síntoma:* Responde que no hay información de INT-MDV-2026.
- *Causa:* Las fuentes no están en el conocimiento disponible para el agente.
- *Solución:* (1) Usar también la palabra clave "Mirador del Valle". (2) Confirmar acceso al sitio `INT-MDV (Laboratorio)`. (3) Referenciar los informes con `/`.

**Mezcla con otros proyectos**
- *Síntoma:* Aparecen datos de proyectos distintos.
- *Causa:* Palabras clave ambiguas.
- *Solución:* (1) Pedir que se limite al código INT-MDV-2026. (2) Repetir la Tarea 1.

## Limpieza

- Conservar el entregable; se usa como referencia en las prácticas 9 y 11.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Intermedia · Nivel de Bloom: Analizar</sub>

---

[⬅ Anterior: Práctica 6](../../Capitulo02/Practica06/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 8 ➡](../../Capitulo03/Practica08/README.md)
