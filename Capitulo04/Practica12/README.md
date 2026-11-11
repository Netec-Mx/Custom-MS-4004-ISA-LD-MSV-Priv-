# Práctica 12. Diseñar un agente para dar seguimiento a una necesidad recurrente

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Comparar Copilot Chat, agentes de plantilla disponibles y un agente personalizado para una tarea recurrente.
- Definir propósito, datos de entrada, criterios, prioridades, formato y límites para el nuevo agente.
- Redactar el prompt de creación que se ejecutará en la práctica 13.

<img src="../../images/p12-objetivo.svg" alt="Mapa visual de la práctica 12" width="720"/>

## Duración aproximada:

- 10 minutos.

## Tabla de ayuda:

| Elemento | Valor |
|---|---|
| Escenario | Laura lidera seis personas y recibe cada semana informes de cinco iniciativas |
| Criterios de revisión | Avance, desviaciones, riesgos, bloqueos, decisiones requeridas y próximos pasos |
| Prioridades | Retraso mayor a 10 días hábiles; bloqueo sin responsable; decisión que vence en siete días |
| Entregable de diseño | `Entregables/Diseno_Agente.docx` |

## Instrucciones

Laura necesita revisar semanalmente reportes con criterios consistentes. En la actualidad realiza solicitudes distintas a Copilot y obtiene respuestas de estructuras diferentes. Los informes contienen porcentajes, plazos, riesgos y decisiones, pero pueden llegar incompletos o con contradicciones.

### Tarea 1. Seleccionar la alternativa para la necesidad (3 min)

**Paso 1.** Comparar tres opciones para la revisión semanal: Copilot Chat (peticiones independientes), un agente de plantilla (objetivos predeterminados) y uno personalizado (mismos criterios y estructura en cada ejecución).

**Paso 2.** Crear un documento de Word en blanco y guardarlo como `Diseno_Agente.docx` en `Laboratorio_Copilot_ISA/Entregables`. Anotar en una frase por qué la recurrencia y los seis criterios justifican el agente personalizado.

### Tarea 2. Definir instrucciones y límites (4 min)

**Paso 1.** Especificar en el documento **propósito** (revisar informes), **entrada** (texto del reporte), **criterios** (seis), **salida** (tabla con hallazgo y evidencia) y **prioridades** (tres umbrales del escenario).

**Paso 2.** Escribir la conducta para datos faltantes (indicar lo que falta, solicitar aclaración y no inventar) y contradicciones (mostrar ambas afirmaciones y no declarar una verdadera sin evidencia). Limitarlo al seguimiento de iniciativas y prohibir tomar decisiones en nombre de Laura.

### Tarea 3. Construir el prompt del agente (3 min)

**Paso 1.** Copiar en Word el siguiente prompt de referencia; revisarlo para confirmar que incluye todas las reglas definidas.

**Prompt 1 - Crear el Revisor de Avance de Iniciativas**

```text
Crea un agente llamado Revisor de Avance de Iniciativas para analizar semanalmente reportes de las
iniciativas de mi equipo. Para cada reporte revisa seis criterios: avance real frente al planeado,
desviaciones de plazo/costo/alcance, riesgos, bloqueos, decisiones requeridas y próximos pasos.
Responde con una tabla de columnas criterio, hallazgo, evidencia textual y estado de verificación;
termina con una síntesis breve. Marca PRIORITARIO cuando un retraso supere 10 días hábiles,
exista un bloqueo sin responsable o una decisión deba tomarse en los siguientes siete días.
No inventes fechas, cifras, responsables o resultados. Cuando falten datos, solicita la aclaración
necesaria; si hay contradicciones, identifica los fragmentos en conflicto y suspende esa conclusión.
No tomes decisiones por la persona usuaria. Para solicitudes ajenas al seguimiento de iniciativas,
explica tu finalidad y pide un informe de avance pertinente.
```

**Paso 2.** Verificar que el prompt distingue el comportamiento del agente de las decisiones humanas, guardar el documento y conservarlo para la práctica 13.

### Resultado esperado

<img src="../../images/p12-resultado.svg" alt="Resultado esperado de la práctica 12" width="720"/>


Queda preparado un prompt de creación completo con propósito, seis criterios, estructura de respuesta, prioridades y restricciones frente a datos ausentes, contradicciones y solicitudes fuera del alcance. El archivo `Diseno_Agente.docx` se reutiliza directamente para crear el agente.
