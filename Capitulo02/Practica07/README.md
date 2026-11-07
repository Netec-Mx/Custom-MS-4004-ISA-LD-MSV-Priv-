# Práctica 7. Obtener una visión integral del estado de un proyecto

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Intermedia |
| Nivel de Bloom | Analizar |
| Tecnología Principal | Project Delta Digest |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Consultar el estado del proyecto | 4 min |
| Tarea 2. Generar la vista para liderazgo y revisar bloqueadores | 4 min |
| Tarea 3. Generar la vista para el PM y comparar | 3 min |
| Tarea 4. Preparar la agenda de seguimiento y comparar con el Agente de actualización de estado | 4 min |
| **Total** | **15 min** |

---

# Descripción General

El proyecto **INT-MDV-2026** tiene señales en correos, archivos, conversaciones y reuniones. El participante usará Project Delta Digest para obtener una revisión integral del proyecto, generar una vista para liderazgo y otra para el gerente del proyecto (PM), distinguir información confirmada de la incompleta y preparar la agenda de la próxima reunión de seguimiento. Al final comparará este agente con el Agente de actualización de estado.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Consultar con Project Delta Digest el estado de un proyecto con avances, hitos, bloqueadores, riesgos y decisiones, con sus fuentes.
- Generar una vista para liderazgo y otra para el PM y comparar cómo cambia el nivel de detalle.
- Diferenciar información confirmada de la incompleta, desactualizada o no verificable.
- Preparar una agenda de seguimiento basada en bloqueadores y decisiones pendientes, previa confirmación.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 7](../../images/p07-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Conceptos de seguimiento de proyectos (hitos, bloqueadores, riesgos).

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Agente Project Delta Digest habilitado.
- Acceso de lectura al sitio de laboratorio `INT-MDV (Laboratorio)`.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Project Delta Digest |
| Código del proyecto | `INT-MDV-2026` |
| Palabras clave | Mirador del Valle, INT-MDV |
| Recurso adicional | Nombre del entregable: `Estado_Proyecto_INT-MDV_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Project Delta Digest | Servicio administrado | Revisión integral del estado de proyectos | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Informe_Avance_INT-MDV_Semana44.docx](recursos/Informe_Avance_INT-MDV_Semana44.docx) | Informe semanal del PM, semana 44 |
| [Informe_Avance_INT-MDV_Semana45.docx](recursos/Informe_Avance_INT-MDV_Semana45.docx) | Informe semanal del PM, semana 45 |
| [Registro_Decisiones_INT-MDV.xlsx](recursos/Registro_Decisiones_INT-MDV.xlsx) | Decisiones tomadas y pendientes del proyecto |

## Archivos de la práctica

```text
Capitulo02/Practica07/recursos/Informe_Avance_INT-MDV_Semana44.docx
Capitulo02/Practica07/recursos/Informe_Avance_INT-MDV_Semana45.docx
Capitulo02/Practica07/recursos/Registro_Decisiones_INT-MDV.xlsx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica07/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Consultar el estado del proyecto

## Objetivo

Obtener una revisión integral con fuentes.

## Instrucciones

### Paso 1

En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Project Delta Digest**.

### Paso 2

Escribir:

```text
Revisa el estado actual del proyecto INT-MDV-2026 (Mirador del Valle). Identifica avances, entregables completados,
actividades en progreso, próximos hitos, bloqueadores, elementos estancados, riesgos y decisiones recientes.
Indica la fuente de cada hallazgo.
```

### Paso 3

Verificar que aparezcan: ventana de **30 h** frente a 36 h, permiso ambiental con respuesta el **25-nov**, cliente que pide reprogramar y plan con comunidades **estancado** desde hace 2 semanas.

---

# Tarea 2. Generar la vista para liderazgo y revisar bloqueadores

## Objetivo

Priorizar lo que necesita atención de liderazgo y clasificar la calidad de la información.

## Instrucciones

### Paso 1

Escribir:

```text
Genera una vista para liderazgo: resultados, riesgos, hitos, fechas y aspectos que requieren atención, con poco detalle operativo.
```

### Paso 2

Escribir:

```text
Para cada bloqueador y riesgo indica si requiere seguimiento, escalación o decisión, y clasifica la información como
confirmada, incompleta, desactualizada o no verificable.
```

---

# Tarea 3. Generar la vista para el PM y comparar

## Objetivo

Reconocer cómo el agente adapta profundidad y detalle según la audiencia.

## Instrucciones

### Paso 1

Escribir:

```text
Genera ahora una versión para el gerente del proyecto (PM), con el detalle operativo necesario para gestionar las actividades.
```

### Paso 2

Anotar tres diferencias entre la vista de liderazgo y la del PM (extensión, nivel de detalle, tipo de acciones).

---

# Tarea 4. Preparar la agenda de seguimiento y comparar con el Agente de actualización de estado

## Objetivo

Convertir bloqueadores y decisiones pendientes en una agenda y elegir el agente adecuado.

## Instrucciones

### Paso 1

Escribir:

```text
Con base en los bloqueadores y decisiones pendientes, propón la agenda para la próxima reunión de seguimiento.
Muéstramela primero para confirmarla antes de darla por final.
```

### Paso 2

Revisar la propuesta y confirmarla o pedir un ajuste.

### Paso 3

Copiar el resumen de liderazgo, la vista para PM y la agenda a Word. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Estado_Proyecto_INT-MDV_[INICIALES].docx`.

### Paso 4

Escribir en el documento una línea que explique cuándo usar el Agente de actualización de estado (actividad de una persona o equipo) y cuándo Project Delta Digest (seguimiento integral de un proyecto).

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué elemento está estancado?" | Plan de comunicación con comunidades, con fuente |
| Caso 2 | Comparar vistas | La vista de liderazgo es más corta y prioriza decisiones |
| Caso 3 | Pedir la agenda | El agente muestra la agenda para confirmación antes de cerrarla |
| Caso adversarial | Preguntar: "¿Ya se aprobó la ventana de 36 horas?" | El agente indica que solo hay aprobación preliminar de 30 horas |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Resumen ejecutivo del estado del proyecto con fuentes.
- Vista para PM.
- Agenda de seguimiento confirmada.

**Entregable:** resumen ejecutivo del estado del proyecto, vista para PM y agenda de seguimiento basada en bloqueadores y decisiones pendientes (`Estado_Proyecto_INT-MDV_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 7](../../images/p07-resultado.svg)

