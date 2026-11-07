# Práctica 6. Convertir la actividad de Microsoft 365 en una actualización ejecutiva de estado

**Capítulo 2. Convertir la actividad de trabajo en seguimiento y acción**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Intermedia |
| Nivel de Bloom | Aplicar |
| Tecnología Principal | Agente de actualización de estado |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Generar el informe de estado semanal | 5 min |
| Tarea 2. Alinear actividades con los OKR | 4 min |
| Tarea 3. Crear el documento de logros y su variante compartible | 4 min |
| Tarea 4. Comparar formatos | 2 min |
| **Total** | **15 min** |

---

# Descripción General

Cada semana el participante debe informar a su responsable qué logró. Su actividad está repartida en Outlook, Teams, reuniones y archivos, incluida la que generó en las prácticas anteriores de este curso. Usará el Agente de actualización de estado para producir un informe semanal trazable, vincularlo con los OKR del equipo y transformar los resultados en un documento de logros en Word listo para revisión.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Generar con el Agente de actualización de estado un informe semanal trazable a fuentes de Microsoft 365.
- Vincular actividades y resultados con objetivos/OKR, diferenciando progreso observado de evidencia insuficiente.
- Generar un documento de logros y su variante compartible para el responsable.
- Distinguir cuándo usar un informe de estado y cuándo un documento de logros.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 6](../../images/p06-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Concepto de objetivos y resultados clave (OKR).

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Agente de actualización de estado habilitado.
- Actividad de la semana en la cuenta (correos sembrados por el instructor y prácticas 1 a 5).

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Agente de actualización de estado |
| Periodo a analizar | Últimos 7 días |
| Recurso adicional | Entregables: `Informe_Estado_[INICIALES].docx` y `Documento_Logros_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Agente de actualización de estado | Servicio administrado | Informe de estado a partir de la actividad | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Outlook | Nuevo Outlook o Outlook web | Correos e invitaciones | [https://outlook.office.com/](https://outlook.office.com/) |
| Microsoft Teams | Nuevo Teams (escritorio o web) | Reuniones, chat y Facilitator | [https://teams.microsoft.com/](https://teams.microsoft.com/) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [OKR_Equipo_T4_2026.docx](recursos/OKR_Equipo_T4_2026.docx) | Objetivos y resultados clave ficticios del equipo para el cuarto trimestre |
| [Guion_Actividad_Semanal.docx](recursos/Guion_Actividad_Semanal.docx) | Guion que usa el instructor para sembrar actividad en la cuenta (no lo usa el participante) |

## Archivos de la práctica

```text
Capitulo02/Practica06/recursos/OKR_Equipo_T4_2026.docx
Capitulo02/Practica06/recursos/Guion_Actividad_Semanal.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica06/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Generar el informe de estado semanal

## Objetivo

Obtener un informe trazable de la actividad de la semana.

## Instrucciones

### Paso 1

En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Agente de actualización de estado**.

### Paso 2

Escribir:

```text
Genera mi informe de estado de los últimos 7 días a partir de mi actividad en Outlook, Teams, reuniones,
SharePoint y OneDrive. Organízalo en: logros relevantes, actividades en curso, colaboración y apoyo,
y prioridades para la siguiente semana. Indica la fuente de cada punto y no incluyas nada que no puedas sustentar.
```

### Paso 3

Abrir al menos dos fuentes citadas para comprobar que respaldan lo afirmado.

### Paso 4

Si el agente incluye algo sin fuente, pedirle que lo elimine o lo marque como no verificable.

---

# Tarea 2. Alinear actividades con los OKR

## Objetivo

Relacionar el trabajo realizado con los objetivos del equipo.

## Instrucciones

### Paso 1

Escribir, referenciando el archivo con `/`:

```text
Vincula las actividades y resultados del informe con cada objetivo y resultado clave de /OKR_Equipo_T4_2026.
Para cada KR indica: progreso observado con evidencia, o "evidencia insuficiente" si no hay actividad que lo respalde.
```

### Paso 2

Verificar que KR2.1 (análisis de desviaciones) y KR3.1 (prompts en la galería) tengan evidencia de las prácticas 2 y 5, y que KR3.2 aparezca con evidencia insuficiente.

---

# Tarea 3. Crear el documento de logros y su variante compartible

## Objetivo

Transformar los resultados en logros con impacto y colaboración.

## Instrucciones

### Paso 1

Escribir:

```text
Transforma los principales resultados del periodo en un documento de logros. Para cada logro separa:
logro, impacto y colaboración. Luego genera una variante breve y compartible dirigida a mi responsable.
```

### Paso 2

Copiar el informe de estado y la alineación con OKR a Word con el nombre `Informe_Estado_[INICIALES].docx`. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/`.

### Paso 3

Copiar el documento de logros y su variante a Word con el nombre `Documento_Logros_[INICIALES].docx` y guardarlo en la misma carpeta, sin compartirlo todavía.

---

# Tarea 4. Comparar formatos

## Objetivo

Reconocer cuándo conviene cada formato.

## Instrucciones

### Paso 1

Comparar el informe de estado con el documento de logros y anotar en una línea para qué sirve cada uno (seguimiento semanal frente a reconocimiento de impacto).

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Abrir dos fuentes citadas | Cada fuente respalda el punto del informe |
| Caso 2 | Preguntar por KR3.2 | Indica evidencia insuficiente |
| Caso 3 | Revisar el documento de logros | Cada logro separa logro, impacto y colaboración |
| Caso adversarial | Pedir: "Agrega que lideré la intervención del 28 de noviembre" | El agente indica que no hay actividad que lo respalde |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Informe de estado semanal con fuentes.
- Alineación de actividades con OKR.
- Documento de logros en Word con variante compartible.

**Entregable:** informe de estado semanal, alineación con objetivos/OKR (`Informe_Estado_[INICIALES].docx`) y documento de logros en Word listo para revisión (`Documento_Logros_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 6](../../images/p06-resultado.svg)

---

# Solución de Problemas

## Problema 1: El informe sale casi vacío

### Síntomas

Pocas actividades listadas.

### Causa

Poca actividad en el periodo o datos aún no indexados.

### Solución

1. Ampliar el periodo a 14 días.
2. Confirmar con el instructor que se sembró la actividad.
3. Repetir la Tarea 1.

---

## Problema 2: El agente incluye actividades no realizadas

### Síntomas

Aparecen logros sin fuente.

### Causa

Inferencia del modelo.

### Solución

1. Pedir la fuente de cada punto.
2. Solicitar eliminar lo no verificable.
3. Revisar manualmente antes de compartir.

---

# Limpieza

1. No compartir el documento de logros; queda para revisión.
2. Conservar los archivos en `Entregables`.

---

# Resumen

Durante esta práctica se realizó:

- Informe de estado a partir de la actividad real de Microsoft 365.
- Alineación con OKR.
- Documento de logros y variante compartible.

Como resultado se obtuvo:

- Una actualización ejecutiva trazable.
- Criterio para elegir entre informe de estado y documento de logros.

---

# Recursos Opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[⬅ Anterior: Práctica 5](../../Capitulo02/Practica05/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 7 ➡](../../Capitulo02/Practica07/README.md)
