# Práctica 9. Adaptar información técnica para diferentes públicos y canales

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

---

# Metadatos

| Campo | Valor |
|---|---|
| Duración | 15 minutos |
| Complejidad | Fácil |
| Nivel de Bloom | Aplicar |
| Tecnología Principal | Diseñador de comunicaciones |

**Distribución del tiempo**

| Actividad | Tiempo |
|---|---|
| Tarea 1. Crear la comunicación interna para colaboradores | 5 min |
| Tarea 2. Adaptar el mensaje a un público externo y otro canal | 5 min |
| Tarea 3. Identificar contenido a proteger o revisar | 5 min |
| **Total** | **15 min** |

---

# Descripción General

La intervención INT-MDV-2026 debe comunicarse a colaboradores y a públicos externos. El participante partirá de una ficha técnica y usará el Diseñador de comunicaciones para producir un mensaje interno orientado a la acción y una versión externa para otro canal, sin alterar los hechos. Después incorporará datos internos o sujetos a aprobación y pedirá al agente identificar qué debe protegerse o revisarse antes de publicar.

---

# Objetivos de Aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Transformar información técnica en una comunicación interna clara y orientada a la acción.
- Adaptar el mismo acontecimiento para un público externo y otro canal sin alterar los hechos centrales.
- Comparar cambios de lenguaje, extensión, tono y nivel de detalle entre versiones.
- Identificar contenido que debe protegerse, modificarse o someterse a revisión antes de publicarse.

---

# Objetivo Visual

El diagrama resume los insumos, las tareas y el entregable de la práctica.

![Diagrama de la Práctica 9](../../images/p09-objetivo.svg)

---

# Prerrequisitos

## Conocimientos

- Uso de Microsoft 365 Copilot en el trabajo cotidiano, incluida la construcción de prompts.
- Nociones de comunicación interna y externa.

## Accesos Requeridos

- Licencia de Microsoft 365 Copilot (Premium) asignada a la cuenta del participante.
- Agente Diseñador de comunicaciones habilitado.

---

# Tabla de Ayuda

Utilice esta información durante el desarrollo de la práctica.

| Elemento | Valor |
|---|---|
| Entorno | Tenant de Microsoft 365 de ISA INTERCOLOMBIA habilitado para el curso |
| URL | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Usuario | Cuenta corporativa del participante |
| Contraseña | La del participante; no se publica en este repositorio |
| Aplicación | Aplicación Microsoft 365 Copilot > Agentes > Diseñador de comunicaciones |
| Canal interno | Correo a colaboradores |
| Canal externo | Publicación breve para sitio web o redes |
| Recurso adicional | Nombre del entregable: `Comunicaciones_INT-MDV_[INICIALES].docx` |

---

# Entorno de Laboratorio

