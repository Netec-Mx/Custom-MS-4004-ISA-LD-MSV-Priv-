# Práctica 8. Identificar cambios y novedades relevantes en la organización

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 12 minutos |
| Complejidad | Fácil |
| Nivel de Bloom | Comprender |
| Tecnología Principal | Agente de resumen personal de noticias |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Resumir las novedades de la semana por temática | 4 min |
| Tarea 2. Profundizar en una temática | 4 min |
| Tarea 3. Ponerse al día después de una ausencia | 4 min |
| **Total** | **12 min** |

---

# Descripción General

Durante la semana se publicaron comunicaciones del liderazgo, un cambio de procedimiento, una iniciativa de sostenibilidad, una alerta de seguridad, una actualización operativa y un boletín recurrente (todas ficticias). El participante usará el Agente de resumen personal de noticias para entender qué es relevante para su trabajo, profundizar en un tema y ponerse al día tras simular varios días de ausencia.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Obtener un resumen de novedades de la última semana agrupado por temática.
- Diferenciar cambios importantes, información contextual y comunicaciones recurrentes.
- Profundizar en una temática para comprender antecedentes, alcance e implicaciones por área.
- Sintetizar lo ocurrido durante una ausencia con referencias a las fuentes originales.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 8](../../images/p08-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Uso básico de agentes en Microsoft 365 Copilot.

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Agente Resumen personal de noticias habilitado.
- Comunicaciones publicadas en el sitio de noticias de laboratorio.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Resumen personal de noticias |
| Periodo | Semana del 2 al 6 de noviembre de 2026 |
| Recurso adicional | Nombre del entregable: `Panorama_Novedades_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Resumen personal de noticias | Servicio administrado | Síntesis de novedades organizativas | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Comunicado_Liderazgo_Prioridades.docx](recursos/Comunicado_Liderazgo_Prioridades.docx) | Comunicación del liderazgo |
| [Cambio_Procedimiento_Consignaciones.docx](recursos/Cambio_Procedimiento_Consignaciones.docx) | Cambio en procedimiento interno |
| [Iniciativa_Sostenibilidad_SF6.docx](recursos/Iniciativa_Sostenibilidad_SF6.docx) | Iniciativa institucional de sostenibilidad |
| [Alerta_Seguridad_Correo.docx](recursos/Alerta_Seguridad_Correo.docx) | Alerta de seguridad |
| [Actualizacion_Operacion_Infraestructura.docx](recursos/Actualizacion_Operacion_Infraestructura.docx) | Actualización de operación e infraestructura |
| [Boletin_Bienestar_Semanal.docx](recursos/Boletin_Bienestar_Semanal.docx) | Comunicación recurrente |

## Archivos de la práctica

```text
Capitulo03/Practica08/recursos/Comunicado_Liderazgo_Prioridades.docx
Capitulo03/Practica08/recursos/Cambio_Procedimiento_Consignaciones.docx
Capitulo03/Practica08/recursos/Iniciativa_Sostenibilidad_SF6.docx
Capitulo03/Practica08/recursos/Alerta_Seguridad_Correo.docx
Capitulo03/Practica08/recursos/Actualizacion_Operacion_Infraestructura.docx
Capitulo03/Practica08/recursos/Boletin_Bienestar_Semanal.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica08/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Resumir las novedades de la semana por temática

## Objetivo

Obtener un panorama clasificado de la semana.

## Instrucciones

### Paso 1

En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Resumen personal de noticias**.

### Paso 2

Escribir:

```text
Resume las novedades organizativas y operativas de la última semana relevantes para mi trabajo en proyectos de infraestructura.
Agrúpalas por temática y clasifícalas como: cambio importante, información contextual o comunicación recurrente.
Incluye la fuente de cada novedad.
```

### Paso 3

Verificar la clasificación esperada: cambio de procedimiento de consignaciones y alerta de seguridad = **cambio importante**; prioridades del liderazgo, sostenibilidad y actualización operativa = **contextual o importante según el área**; boletín de bienestar = **recurrente**.

---

# Tarea 2. Profundizar en una temática

## Objetivo

Comprender antecedentes, alcance e implicaciones de un cambio.

## Instrucciones

### Paso 1

Escribir:

```text
Profundiza en el cambio del procedimiento de solicitud de consignaciones: antecedentes, qué cambia, desde cuándo,
a quién aplica e implicaciones para Operación, Proyectos y Comunicaciones.
```

### Paso 2

Comprobar que mencione el paso de **15 a 20 días hábiles** de anticipación, el plan de comunicación aprobado y la vigencia desde el **1-dic-2026**.

### Paso 3

Preguntar si el cambio afecta la intervención INT-MDV-2026 (28-nov) y verificar que el agente note que inicia antes de la vigencia.

---

# Tarea 3. Ponerse al día después de una ausencia

## Objetivo

Identificar lo que cambió durante varios días fuera.

## Instrucciones

### Paso 1

Escribir:

```text
Estuve ausente del 2 al 6 de noviembre. ¿Qué cambió en ese periodo que debo conocer al volver? Prioriza lo que requiere acción
de mi parte e indica la fuente original para ampliar cada tema.
```

### Paso 2

Copiar el panorama, la profundización y la síntesis a Word. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Panorama_Novedades_[INICIALES].docx`.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Preguntar: "¿Qué alerta de seguridad hubo?" | Campaña de correos que suplanta proveedores, con fuente |
| Caso 2 | Preguntar desde cuándo aplica el cambio de consignaciones | 1 de diciembre de 2026 |
| Caso 3 | Pedir comunicaciones recurrentes | Boletín de bienestar |
| Caso adversarial | Preguntar: "¿Qué dijo el comunicado sobre despidos?" | El agente indica que no existe esa información |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Panorama de novedades clasificado por temática y relevancia.
- Análisis de implicaciones de un cambio.
- Síntesis de regreso con fuentes originales.

**Entregable:** panorama de novedades organizativas clasificado por temática, relevancia e implicaciones, con referencias a las fuentes originales (`Panorama_Novedades_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 8](../../images/p08-resultado.svg)

---

# Solución de Problemas

## Problema 1: El agente no encuentra las comunicaciones

### Síntomas

Resumen vacío o genérico.

### Causa

Las noticias no se publicaron o no están indexadas.

### Solución

1. Confirmar con el instructor la publicación en el sitio de noticias de laboratorio.
2. Referenciar los documentos con `/`.
3. Repetir la Tarea 1.

---

# Limpieza

1. Conservar el entregable en `Entregables`.

---

# Resumen

Durante esta práctica se realizó:

- Resumen semanal de novedades.
- Profundización en un cambio de procedimiento.
- Síntesis de regreso tras ausencia.

Como resultado se obtuvo:

- Un panorama organizativo clasificado y trazable.

---

# Recursos Opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[⬅ Anterior: Práctica 7](../../Capitulo02/Practica07/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 9 ➡](../../Capitulo03/Practica09/README.md)
