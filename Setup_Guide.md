# Setup Guide — Productividad avanzada con IA y agentes

Preparación del entorno para **Custom MS-4004 ISA LD MSV (Priv)**. Comprende cuatro capítulos y catorce prácticas con duración total de cuatro horas. [Volver al inicio](README.md).

## 1. Entorno y herramientas necesarias

Utilizar una cuenta de trabajo o educativa con Microsoft 365 Copilot, acceso autorizado a Teams, Outlook, OneDrive o SharePoint, Word, Excel, PowerPoint y Loop. El usuario debe tener habilitados **Investigador (Researcher)** y **Analista (Analyst)**, la creación de agentes personales desde Microsoft 365 Copilot y los siete agentes definidos en el temario. **No se requiere Copilot Studio**.

Se recomienda un equipo con 8 GB de RAM, navegador actualizado, conexión estable y capacidad de trabajar en dos ventanas. La aplicación de Microsoft 365 Copilot está disponible mediante [Microsoft 365](https://www.microsoft365.com/) con la cuenta autorizada.

> **Importante:** los materiales representan un caso de capacitación y no son información operativa ni comunicaciones oficiales de ISA INTERCOLOMBIA. Utilizar un espacio de prueba autorizado y no publicar mensajes ni decisiones como si hubieran sido emitidos por la organización.

## 2. Licencias, agentes y comprobación de acceso

1. Confirmar la asignación de Microsoft 365 Copilot y las aplicaciones de Microsoft 365. El temario utiliza el término *Copilot Premium* para referirse al acceso a las capacidades avanzadas del curso.
2. Abrir Copilot y verificar que Investigador, Analista y la opción **Nuevo agente / Crear agente** aparecen disponibles.
3. Verificar el acceso de cada participante a los siguientes agentes creados a partir de las plantillas admitidas por la organización:

| Agente del curso | Plantilla de referencia | Práctica |
|---|---|---|
| Entrenador de ideas | Idea Coach | 3 |
| Agente de actualización de estado | Status Update Agent | 6 |
| Project Delta Digest | Project Delta Digest | 7 |
| Resumen personal de noticias | Personal News Digest | 8 |
| Diseñador de comunicaciones | Corporate Communications Crafter | 9 |
| Agente de informe ejecutivo | Executive Briefing Agent | 10 |
| Prompt Coach | Prompt Coach | 11 |

Las plantillas **no sustituyen** a los agentes ya creados: deben estar configurados y compartidos previamente, con sus fuentes de conocimiento autorizadas. Verificar que los resultados muestran citas o referencias cuando corresponde. Las fuentes de SharePoint y los correos siguen sujetos a permisos e indexación.

## 3. Preparar los recursos en OneDrive

1. Descargar el ZIP y extraerlo manteniendo `Capitulo01` a `Capitulo04`.
2. En OneDrive, crear `Laboratorio_Copilot_ISA`, una subcarpeta `Entregables` y las carpetas `Practica01` a `Practica14`.
3. Cargar a cada carpeta los archivos Word y Excel encontrados en el directorio `recursos/` de la práctica correspondiente. **Los archivos `.eml` se importan a Outlook y `.ics` al calendario; no se limitan a cargarlos en OneDrive**.
4. Abrir los Word y Excel desde OneDrive, revisar que el contenido sea legible y permitir que Copilot los utilice cuando la aplicación ofrezca la selección o adjunto de archivos.
5. Confirmar que la cuenta del participante puede acceder a los documentos y editarlos. Guardar los entregables en `Entregables` para conservar intactos los insumos.

## 4. Importar los correos electrónicos (.eml) a Outlook

Los recursos de las prácticas 4 y 8 se entregan como archivos MIME UTF-8 que pueden abrirse e **importarse** en el nuevo Outlook para Windows. El procedimiento de importación masiva documentado por Microsoft es:

1. Copiar los tres correos `.eml` de `Capitulo02/Practica04/recursos/` a una carpeta local denominada `Correos_INT-MDV` **sin subcarpetas**.
2. Abrir el **nuevo Outlook para Windows** con la cuenta de prácticas.
3. Ir a **Configuración > Archivos > Importar**, iniciar la importación y seleccionar `Correos_INT-MDV`, la cuenta y la carpeta de correo de destino. Repetir para los seis mensajes `.eml` de `Capitulo03/Practica08/recursos/`, almacenados juntos en otra carpeta local sin subcarpetas.
4. Comprobar en Outlook los asuntos `INT-MDV` y las seis noticias del periodo 2–6 de noviembre de 2026. Los remitentes utilizan el dominio reservado `laboratorio.example.org` para no representar cuentas empresariales reales.
5. Si el nuevo Outlook no dispone de importación masiva, abrir cada `.eml` arrastrándolo al panel de lectura. **Abrir un mensaje no equivale a importarlo al buzón ni garantiza que Copilot pueda recuperarlo**. Antes del taller debe validarse el método admitido por el inquilino.

**Documentación:** [Importación masiva de `.eml` en el nuevo Outlook](https://support.microsoft.com/es-es/outlook/bulk-import-eml-files-in-new-outlook) y [abrir `.eml` en Outlook](https://support.microsoft.com/es-es/outlook/mail/open-eml-msg-and-oft-files-in-new-outlook-and-outlook-on-the-web).

## 5. Importar la convocatoria (.ics) y preparar Teams

1. Abrir Outlook en la Web con la cuenta autorizada y seleccionar **Calendario > Agregar calendario > Cargar desde archivo**.
2. Importar `Capitulo02/Practica04/recursos/Reunion_Preparacion_INT-MDV.ics` en el calendario elegido. Confirmar el asunto **Revisión de preparación INT-MDV-2026**, con fecha **19 de noviembre de 2026, de 14:00 a 14:45 (hora de Bogotá)**.
3. Abrir el evento y, con una cuenta con permisos de organizador, habilitar la opción de **reunión de Teams**, agregar participantes reales del entorno de formación y compartir el `Plan_Intervencion_Mirador_del_Valle.docx` desde OneDrive. El archivo `.ics` no crea por sí mismo un vínculo de Teams ni invita a usuarios reales.
4. Antes de la sesión, comprobar en Teams la invitación, los tres correos `INT-MDV`, el plan y la matriz de riesgos. Verificar que la persona organizadora dispone de la opción de **Facilitator**; no iniciarla como parte de la práctica de preparación.

**Documentación:** [Importar calendarios `.ics` en Outlook](https://support.microsoft.com/es-es/outlook/import-or-subscribe-to-a-calendar-in-outlook-com-or-outlook-on-the-web).

## 6. Preparar el material de reuniones para Loop y Project Delta Digest

**Práctica 5.** El documento [Actas_Reuniones_INT-MDV.docx](Capitulo02/Practica05/recursos/Actas_Reuniones_INT-MDV.docx) reúne una transcripción y las notas de las reuniones del 20 y 27 de octubre y 3 de noviembre. Antes del taller, preparar **dos páginas de Loop** con el contenido de las reuniones B y C, denominadas `Notas INT-MDV 27-oct` y `Notas INT-MDV 03-nov`, y compartirlas con los participantes. Mantener el documento completo accesible en OneDrive para el registro del 20 de octubre.

Estas páginas se preparan a partir de texto; **no se presentan como resultados generados por Facilitator**. Para demostrar Facilitator de forma real, habilitarlo en una reunión de Teams, revisar las políticas de grabación y transcripción de la organización y utilizar las notas que produzca durante esa reunión.

**Práctica 7.** Compartir desde SharePoint o OneDrive `Evolucion_INT-MDV_Semanas44_45.docx` y `Registro_Decisiones_INT-MDV.xlsx`, comprobar acceso del usuario y enlazar la fuente de SharePoint con Project Delta Digest si su configuración lo necesita. El agente debe distinguir hechos confirmados, pendientes e información incompleta.

## 7. Preparar la actividad y las fuentes del resto del curso

- **Prácticas 1 a 3:** abrir los Word y Excel de los recursos y comprobar la selección de archivos en Investigador, Analista y Entrenador de ideas.
- **Práctica 6:** el agente de actualización de estado utiliza señales realmente accesibles desde la cuenta en Outlook, Teams y OneDrive. El documento de OKR aporta criterios de evaluación, pero no sustituye la actividad observable. Dejar disponible material de la semana de trabajo del participante.
- **Práctica 8:** la plantilla de resumen de noticias puede consultar fuentes autorizadas de Outlook, Teams y SharePoint. La búsqueda del periodo 2–6 de noviembre funciona como referencia estable para los correos proporcionados; si la capacitación se realiza después, no depender del filtro «últimos siete días» para recuperar esos mensajes.
- **Prácticas 9 y 10:** mantener accesibles las fichas técnicas y permitir al agente consultar fuentes públicas donde lo requiera el temario. Las comunicaciones externas son borradores sujetos a aprobación.
- **Prácticas 11 a 13:** las fuentes de la práctica 11 se reutilizan desde los capítulos anteriores. En la práctica 12 se redacta el prompt y en la práctica 13 se crea el agente mediante lenguaje natural; no se requieren archivos administrativos nuevos.
- **Práctica 14:** comprobar que `Caso_Monitoreo_Predictivo_Activos.docx` y `Datos_Activos_MPA.xlsx` abren en Word y Excel con Copilot disponible. Abrir PowerPoint para garantizar que puede crearse una presentación en la carpeta de entregables.

## 8. Validaciones previas y límites de ejecución

- Probar importación real de un `.eml` y un `.ics` en el entorno previsto, con texto acentuado correcto (por ejemplo, «intervención», «Gestión Ambiental» y «reprogramación»).
- Confirmar acceso y permisos de los siete agentes, Investigador, Analista y opciones de Agent Builder y Facilitator.
- Verificar que las dos páginas de Loop y las fuentes de SharePoint son visibles a la cuenta que ejecutará las prácticas.
- En Copilot, comprobar que una respuesta cita realmente la fuente. Una respuesta genérica no valida que el recurso se haya recuperado desde Microsoft 365.
- Evitar información real confidencial, direcciones de correo personales y publicación automática de borradores. Respetar los controles de seguridad e identidad de la organización.
- La duración oficial de cada práctica supone materiales y agentes **preparados antes** de la sesión. La indexación y las investigaciones pueden variar en tiempo; las 4 horas no incluyen la configuración inicial del inquilino.

## 9. Documentación técnica oficial

- [Plantillas de agentes de Microsoft 365 Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-templates-overview)
- [Crear un agente mediante lenguaje natural](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-build-agents)
- [Personal News Digest](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-template-personal-news-digest)
- [Project Delta Digest](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-template-project-delta-digest)
- [Facilitator en reuniones de Teams](https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings)
