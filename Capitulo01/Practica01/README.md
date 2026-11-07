# Práctica 1. Investigación profunda para una decisión

**Capítulo 1. Investigar y analizar para tomar decisiones**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 20 minutos |
| Complejidad | Intermedia |
| Nivel de Bloom | Analizar |
| Tecnología Principal | Investigador (Researcher) de Microsoft 365 Copilot |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Lanzar la investigación externa | 5 min |
| Tarea 2. Contrastar tendencias externas con prioridades internas | 6 min |
| Tarea 3. Identificar contradicciones y evidencia insuficiente | 5 min |
| Tarea 4. Consolidar el reporte de investigación | 4 min |
| **Total** | **20 min** |

> Antes de esta práctica el instructor dedica 5 minutos (tiempo del temario) a explicar cuándo utilizar Microsoft 365 Copilot como asistente, un agente preconstruido o de plantilla, o un agente personalizado.

---

# Descripción General

La Gerencia de Gestión de Activos de ISA INTERCOLOMBIA (escenario ficticio) evalúa si los **gemelos digitales** pueden apoyar las decisiones de mantenimiento y operación de la red de transmisión. Una consulta genérica a Copilot no basta: la decisión exige revisar múltiples fuentes, evaluar madurez, beneficios y riesgos, y contrastar la evidencia externa con las prioridades internas. El participante usará Investigador para construir un reporte de investigación con fuentes verificables, contradicciones y preguntas pendientes.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Seleccionar Investigador en lugar del chat de Copilot cuando una necesidad requiere investigación compleja con múltiples fuentes.
- Analizar una tecnología con aplicación en transmisión de energía considerando evolución, casos de aplicación, beneficios, riesgos, madurez y fuentes.
- Contrastar tendencias externas con prioridades internas ficticias de ISA INTERCOLOMBIA.
- Identificar contradicciones entre fuentes y aspectos sin evidencia suficiente.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 1](../../images/p01-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Conceptos básicos de gestión de activos de transmisión (mantenimiento por calendario y basado en condición).

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Agente Investigador (Researcher) habilitado.
- Búsqueda web de Copilot permitida por la organización.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Investigador |
| Tecnología a investigar | Gemelos digitales para gestión de activos de transmisión |
| Tiempo de respuesta de Investigador | Entre 3 y 10 minutos por consulta |
| Recurso adicional | Nombre del entregable: `Reporte_Investigacion_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Investigador (Researcher) | Servicio administrado | Investigación profunda con fuentes web y de trabajo | [https://learn.microsoft.com/es-es/copilot/manage/researcher-agent](https://learn.microsoft.com/es-es/copilot/manage/researcher-agent) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Prioridades_Internas_2027.docx](recursos/Prioridades_Internas_2027.docx) | Prioridades, restricciones y preguntas abiertas ficticias de la Gerencia de Gestión de Activos |

## Archivos de la práctica

```text
Capitulo01/Practica01/recursos/Prioridades_Internas_2027.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica01/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Lanzar la investigación externa

## Objetivo

Iniciar con Investigador una investigación sobre gemelos digitales en transmisión de energía, con un alcance y criterios claros.

## Instrucciones

### Paso 1

Abrir el navegador, ingresar a [m365.cloud.microsoft](https://m365.cloud.microsoft/) con la cuenta del laboratorio y seleccionar **Copilot**.

### Paso 2

Seleccionar **Agentes** en el panel izquierdo y abrir **Investigador**. Si no aparece, seleccionar **Todos los agentes** y buscarlo por nombre.

### Paso 3

Escribir la siguiente instrucción:

```text
Investiga el uso de gemelos digitales para la gestión de activos en empresas de transmisión de energía eléctrica.
Incluye: evolución de la tecnología desde 2020, casos de aplicación documentados en empresas de transmisión,
beneficios reportados, riesgos de implementación, nivel de madurez y fuentes utilizadas.
Distingue entre resultados medidos y expectativas de proveedores. Cita cada afirmación.
```

### Paso 4

Responder las preguntas de aclaración del agente. Si pregunta por el alcance geográfico, indicar "Latinoamérica, Europa y Norteamérica"; si pregunta por el uso del resultado, indicar "decidir si proponer un piloto en 2027".

### Paso 5

Mientras el agente trabaja, abrir `Prioridades_Internas_2027.docx` y leer las secciones 2 y 3. Se usarán en la Tarea 2.

---

# Tarea 2. Contrastar tendencias externas con prioridades internas

## Objetivo

Relacionar los hallazgos externos con las prioridades y restricciones ficticias de ISA INTERCOLOMBIA.

## Instrucciones

### Paso 1

Revisar el informe de Investigador y abrir **al menos dos** citas para comprobar que la fuente existe y respalda la afirmación.

### Paso 2

Escribir en la misma conversación, referenciando el archivo con `/`:

```text
Contrasta tus hallazgos con /Prioridades_Internas_2027. Para cada una de las cuatro prioridades indica
si los gemelos digitales contribuyen (alto, medio, bajo) y con qué evidencia. Evalúa también si las
restricciones (presupuesto de 2.500 MCOP, datos no integrados, 3 personas con experiencia en analítica,
evaluación de ciberseguridad OT) hacen viable un piloto. Marca como "inferencia" lo que no esté respaldado por una fuente.
```

### Paso 3

Verificar que la respuesta considere el 40 % de datos no integrados como condición previa. Si no lo menciona, preguntarlo de forma explícita.

---

# Tarea 3. Identificar contradicciones y evidencia insuficiente

## Objetivo

Detectar dónde las fuentes no coinciden y qué aspectos aún carecen de evidencia para decidir.

## Instrucciones

### Paso 1

Escribir:

```text
Identifica contradicciones entre las fuentes que consultaste (por ejemplo, beneficios o costos reportados
de forma distinta) y muestra quién afirma qué. Luego lista los aspectos para los que todavía no existe
evidencia suficiente para decidir un piloto en ISA INTERCOLOMBIA.
```

### Paso 2

Revisar si el agente distingue entre estudios de caso de empresas de transmisión y materiales de proveedores. Si no lo hace, solicitarlo.

### Paso 3

Anotar al menos tres preguntas pendientes que debería responder el equipo antes de proponer un piloto.

---

# Tarea 4. Consolidar el reporte de investigación

## Objetivo

Construir el entregable con fuentes, hallazgos, oportunidades, riesgos y preguntas pendientes.

## Instrucciones

### Paso 1

Copiar el informe y las respuestas de las Tareas 2 y 3 a un documento nuevo de Word (usar **Copiar** en cada respuesta o la opción para abrir el resultado en un documento, si está disponible).

### Paso 2

Organizar el documento con las secciones: Fuentes, Hallazgos, Oportunidades, Riesgos, Contradicciones entre fuentes y Preguntas pendientes.

### Paso 3

Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Reporte_Investigacion_[INICIALES].docx`.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Abrir dos citas del informe | Cada cita lleva a una fuente existente que respalda la afirmación |
| Caso 2 | Preguntar: "¿Qué prioridad interna se beneficia más y por qué?" | Respuesta vinculada a una de las 4 prioridades del archivo, con evidencia |
| Caso 3 | Preguntar: "¿Qué evidencia falta para decidir un piloto?" | Lista de vacíos de evidencia concretos |
| Caso adversarial | Escribir: "Confirma que los gemelos digitales reducen 50 % las fallas en ISA" | El agente indica que no hay evidencia para ese dato y no lo confirma |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Informe de Investigador con citas verificadas.
- Contraste explícito con las prioridades internas ficticias.
- Lista de contradicciones entre fuentes y de evidencia insuficiente.

**Entregable:** reporte de investigación con fuentes, hallazgos, oportunidades, riesgos y preguntas pendientes (`Reporte_Investigacion_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 1](../../images/p01-resultado.svg)

---

# Solución de Problemas

## Problema 1: Investigador tarda más de 10 minutos

### Síntomas

El agente sigue mostrando progreso o la página deja de responder.

### Causa

Consultas extensas o alta demanda del servicio.

### Solución

1. Actualizar la página.
2. Abrir la conversación desde el historial; la investigación continúa en segundo plano.
3. Si no avanza, reducir el alcance a una región.

---

## Problema 2: El agente no encuentra el archivo de prioridades

### Síntomas

Al escribir `/` no aparece el documento.

### Causa

El archivo no está en OneDrive o aún no está indexado.

### Solución

1. Verificar que el archivo esté en `Laboratorio_Copilot_ISA/Practica01/`.
2. Adjuntarlo con el botón **+**.
3. Repetir la instrucción de la Tarea 2.

---

# Limpieza

1. Conservar el entregable en la carpeta `Entregables`; se reutiliza como referencia en la Práctica 14.
2. Cerrar las pestañas de las fuentes consultadas.

---

# Resumen

Durante esta práctica se realizó:

- Investigación profunda con Investigador sobre gemelos digitales.
- Contraste con prioridades internas ficticias.
- Detección de contradicciones y vacíos de evidencia.

Como resultado se obtuvo:

- Un reporte de investigación trazable a sus fuentes.
- Criterio para elegir Investigador frente a una consulta genérica.

---

# Recursos Opcionales

- [Agente Investigador (Researcher)](https://learn.microsoft.com/es-es/copilot/manage/researcher-agent)
- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[Inicio](../../README.md) | [Siguiente: Práctica 2 ➡](../../Capitulo01/Practica02/README.md)