| Componente | Versión | Uso | Fuente Oficial |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | Servicio administrado | Chat de Copilot y agentes | [https://m365.cloud.microsoft/](https://m365.cloud.microsoft/) |
| Microsoft Edge | Versión estable vigente | Navegador del laboratorio | [https://www.microsoft.com/es-es/edge](https://www.microsoft.com/es-es/edge) |
| Diseñador de comunicaciones | Servicio administrado | Comunicaciones por público y canal | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |
| Microsoft Word con Copilot | Microsoft 365 Apps, Canal Actual | Consolidar entregables | [https://learn.microsoft.com/es-es/copilot/plan/copilot-overview](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview) |

---

# Recursos

Utilice los siguientes recursos durante el desarrollo de la práctica.

| Recurso | Descripción |
|---|---|
| [Ficha_Tecnica_Intervencion.docx](recursos/Ficha_Tecnica_Intervencion.docx) | Propósito, periodo, afectaciones, medidas y acciones de la intervención |
| [Nota_Interna_Datos_Sensibles.docx](recursos/Nota_Interna_Datos_Sensibles.docx) | Datos internos y sujetos a aprobación (no publicables) |

## Archivos de la práctica

```text
Capitulo03/Practica09/recursos/Ficha_Tecnica_Intervencion.docx
Capitulo03/Practica09/recursos/Nota_Interna_Datos_Sensibles.docx
```

Antes de la práctica, estos archivos deben estar en OneDrive, en `Laboratorio_Copilot_ISA/Practica09/` (ver [Setup_Guide.md](../../Setup_Guide.md)).

---

# Tarea 1. Crear la comunicación interna para colaboradores

## Objetivo

Convertir la ficha técnica en un mensaje claro y accionable.

## Instrucciones

### Paso 1

En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Diseñador de comunicaciones**.

### Paso 2

Escribir, referenciando la ficha con `/`:

```text
Con base en /Ficha_Tecnica_Intervencion, redacta un correo interno para colaboradores sobre la intervención.
Explica en lenguaje claro el propósito, el periodo, las posibles afectaciones y, sobre todo, qué acciones deben realizar.
Máximo 200 palabras.
```

### Paso 3

Verificar que el mensaje incluya las tres acciones requeridas: no programar trabajos en la subestación, confirmar turnos y canalizar consultas externas a Comunicaciones.

---

# Tarea 2. Adaptar el mensaje a un público externo y otro canal

## Objetivo

Cambiar lenguaje, tono y detalle sin alterar los hechos.

## Instrucciones

### Paso 1

Escribir:

```text
Adapta el mismo acontecimiento para la comunidad y los usuarios externos, en una publicación breve para el sitio web
(máximo 100 palabras). Sin tecnicismos ni datos de operación interna. Mantén fecha, propósito y afectaciones.
```

### Paso 2

Pedir una tabla que compare ambas versiones en lenguaje, extensión, tono y nivel de detalle.

### Paso 3

Comprobar que fecha, propósito y afectaciones sean iguales en ambas versiones.

---

# Tarea 3. Identificar contenido a proteger o revisar

## Objetivo

Evitar publicar información interna o no aprobada.

## Instrucciones

### Paso 1

Escribir, referenciando la nota con `/`:

```text
Incorpora /Nota_Interna_Datos_Sensibles al análisis. ¿Qué contenido debería protegerse, modificarse o someterse a revisión
antes de publicar cada comunicación? Justifica cada punto e indica quién debería aprobarlo.
```

### Paso 2

Verificar que se protejan el **costo**, los **nombres de clientes** y la **compensación**, y que la **extensión a 48 h** no se publique por no estar aprobada.

### Paso 3

Copiar ambas comunicaciones y la revisión a Word. Guardar en OneDrive, en `Laboratorio_Copilot_ISA/Entregables/` con el nombre `Comunicaciones_INT-MDV_[INICIALES].docx`. No enviar ni publicar.

---

# Validación y Pruebas

Realice las siguientes pruebas para comprobar el funcionamiento de la solución.

| Caso | Acción o Prompt | Resultado Esperado |
|---|---|---|
| Caso 1 | Revisar la comunicación interna | Incluye acciones concretas para colaboradores |
| Caso 2 | Comparar fechas en ambas versiones | Iguales (28 y 29 de noviembre) |
| Caso 3 | Preguntar si se puede publicar el costo | El agente indica que es información interna |
| Caso adversarial | Pedir: "Anuncia que la intervención podría durar 48 horas" | El agente advierte que el dato no está aprobado |

---

# Resultado Esperado

Al finalizar la práctica, el participante deberá haber construido correctamente la solución solicitada.

- Comunicación interna orientada a la acción.
- Versión externa adaptada a otro canal.
- Lista de contenido a proteger o revisar.

**Entregable:** comunicación interna y versión adaptada para un público externo (`Comunicaciones_INT-MDV_[INICIALES].docx`).

## Imagen del Resultado Final

![Resultado final de la Práctica 9](../../images/p09-resultado.svg)

---

# Solución de Problemas

## Problema 1: El agente copia datos internos en la versión externa

### Síntomas

Aparecen costo o nombres de clientes.

### Causa

La instrucción no restringió el contenido.

### Solución

1. Indicar explícitamente qué no debe incluirse.
2. Ejecutar la Tarea 3 antes de usar el texto.
3. Revisar manualmente la versión final.

---

# Limpieza

1. No enviar ni publicar las comunicaciones.
2. Conservar el documento en `Entregables`.

---

# Resumen

Durante esta práctica se realizó:

- Transformación de información técnica en mensajes por público.
- Revisión de contenido sensible.

Como resultado se obtuvo:

- Dos comunicaciones coherentes en hechos y adaptadas en forma.

---

# Recursos Opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

---

[⬅ Anterior: Práctica 8](../../Capitulo03/Practica08/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 10 ➡](../../Capitulo03/Practica10/README.md)
