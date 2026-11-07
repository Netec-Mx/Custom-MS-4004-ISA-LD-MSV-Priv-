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

**Paso 1.** En la aplicación Microsoft 365 Copilot, abrir **Agentes** y seleccionar **Diseñador de comunicaciones**.

**Paso 2.** Escribir, referenciando la ficha con `/`:

```text
Con base en /Ficha_Tecnica_Intervencion, redacta un correo interno para colaboradores sobre la intervención.
Explica en lenguaje claro el propósito, el periodo, las posibles afectaciones y, sobre todo, qué acciones deben realizar.
Máximo 200 palabras.
```

**Paso 3.** Verificar que el mensaje incluya las tres acciones requeridas: no programar trabajos en la subestación, confirmar turnos y canalizar consultas externas a Comunicaciones.

**Al terminar esta tarea debes tener:**

- ✔ El correo con propósito, periodo, afectaciones y las 3 acciones.

---

## Tarea 2. Adaptar el mensaje a un público externo y otro canal (5 min)

**Objetivo:** Tener una publicación externa de máximo 100 palabras y una tabla que compare ambas versiones.

**Por qué:** El mismo hecho se comunica distinto a la comunidad: sin tecnicismos ni datos internos, pero con los mismos hechos.

**Paso 1.** Escribir:

```text
Adapta el mismo acontecimiento para la comunidad y los usuarios externos, en una publicación breve para el sitio web
(máximo 100 palabras). Sin tecnicismos ni datos de operación interna. Mantén fecha, propósito y afectaciones.
```

**Paso 2.** Pedir una tabla que compare ambas versiones en lenguaje, extensión, tono y nivel de detalle.

**Paso 3.** Comprobar que fecha, propósito y afectaciones sean iguales en ambas versiones.

**Al terminar esta tarea debes tener:**

- ✔ La publicación externa.
- ✔ La tabla comparativa.
- ✔ Fecha, propósito y afectaciones iguales en ambas versiones.

---

## Tarea 3. Identificar contenido a proteger o revisar (5 min)

**Objetivo:** Tener la lista de contenido a proteger o revisar con su aprobador, y ambas comunicaciones guardadas sin enviar.

**Por qué:** Publicar un costo interno o una duración no aprobada genera problemas legales y de reputación.

**Paso 1.** Escribir, referenciando la nota con `/`:

```text
Incorpora /Nota_Interna_Datos_Sensibles al análisis. ¿Qué contenido debería protegerse, modificarse o someterse a revisión
antes de publicar cada comunicación? Justifica cada punto e indica quién debería aprobarlo.
```

**Paso 2.** Verificar que se protejan el **costo**, los **nombres de clientes** y la **compensación**, y que la **extensión a 48 h** no se publique por no estar aprobada.

**Paso 3.** Abrir Word (escritorio o web) y crear un **Documento en blanco**. En Copilot, seleccionar **Copiar** debajo de cada comunicación y de la revisión y pegar en Word con **Ctrl+V**. Seleccionar **Archivo > Guardar como**, elegir **OneDrive > Laboratorio_Copilot_ISA > Entregables** y guardar con el nombre `Comunicaciones_INT-MDV_[INICIALES].docx`. No enviar ni publicar.

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
