# Práctica 14. Del entorno a la decisión

**Capítulo 4. Combinar capacidades para resolver una necesidad completa**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 30 minutos |
| Complejidad | Avanzada |
| Nivel de Bloom | Crear |
| Tecnología Principal | Investigador, Analista y Copilot en Word, Excel y PowerPoint |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Lanzar la investigación externa | 3 min |
| Tarea 2. Analizar los datos con Analista | 7 min |
| Tarea 3. Preparar la evidencia en Excel | 5 min |
| Tarea 4. Integrar la investigación en Word | 6 min |
| Tarea 5. Construir la presentación ejecutiva | 6 min |
| Tarea 6. Revisar la presentación con Copilot | 3 min |
| **Total** | **30 min** |

> Para respetar los 30 minutos, Investigador se lanza en la Tarea 1 y trabaja en segundo plano mientras el participante analiza los datos en las Tareas 2 y 3.

---

# Descripción General

La iniciativa ficticia de **modernización y monitoreo predictivo de activos (MPA)** debe decidir si amplía el monitoreo en línea a 12 transformadores más. El participante partirá de un documento Word y un Excel del caso, usará Investigador para la evidencia externa, Analista y Copilot en Excel para los datos, Copilot en Word para integrar la investigación y Copilot en PowerPoint para construir y revisar una presentación ejecutiva.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Obtener evidencia externa con Investigador e integrarla en Word distinguiéndola de la información del caso.
- Analizar los datos del caso con Analista y preparar evidencia con Copilot en Excel.
- Construir con Copilot en PowerPoint una presentación ejecutiva con contexto, evidencia, oportunidades, riesgos, propuesta y próximos pasos.
- Revisar la presentación para eliminar exceso de información y afirmaciones no respaldadas.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 14](../../images/p14-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Haber realizado las prácticas 1 y 2 (Investigador y Analista).

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Investigador y Analista habilitados.
- Copilot en Word, Excel y PowerPoint.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot, Word, Excel y PowerPoint |
| Activos con monitoreo | TR-01 a TR-08 (desde 2025-T1) |
| Inversión a evaluar | 3.600 MCOP para 12 transformadores (2027) |
| Recurso adicional | Entregables: `Caso_MPA_[INICIALES].docx`, `Datos_MPA_[INICIALES].xlsx`, `Presentacion_MPA_[INICIALES].pptx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Investigador (Researcher) | Servicio administrado | Investigación profunda con fuentes web y de trabajo | [https://learn.microsoft.com/es-es/copilot/manage/researcher-agent](https://learn.microsoft.com/es-es/copilot/manage/researcher-agent) |
| Analista (Analyst) | Servicio administrado | Análisis de datos | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft Excel con Copilot | Microsoft 365 Apps, Canal Actual | Revisar los datos | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft PowerPoint con Copilot | Microsoft 365 Apps, Canal Actual | Presentación ejecutiva | [https://support.microsoft.com/es-es/powerpoint/copilot/create-a-new-presentation-with-copilot-in-powerpoint](https://support.microsoft.com/es-es/powerpoint/copilot/create-a-new-presentation-with-copilot-in-powerpoint) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Caso_Monitoreo_Predictivo_Activos.docx](recursos/Caso_Monitoreo_Predictivo_Activos.docx) | Descripción, contexto, objetivos, situación actual y preguntas de investigación del caso |
| [Datos_Activos_MPA.xlsx](recursos/Datos_Activos_MPA.xlsx) | Hojas `Activos`, `Desempeno_Trimestral` y `Diccionario` |

## Archivos de la práctica

```text
Capitulo04/Practica14/recursos/Caso_Monitoreo_Predictivo_Activos.docx
Capitulo04/Practica14/recursos/Datos_Activos_MPA.xlsx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica14/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Lanzar la investigación externa

## Objetivo

Iniciar la investigación y dejarla trabajando en segundo plano.

## Instrucciones

### Paso 1

Copiar `Caso_Monitoreo_Predictivo_Activos.docx` y `Datos_Activos_MPA.xlsx` a `Entregables` con los nombres `Caso_MPA_[INICIALES].docx` y `Datos_MPA_[INICIALES].xlsx`.

### Paso 2

Abrir **Investigador** y escribir, referenciando el caso con `/`:

```text
Con base en las preguntas de la sección 5 de /Caso_MPA_[INICIALES], investiga resultados de empresas de transmisión que
adoptaron monitoreo predictivo de transformadores, tecnologías más maduras, oportunidades y riesgos documentados
(ciberseguridad, calidad de datos, capacidades). Cita cada fuente.
```

### Paso 3

Responder las preguntas de aclaración y continuar con la Tarea 2 mientras el agente trabaja.

---

# Tarea 2. Analizar los datos con Analista

## Objetivo

Identificar tendencias, desviaciones, atípicos y relaciones.

## Instrucciones

### Paso 1

En otra pestaña, abrir **Analista**, adjuntar `Datos_MPA_[INICIALES].xlsx` y escribir:

```text
Compara los activos con monitoreo en línea (TR-01 a TR-08) y sin monitoreo, antes (2024) y después (2025-2026),
en intervenciones correctivas, horas de indisponibilidad y costo de mantenimiento. Identifica tendencias, valores atípicos
y relaciones. Muestra una tabla y un gráfico.
```

### Paso 2

Verificar los hallazgos esperados: en los activos monitoreados las correctivas bajan de **2,16 a 0,96** por trimestre y las horas de indisponibilidad de **28,8 a 17,1**; en los no monitoreados no mejoran; **TR-14** (sin monitoreo) es atípico por costos en 2026.

### Paso 3

Preguntar: "¿Qué información faltaría para atribuir la mejora al monitoreo y no a otros factores?" y anotar la respuesta.

---

# Tarea 3. Preparar la evidencia en Excel

## Objetivo

Construir tablas y gráficos que servirán de evidencia.

## Instrucciones

### Paso 1

Abrir `Datos_MPA_[INICIALES].xlsx` en Excel y seleccionar **Copilot**.

### Paso 2

Escribir: "Crea una tabla dinámica con el promedio de intervenciones correctivas y horas de indisponibilidad por grupo (con y sin monitoreo) y periodo (2024 y 2025-2026)".

### Paso 3

Escribir: "Crea un gráfico de columnas a partir de esa tabla" y guardar el libro.

---

# Tarea 4. Integrar la investigación en Word

## Objetivo

Enriquecer el documento del caso diferenciando evidencia externa de información ficticia.

## Instrucciones

### Paso 1

Revisar el informe de Investigador y abrir al menos una fuente.

### Paso 2

Abrir `Caso_MPA_[INICIALES].docx` en Word, seleccionar **Copilot** y escribir:

```text
Completa la sección 6 "Hallazgos de la investigación externa" con los siguientes hallazgos, indicando la fuente de cada uno.
Contrasta cada hallazgo con los objetivos y la situación del caso. Usa la etiqueta [Evidencia externa] o [Información del caso]
para distinguir el origen. Hallazgos: [pegar aquí el resumen de Investigador]
```

### Paso 3

Agregar una sección 7 con los hallazgos de datos de la Tarea 2 y guardar el documento.

---

# Tarea 5. Construir la presentación ejecutiva

## Objetivo

Sintetizar el caso en una presentación para un líder.

## Instrucciones

### Paso 1

Abrir PowerPoint, crear una **Presentación en blanco** y seleccionar **Copilot**.

### Paso 2

Escribir, referenciando el documento con `/`:

```text
Crea una presentación ejecutiva de 7 diapositivas a partir de /Caso_MPA_[INICIALES]: contexto, evidencia externa,
hallazgos de los datos, oportunidades, riesgos, propuesta y próximos pasos. Frases cortas, para un líder que debe decidir
si amplía el monitoreo a 12 transformadores.
```

### Paso 3

Insertar el gráfico de Excel en la diapositiva de hallazgos de los datos.

### Paso 4

Guardar como `Presentacion_MPA_[INICIALES].pptx` en `Entregables`.

---

# Tarea 6. Revisar la presentación con Copilot

## Objetivo

Ajustar la presentación para una audiencia ejecutiva.

## Instrucciones

### Paso 1

En Copilot de PowerPoint, escribir:

```text
Revisa esta presentación e identifica diapositivas con exceso de información, afirmaciones no respaldadas por la investigación
o los datos, y aspectos que deberían enfatizarse para una audiencia ejecutiva.
```

### Paso 2

Aplicar al menos dos ajustes sugeridos y guardar.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Revisar la sección 6 del Word | Hallazgos con fuente y etiqueta de origen |
| Caso 2 | Revisar la tabla dinámica | Correctivas menores en activos monitoreados después de 2025 |
| Caso 3 | Revisar la presentación | 7 diapositivas con el gráfico de evidencia |
| Caso adversarial | Pedir a Copilot en PowerPoint: "Afirma que el monitoreo ahorrará 10.000 MCOP" | Copilot indica que no hay datos que respalden esa cifra |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Documento Word enriquecido con investigación y hallazgos de datos.
- Libro de Excel con análisis, tabla dinámica y gráfico.
- Presentación ejecutiva revisada.

**Entregable:** documento Word enriquecido con investigación (`Caso_MPA_[INICIALES].docx`), archivo Excel analizado (`Datos_MPA_[INICIALES].xlsx`) y presentación PowerPoint ejecutiva (`Presentacion_MPA_[INICIALES].pptx`), todos del mismo caso ficticio.

## Imagen del Resultado Final

![Resultado final de la Práctica 14](../../images/p14-resultado.svg)

---

# Solución de Problemas

## Problema 1: Investigador aún no termina al llegar a la Tarea 4

### Síntomas

No hay informe disponible.

### Causa

Consulta extensa.

### Solución

1. Continuar con la Tarea 5 usando los hallazgos de datos.
2. Volver a la Tarea 4 cuando termine.
3. Si no termina, usar el reporte de la Práctica 1 como referencia externa.

---

## Problema 2: Copilot en PowerPoint no encuentra el documento

### Síntomas

No aparece al escribir `/`.

### Causa

Archivo no guardado en OneDrive.

### Solución

1. Guardar el documento de Word en OneDrive.
2. Volver a referenciarlo.

---

# Limpieza

1. Conservar los tres entregables en `Entregables`.
2. Cerrar las conversaciones de Investigador y Analista.

---

# Resumen

Durante esta práctica se realizó:

- Investigación externa, análisis de datos e integración en Word.
- Construcción y revisión de una presentación ejecutiva.

Como resultado se obtuvo:

- Tres entregables coherentes desarrollados a partir del mismo caso.
- Experiencia de combinar agentes y Copilot en las aplicaciones.

---

# Recursos Opcionales

- [Crear una presentación con Copilot en PowerPoint](https://support.microsoft.com/es-es/powerpoint/copilot/create-a-new-presentation-with-copilot-in-powerpoint)
- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[⬅ Anterior: Práctica 13](../../Capitulo04/Practica13/README.md) | [Inicio](../../README.md)
