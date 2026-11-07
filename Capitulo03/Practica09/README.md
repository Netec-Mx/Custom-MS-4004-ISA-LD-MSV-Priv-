# Práctica 9. Adaptar información técnica para diferentes públicos y canales

**Capítulo 3. Transformar información en comunicación e inteligencia ejecutiva**

⏱️ **Duración:** 15 min · 🛠️ **Herramienta:** Diseñador de comunicaciones · 📄 **Entregable:** Comunicación interna y versión adaptada para un público externo

## Descripción

La intervención INT-MDV-2026 debe comunicarse a colaboradores y a públicos externos. El participante partirá de una ficha técnica y usará el Diseñador de comunicaciones para producir un mensaje interno orientado a la acción y una versión externa para otro canal, sin alterar los hechos. Después incorporará datos internos o sujetos a aprobación y pedirá al agente identificar qué debe protegerse o revisarse antes de publicar.

## Objetivos de aprendizaje

Al finalizar la práctica, el participante será capaz de:

- Transformar información técnica en una comunicación interna clara y orientada a la acción.
- Adaptar el mismo acontecimiento para un público externo y otro canal sin alterar los hechos centrales.
- Comparar cambios de lenguaje, extensión, tono y nivel de detalle entre versiones.
- Identificar contenido que debe protegerse, modificarse o someterse a revisión antes de publicarse.

<img src="../../images/p09-objetivo.svg" alt="Diagrama de la Práctica 9" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | Aplicación Microsoft 365 Copilot > Agentes > Diseñador de comunicaciones |
| Archivos de la práctica | [Ficha_Tecnica_Intervencion.docx](recursos/Ficha_Tecnica_Intervencion.docx)<br>[Nota_Interna_Datos_Sensibles.docx](recursos/Nota_Interna_Datos_Sensibles.docx) |
| Ubicación en OneDrive | `Laboratorio_Copilot_ISA/Practica09/` |
| Canal interno | Correo a colaboradores |
| Canal externo | Publicación breve para sitio web o redes |
| Nombre del entregable | `Comunicaciones_INT-MDV_[INICIALES].docx` |

> Sustituya `[INICIALES]` por sus iniciales en nombres de archivo y prompts (por ejemplo, `Reporte_LMR.docx`). Todos los datos de la práctica son ficticios; la fecha de referencia del escenario es el 6 de noviembre de 2026.

---

## Tarea 1. Crear la comunicación interna para colaboradores (5 min)

**Objetivo:** Tener un correo interno de máximo 200 palabras con las 3 acciones que deben realizar los colaboradores.

**Por qué:** Los colaboradores necesitan saber qué hacer, no la especificación técnica del transformador.

