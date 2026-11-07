# Práctica 13. Crear, probar y ajustar el agente personalizado

**Capítulo 4. Combinar capacidades para resolver una necesidad completa**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Avanzada |
| Nivel de Bloom | Crear |
| Tecnología Principal | Agent Builder (creación con lenguaje natural) |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Crear el agente con lenguaje natural | 4 min |
| Tarea 2. Probar el comportamiento del agente | 6 min |
| Tarea 3. Ajustar las instrucciones y volver a probar | 3 min |
| Tarea 4. Comparar con Copilot Chat | 2 min |
| **Total** | **15 min** |

---

# Descripción General

A partir del prompt diseñado en la Práctica 12, el participante creará su agente con lenguaje natural (sin configuración manual), lo probará con reportes completos, incompletos y contradictorios y con una solicitud fuera de propósito, ajustará sus instrucciones y comparará su resultado con Copilot Chat.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Crear un agente personalizado mediante lenguaje natural a partir de un prompt de diseño.
- Validar su comportamiento con información completa, incompleta, contradictoria y fuera de propósito.
- Ajustar las instrucciones según los resultados y comprobar la mejora.
- Comparar el agente con Copilot Chat para reconocer el valor de la especialización y la consistencia.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 13](../../images/p13-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Haber completado la Práctica 12.

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Permiso para crear agentes con Agent Builder.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Crear agente |
| Nombre del agente | `Revisor de Avance de Iniciativas - [INICIALES]` |
| Modo de creación | Pestaña **Describir** (lenguaje natural); no usar **Configurar** |
| Recurso adicional | Nombre del entregable: agente creado y `Pruebas_Agente_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Agent Builder | Servicio administrado | Creación de agentes personalizados | [https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Reporte_Iniciativa_Completo.docx](recursos/Reporte_Iniciativa_Completo.docx) | Reporte con todos los criterios (prueba de calidad) |
| [Reporte_Iniciativa_Incompleto.docx](recursos/Reporte_Iniciativa_Incompleto.docx) | Reporte sin datos (prueba de datos faltantes) |
| [Reporte_Iniciativa_Contradictorio.docx](recursos/Reporte_Iniciativa_Contradictorio.docx) | Reporte con contradicciones (prueba de inconsistencias) |

## Archivos de la práctica

```text
Capitulo04/Practica13/recursos/Reporte_Iniciativa_Completo.docx
Capitulo04/Practica13/recursos/Reporte_Iniciativa_Incompleto.docx
Capitulo04/Practica13/recursos/Reporte_Iniciativa_Contradictorio.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica13/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Crear el agente con lenguaje natural

## Objetivo

Construir el agente a partir del prompt de diseño.

## Instrucciones

### Paso 1

En la aplicación Microsoft 365 Copilot, seleccionar **Agentes** y luego **Crear agente**.

### Paso 2

Permanecer en la pestaña **Describir** y pegar el prompt de creación de `Diseno_Agente_[INICIALES].docx`.

### Paso 3

Responder las preguntas del asistente de creación y, si propone un nombre, cambiarlo por `Revisor de Avance de Iniciativas - [INICIALES]`.

### Paso 4

Seleccionar **Crear** y mantener el agente visible solo para el participante.

---

# Tarea 2. Probar el comportamiento del agente

## Objetivo

Validar el agente en cuatro situaciones.

## Instrucciones

### Paso 1

Abrir `Reporte_Iniciativa_Completo.docx`, copiar su contenido y pegarlo en el agente con el texto "Revisa este reporte:". Verificar los 6 criterios y que la **decisión del 13-nov** aparezca como prioritaria.

### Paso 2

Repetir con `Reporte_Iniciativa_Incompleto.docx`. Verificar que el agente **pida los datos faltantes** (avance, fechas, costo, responsables) en lugar de suponerlos.

### Paso 3

Repetir con `Reporte_Iniciativa_Contradictorio.docx`. Verificar que señale que el estado "en verde" contradice el avance de **45 % frente a 60 %** y que el hito "cumplido" contradice la instalación en **5 de 8** subestaciones.

### Paso 4

Escribir una solicitud fuera de propósito: `Escríbeme un poema sobre la energía`. Verificar que el agente explique su propósito.

### Paso 5

Registrar cada resultado en `Pruebas_Agente_[INICIALES].docx`.

---

# Tarea 3. Ajustar las instrucciones y volver a probar

## Objetivo

Mejorar el comportamiento con base en las pruebas.

## Instrucciones

### Paso 1

Seleccionar el agente, abrir la opción para editarlo y, en **Describir**, escribir el ajuste necesario. Ejemplo: "Antes de la tabla, agrega una sección Alertas con las inconsistencias detectadas".

### Paso 2

Guardar los cambios y repetir la prueba que tuvo el resultado más débil.

### Paso 3

Registrar el antes y el después en el documento de pruebas.

---

# Tarea 4. Comparar con Copilot Chat

## Objetivo

Reconocer el valor de la especialización.

## Instrucciones

### Paso 1

Abrir el chat de Copilot, pegar el reporte contradictorio con el texto "Revisa este reporte:" y comparar con el resultado del agente.

### Paso 2

Anotar en el documento qué aporta el agente (estructura constante, prioridades, alertas) y cuándo se justifica crearlo. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/`.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Reporte completo | Tabla con 6 criterios y decisión del 13-nov marcada como prioritaria |
| Caso 2 | Reporte incompleto | El agente pide los datos faltantes y no concluye el estado |
| Caso 3 | Reporte contradictorio | Señala las contradicciones antes de concluir |
| Caso adversarial | "Escríbeme un poema sobre la energía" | El agente explica su propósito y no atiende la solicitud |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Agente personalizado creado con lenguaje natural.
- Cuatro pruebas documentadas.
- Instrucciones refinadas y comparación con Copilot Chat.

**Entregable:** agente personalizado funcional y validado, con instrucciones refinadas a partir de las pruebas (evidencia en `Pruebas_Agente_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 13](../../images/p13-resultado.svg)

---

# Solución de Problemas

## Problema 1: La opción Crear agente no aparece

### Síntomas

No se muestra en Agentes.

### Causa

La creación de agentes no está habilitada para el usuario.

### Solución

1. Informar al instructor (Setup_Guide, V-10).
2. Continuar documentando las pruebas con el diseño de la Práctica 12.

---

## Problema 2: El agente supone datos faltantes

### Síntomas

Concluye el estado del reporte incompleto.

### Causa

Las instrucciones no son explícitas.

### Solución

1. Agregar: "Si falta un dato, pídelo y no concluyas".
2. Repetir la prueba.

---

# Limpieza

1. Mantener el agente solo para el participante; no compartirlo con la organización.
2. Si la política lo exige, eliminar el agente al finalizar el curso.

---

# Resumen

Durante esta práctica se realizó:

- Creación de un agente con lenguaje natural.
- Pruebas con información completa, incompleta, contradictoria y fuera de propósito.
- Ajuste y comparación con Copilot Chat.

Como resultado se obtuvo:

- Un agente validado y consistente para una tarea recurrente.

---

# Recursos Opcionales

- [Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder)
- [Crear agentes con Agent Builder](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder-build-agents)

---

[⬅ Anterior: Práctica 12](../../Capitulo04/Practica12/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 14 ➡](../../Capitulo04/Practica14/README.md)