---

# Solución de Problemas

## Problema 1: El agente no encuentra el proyecto

### Síntomas

Responde que no hay información de INT-MDV-2026.

### Causa

Las fuentes no están en el conocimiento disponible para el agente.

### Solución

1. Usar también la palabra clave "Mirador del Valle".
2. Confirmar acceso al sitio `INT-MDV (Laboratorio)`.
3. Referenciar los informes con `/`.

---

## Problema 2: Mezcla con otros proyectos

### Síntomas

Aparecen datos de proyectos distintos.

### Causa

Palabras clave ambiguas.

### Solución

1. Pedir que se limite al código INT-MDV-2026.
2. Repetir la Tarea 1.

---

# Limpieza

1. Conservar el entregable; se usa como referencia en las prácticas 9 y 11.

---

# Resumen

Durante esta práctica se realizó:

- Revisión integral del proyecto con Project Delta Digest.
- Vistas para liderazgo y PM.
- Agenda de seguimiento.

Como resultado se obtuvo:

- Un diagnóstico trazable del proyecto para diferentes audiencias.
- Criterio para elegir entre agentes de estado y de proyecto.

---

# Recursos Opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[⬅ Anterior: Práctica 6](../../Capitulo02/Practica06/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 8 ➡](../../Capitulo03/Practica08/README.md)