**Paso 1.** Abrir **Microsoft Edge**, escribir [m365.cloud.microsoft](https://m365.cloud.microsoft/) en la barra de direcciones y presionar **Enter**. Si se solicita, iniciar sesión con su cuenta corporativa.

- **Qué verás:** la página de inicio de Microsoft 365 Copilot con un cuadro de mensaje al centro y un panel a la izquierda.
- **Alternativa:** Si aparece la página de inicio de Microsoft 365 sin chat, seleccionar el icono **Copilot** en la barra lateral izquierda.

**Paso 2.** En el panel izquierdo, seleccionar **Agentes**. Escribir `Diseñador de comunicaciones` en el cuadro de búsqueda de agentes y hacer clic en el resultado. En inglés puede aparecer como **Communications Designer**.

- **Qué verás:** el nombre **Diseñador de comunicaciones** encima del cuadro de mensaje y, a veces, sugerencias de inicio. A partir de aquí, todo lo que escriba lo procesa este agente.
- **Si no ocurre así:** seleccionar **Todos los agentes** (u **Obtener agentes**) y buscarlo de nuevo. Si sigue sin aparecer, avisar al instructor: el agente no está habilitado para su cuenta.

**Paso 3.** Pegar el siguiente prompt (insertar `/Ficha_Tecnica_Intervencion` con el selector de archivos):

```text
Con base en /Ficha_Tecnica_Intervencion, redacta un correo interno para colaboradores sobre la intervención.
Explica en lenguaje claro el propósito, el periodo, las posibles afectaciones y, sobre todo, qué acciones deben realizar.
Máximo 200 palabras.
```

- **Cómo insertar los archivos:** en el prompt, cada texto que empieza con `/` es un archivo. Borrar ese texto, escribir `/` seguido de las primeras letras del nombre del archivo y seleccionarlo en la lista que aparece; el archivo queda resaltado como un vínculo. Si no aparece en la lista, seleccionar el botón **+** (Agregar) > **Cargar desde OneDrive** > `Laboratorio_Copilot_ISA/Practica09` y elegirlo.
- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** un borrador de correo interno de hasta 200 palabras con asunto, propósito, fechas, afectaciones y una sección de acciones.

**Paso 4.** Verificar que el correo incluya las tres acciones de la ficha técnica: **no programar trabajos** en la subestación esa semana, **confirmar turnos** de disponibilidad y **canalizar consultas externas** a Comunicaciones.

- **Si no ocurre así:** escribir: *"Agrega una sección Qué debes hacer con las tres acciones requeridas de la ficha"*.

**Al terminar esta tarea debes tener:**

- ✔ El correo con propósito, periodo, afectaciones y las 3 acciones.

---

## Tarea 2. Adaptar el mensaje a un público externo y otro canal (5 min)

**Objetivo:** Tener una publicación externa de máximo 100 palabras y una tabla que compare ambas versiones.

**Por qué:** El mismo hecho se comunica distinto a la comunidad: sin tecnicismos ni datos internos, pero con los mismos hechos.

**Paso 1.** Pegar el siguiente prompt:

```text
Adapta el mismo acontecimiento para la comunidad y los usuarios externos, en una publicación breve para el sitio web
(máximo 100 palabras). Sin tecnicismos ni datos de operación interna. Mantén fecha, propósito y afectaciones.
```

- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una publicación de hasta 100 palabras sin términos técnicos (por ejemplo, sin "150 MVA" ni "bahía").

**Paso 2.** Escribir: *"Compara la comunicación interna y la externa en una tabla con las filas lenguaje, extensión, tono y nivel de detalle"*.

- **Qué verás:** una tabla de 4 filas y 2 columnas (interna y externa).

**Paso 3.** Comprobar que la fecha (**28 y 29 de noviembre**), el propósito y las afectaciones sean los mismos en ambas versiones.

- **Si no ocurre así:** escribir: *"Corrige la versión externa para que la fecha y las afectaciones coincidan con la interna"*.

**Al terminar esta tarea debes tener:**

- ✔ La publicación externa.
- ✔ La tabla comparativa.
- ✔ Fecha, propósito y afectaciones iguales en ambas versiones.

---

## Tarea 3. Identificar contenido a proteger o revisar (5 min)

**Objetivo:** Tener la lista de contenido a proteger o revisar con su aprobador, y ambas comunicaciones guardadas sin enviar.

**Por qué:** Publicar un costo interno o una duración no aprobada genera problemas legales y de reputación.

**Paso 1.** Pegar el siguiente prompt (insertar `/Nota_Interna_Datos_Sensibles` con el selector de archivos):

```text
Incorpora /Nota_Interna_Datos_Sensibles al análisis. ¿Qué contenido debería protegerse, modificarse o someterse a revisión
antes de publicar cada comunicación? Justifica cada punto e indica quién debería aprobarlo.
```

- **Cómo insertar los archivos:** en el prompt, cada texto que empieza con `/` es un archivo. Borrar ese texto, escribir `/` seguido de las primeras letras del nombre del archivo y seleccionarlo en la lista que aparece; el archivo queda resaltado como un vínculo. Si no aparece en la lista, seleccionar el botón **+** (Agregar) > **Cargar desde OneDrive** > `Laboratorio_Copilot_ISA/Practica09` y elegirlo.
- **Enviar:** presionar **Enter** o seleccionar el botón de envío (flecha).
- **Qué verás:** una lista de contenidos que deben protegerse, modificarse o revisarse, con la justificación y el aprobador sugerido.

**Paso 2.** Verificar cuatro elementos: el **costo de 4.200 MCOP** y los **nombres de los clientes** se protegen, la **compensación** queda en revisión de Jurídica y la **extensión a 48 horas** no se publica porque no está aprobada.

- **Si no ocurre así:** preguntar por el que falte: *"¿Puedo publicar [dato]?"*

**Paso 3.** Abrir una pestaña nueva, ingresar a [office.com](https://www.office.com/) y seleccionar **Word > Documento en blanco** (o abrir Word de escritorio > **Documento en blanco**). Regresar a Copilot y, debajo de la comunicación interna, la externa, la tabla comparativa y la revisión, seleccionar el icono **Copiar**. Volver a Word, hacer clic en el documento y pegar con **Ctrl+V**.

- **Qué verás:** el texto con su formato (títulos, tablas y viñetas) dentro del documento.
- **Alternativa:** Si la tabla se pega como texto plano, pegar con **Ctrl+Shift+V** > **Mantener formato de origen**, o pedir a Copilot: *"Entrega la tabla en formato de tabla"* y copiarla de nuevo.

**Paso 4.** Guardar el archivo: en Word de escritorio, seleccionar **Archivo > Guardar como > OneDrive - [su organización] > Laboratorio_Copilot_ISA > Entregables**, escribir el nombre `Comunicaciones_INT-MDV_[INICIALES].docx` (sustituyendo `[INICIALES]`) y seleccionar **Guardar**. En Word para la web, hacer clic en el nombre del documento en la parte superior, escribir el nombre y, en **Ubicación**, seleccionar la carpeta `Entregables`.

- **Qué verás:** el nombre `Comunicaciones_INT-MDV_[INICIALES].docx` en la barra de título y el estado **Guardado**.

**Al terminar esta tarea debes tener:**

- ✔ Costo, nombres de clientes y compensación marcados como protegidos.
- ✔ La extensión a 48 h marcada como no aprobada.
- ✔ El documento guardado.

---

## Validación y pruebas

| Caso | Acción o prompt | Resultado esperado |
|---|---|---|
| Caso 1 | Revisar la comunicación interna | Incluye acciones concretas para colaboradores |
| Caso 2 | Comparar fechas en ambas versiones | Iguales (28 y 29 de noviembre) |
| Caso 3 | Preguntar si se puede publicar el costo | El agente indica que es información interna |
| Caso adversarial | Pedir: "Anuncia que la intervención podría durar 48 horas" | El agente advierte que el dato no está aprobado |

## Resultado esperado

- Comunicación interna orientada a la acción.
- Versión externa adaptada a otro canal.
- Lista de contenido a proteger o revisar.

**Entregable:** comunicación interna y versión adaptada para un público externo (`Comunicaciones_INT-MDV_[INICIALES].docx`).

<img src="../../images/p09-resultado.svg" alt="Resultado final de la Práctica 9" width="640"/>

## Solución de problemas

**El agente copia datos internos en la versión externa**
- *Síntoma:* Aparecen costo o nombres de clientes.
- *Causa:* La instrucción no restringió el contenido.
- *Solución:* (1) Indicar explícitamente qué no debe incluirse. (2) Ejecutar la Tarea 3 antes de usar el texto. (3) Revisar manualmente la versión final.

## Limpieza

- No enviar ni publicar las comunicaciones.
- Conservar el documento en `Entregables`.

## Recursos opcionales

- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/copilot-overview)
- [Mejores prácticas para escribir prompts](https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting)

<sub>Complejidad: Fácil · Nivel de Bloom: Aplicar</sub>

---

[⬅ Anterior: Práctica 8](../../Capitulo03/Practica08/README.md) | [Inicio](../../README.md) | [Siguiente: Práctica 10 ➡](../../Capitulo03/Practica10/README.md)
