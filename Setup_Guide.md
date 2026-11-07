# Setup Guide General

## Productividad avanzada con IA y agentes

| Control documental | Información |
|---|---|
| Clave del curso | Custom MS-4004 ISA LD MSV (Priv) |
| Versión del documento | 1.0 |
| Estado | BORRADOR: revisión documental completa; pendiente de validación funcional en el tenant de ISA INTERCOLOMBIA |
| Instructor responsable | Por asignar por Netec |
| Fecha de elaboración | 2026-11-06 |
| Fecha de última validación | 2026-11-06 (revisión del repositorio) |
| Repositorio de laboratorios | Se registra al publicar en GitHub |
| Rama y revisión analizada | `main`, versión inicial 1.0 |
| Alcance revisado | 4 capítulos, 14 prácticas, 32 archivos de recursos, 29 imágenes, README principal y Setup Guide |
| Modalidad del entorno | Cloud (servicios SaaS de Microsoft 365) con aplicaciones de escritorio de Microsoft 365 |

[Inicio](README.md)

# Objetivo

Preparar, para cada participante, un entorno de Microsoft 365 con licencia de Microsoft 365 Copilot Premium; acceso a Investigador, Analista, Facilitator y a los agentes Project Delta Digest, Agente de actualización de estado, Resumen personal de noticias, Agente de informe ejecutivo, Prompt Coach, Diseñador de comunicaciones y Entrenador de ideas; permiso para crear agentes personalizados; y los datos ficticios del curso cargados en OneDrive, SharePoint, Outlook, Teams y Loop. El entorno está listo cuando las validaciones obligatorias de la sección [Validación del Entorno](#validacion-entorno) se aprueban con una cuenta equivalente a la de un participante.

# Requisitos de Hardware

| Recurso | Mínimo requerido | Recomendado | Observaciones |
|---|---|---|---|
| Procesador y arquitectura | 64 bits, 2 núcleos, 1.6 GHz | 4 núcleos o más | Requisito de Microsoft 365 Apps |
| Memoria RAM | 8 GB | 16 GB | Varias aplicaciones y pestañas abiertas (la Práctica 14 usa cinco herramientas) |
| Espacio libre | 4 GB | 10 GB | Microsoft 365 Apps, Teams y OneDrive; los recursos ocupan menos de 1 MB |
| Pantalla | 1366 x 768 | 1920 x 1080 o dos monitores | Un monitor para instrucciones y otro para Copilot |
| Conectividad | 10 Mbps por participante | 25 Mbps por participante | Conexión permanente a Microsoft 365 |

# Sistemas Operativos Compatibles

| Sistema operativo | Edición y versión | Arquitectura | Condición de soporte o validación |
|---|---|---|---|
| Windows 11 | Pro o Enterprise, 23H2 o posterior | x64 | Plataforma base del curso. Compatible según fabricante; pendiente de validar en el tenant |
| macOS | 14 Sonoma o posterior | Apple silicon o Intel | Compatible según fabricante; no validado para este curso |

La plataforma base es Windows 11 con Microsoft Edge. En macOS los nombres de menú de las aplicaciones de escritorio pueden variar.

# Software Requerido

| Componente | Edición y versión requerida | Arquitectura | Obligatorio u opcional | Fuente oficial |
|---|---|---|---|---|
| Microsoft Edge | Versión estable vigente | x64 | Obligatorio (o Google Chrome vigente) | [microsoft.com/edge](https://www.microsoft.com/es-es/edge) |
| Aplicación Microsoft 365 Copilot (web) | Servicio administrado | N/A | Obligatorio | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Microsoft 365 Apps (Word, Excel, PowerPoint, Outlook) | Canal Actual o Canal mensual para empresas, con Copilot | x64 | Obligatorio | [Requisitos de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/plan/microsoft-copilot-requirements) |
| Microsoft Teams | Nuevo Teams de escritorio o Teams web | x64 | Obligatorio (prácticas 4 y 5) | [teams.microsoft.com](https://teams.microsoft.com/) |
| OneDrive para el trabajo o la escuela | Cliente de sincronización vigente | x64 | Obligatorio (web) / opcional (cliente) | Incluido en Microsoft 365 |
| Microsoft Loop | Servicio administrado | N/A | Obligatorio (Práctica 5) | Incluido en Microsoft 365 |

Los servicios de Microsoft 365 son administrados y no tienen versión fijable. Registre en el [Registro de validación](#registro-validacion) la fecha de prueba y el nombre con que aparece cada agente en el tenant.

# Herramientas y Dependencias

## Paquetes, frameworks y componentes adicionales

| Dependencia | Versión o restricción | Componente que la necesita | Método de instalación o habilitación |
|---|---|---|---|
| Investigador (Researcher) | Servicio administrado | Prácticas 1 y 14 | Incluido con la licencia; verificar en **Agentes** |
| Analista (Analyst) | Servicio administrado | Prácticas 2 y 14 | Incluido con la licencia; verificar en **Agentes** |
| Entrenador de ideas | Servicio administrado | Práctica 3 | Centro de administración > Agentes; asignar al grupo del curso |
| Facilitator | Servicio administrado | Prácticas 4 y 5 | Directiva de reuniones de Teams con transcripción habilitada ([documentación](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams)) |
| Galería de indicaciones | Servicio administrado | Prácticas 5 y 11 | Disponible en [m365.cloud.microsoft/copilot-prompts](https://m365.cloud.microsoft/copilot-prompts) |
| Agente de actualización de estado | Servicio administrado | Práctica 6 | Centro de administración > Agentes; asignar al grupo del curso |
| Project Delta Digest | Servicio administrado | Práctica 7 | Centro de administración > Agentes; asignar al grupo del curso |
| Resumen personal de noticias | Servicio administrado | Práctica 8 | Centro de administración > Agentes; asignar al grupo del curso |
| Diseñador de comunicaciones | Servicio administrado | Práctica 9 | Centro de administración > Agentes; asignar al grupo del curso |
| Agente de informe ejecutivo | Servicio administrado | Práctica 10 | Centro de administración > Agentes; asignar al grupo del curso |
| Prompt Coach | Servicio administrado | Práctica 11 | Centro de administración > Agentes; asignar al grupo del curso |
| Agent Builder | Servicio administrado | Prácticas 12 y 13 | Permitir la creación de agentes al grupo del curso ([documentación](https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder)) |
| Copilot en Word, Excel, PowerPoint y Outlook | Microsoft 365 Apps con Copilot | Varias prácticas | Incluido con la licencia |
| Materiales ficticios | Versión 1.0 de este repositorio | Prácticas 1 a 14 | Subcarpetas `CapituloNN/PracticaNN/recursos/` |

Los nombres de los agentes en español corresponden al temario; en el tenant pueden aparecer en inglés. La disponibilidad depende de la región, del programa de lanzamiento y de la configuración del tenant, por lo que debe confirmarse con la validación V-03.

## Licencias, cuentas y permisos

| Recurso o servicio | Licencia o suscripción | Cuenta o rol requerido | Permiso mínimo | Responsable de habilitación |
|---|---|---|---|---|
| Microsoft 365 | Microsoft 365 E3/E5 o Business Standard/Premium | Cuenta corporativa del participante | Usuario | Administrador de TI de ISA INTERCOLOMBIA |
| Microsoft 365 Copilot | Licencia de Microsoft 365 Copilot (el temario la denomina "Premium") | Cuenta del participante | Licencia asignada | Administrador de licencias |
| Agentes del curso | Incluidos o habilitados según el tenant | Grupo de seguridad `Curso-Copilot-Avanzado` | Agentes asignados al grupo | Administrador de IA o global |
| Agent Builder | Licencia de Microsoft 365 Copilot | Grupo del curso | Creación de agentes permitida | Administrador de IA o global |
| Reuniones con Facilitator | Licencia de Microsoft 365 Copilot | Participante como coorganizador | Transcripción y Copilot permitidos | Administrador de Teams |
| Sitio `INT-MDV (Laboratorio)` | Incluido en Microsoft 365 | Participantes como miembros | Lectura | Administrador de SharePoint o instructor |
| Sitio de noticias de laboratorio | Incluido en Microsoft 365 | Participantes como visitantes | Lectura | Administrador de SharePoint o instructor |
| Cuentas de laboratorio para sembrar datos | Microsoft 365 con buzón | 4 cuentas: Operación, Gestión Ambiental, Comercial y Dirección del área (nombres a criterio de TI) | Enviar correo y chatear | Administrador de TI |

Las credenciales se entregan por el canal autorizado por ISA INTERCOLOMBIA. No registre contraseñas, códigos MFA ni tokens en este repositorio ni en los entregables.

# Instalación y Configuración

## 1. Obtener los materiales

- Repositorio autorizado: este repositorio de GitHub (botón **Code > Download ZIP**).
- Revisión: rama `main`, versión 1.0.
- Directorio local: `C:\Cursos\MS-4004-ISA\` (Windows).
- Archivos de entrada: `Capitulo01/Practica01/recursos/` a `Capitulo04/Practica14/recursos/`.

Los archivos de `recursos` se distribuyen; los entregables los crean los participantes en `Laboratorio_Copilot_ISA/Entregables/`. Los archivos `Guion_*.docx` son solo para el instructor.

## 2. Instalar o habilitar los componentes

### Licencias y agentes (administrador)

1. Crear el grupo de seguridad `Curso-Copilot-Avanzado` con participantes e instructor.
2. Asignar la licencia de Microsoft 365 Copilot a sus miembros.
3. En el [Centro de administración de Microsoft 365](https://admin.microsoft.com/), abrir **Agentes**, localizar cada agente del curso y asignarlo al grupo ([documentación](https://learn.microsoft.com/es-es/microsoft-agent-365/admin/manage-copilot-agents-integrated-apps)).
4. Permitir la creación de agentes con Agent Builder para el grupo del curso.
5. Esperar la propagación (hasta 24 horas).

**Plataforma y terminal:** navegador web, Centro de administración de Microsoft 365.

**Resultado esperado:** con una cuenta de participante, **Agentes** muestra los agentes del curso y la opción **Crear agente**.

### Directiva de reuniones de Teams (administrador de Teams)

1. En el [Centro de administración de Teams](https://admin.teams.microsoft.com/), abrir **Reuniones > Directivas de reunión**.
2. En la directiva asignada a los participantes, habilitar la **Transcripción** y Copilot en reuniones.
3. Verificar que Facilitator esté permitido según la [documentación de Facilitator](https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams).

**Resultado esperado:** en **Opciones de reunión** se muestra la configuración de Copilot y Facilitator.

### Estructura de carpetas en OneDrive (cada participante)

**Plataforma y terminal:** Windows 11, PowerShell 5.1 o posterior, con el cliente de OneDrive iniciado con la cuenta corporativa.

```powershell
$repo = "C:\Cursos\MS-4004-ISA"
$dest = Join-Path $env:OneDriveCommercial "Laboratorio_Copilot_ISA"
New-Item -ItemType Directory -Force -Path (Join-Path $dest "Entregables") | Out-Null
1..14 | ForEach-Object {
    $n = $_
    $c = if ($n -le 3) { 1 } elseif ($n -le 7) { 2 } elseif ($n -le 11) { 3 } else { 4 }
    $prac = "Practica{0:D2}" -f $n
    $cap = "Capitulo{0:D2}" -f $c
    $target = Join-Path $dest $prac
    New-Item -ItemType Directory -Force -Path $target | Out-Null
    Get-ChildItem -LiteralPath (Join-Path $repo "$cap\$prac\recursos") -File |
        Where-Object { $_.Name -notlike "Guion_*" } |
        Copy-Item -Destination $target -Force
}
Get-ChildItem $dest -Recurse -File | Measure-Object | Select-Object Count
```

**Resultado esperado:** `Count` igual a **30** (32 recursos menos los 2 guiones del instructor) y, en OneDrive web, `Laboratorio_Copilot_ISA` con `Practica01` a `Practica14` y `Entregables`. Si `$env:OneDriveCommercial` está vacío, el cliente de OneDrive no ha iniciado sesión.

Sin cliente de sincronización: crear las carpetas en OneDrive web y cargar el contenido de cada `recursos` con **Cargar > Archivos**.

## 3. Preparar archivos de configuración

| Archivo | Ruta | Configuración necesaria | Origen |
|---|---|---|---|
| Recursos por práctica | `OneDrive/Laboratorio_Copilot_ISA/PracticaNN/` | Cargar sin cambiar nombres | Incluido en repositorio |
| Invitación y correos de la reunión | Calendario y buzón del participante | Crear según el guion | [Guion_Correos_Invitacion_Reunion.docx](Capitulo02/Practica04/recursos/Guion_Correos_Invitacion_Reunion.docx) |
| Páginas de Loop de Facilitator | Espacio de Loop del instructor, compartidas con participantes | Crear dos páginas con el contenido de las notas | [Notas del 27-oct](Capitulo02/Practica05/recursos/Notas_Facilitator_2026-10-27.docx) y [notas del 03-nov](Capitulo02/Practica05/recursos/Notas_Facilitator_2026-11-03.docx) |
| Actividad de la semana | Buzón y Teams del participante | Enviar los mensajes del guion durante la semana previa | [Guion_Actividad_Semanal.docx](Capitulo02/Practica06/recursos/Guion_Actividad_Semanal.docx) |

# Variables de Entorno

| Variable | Propósito | Valor o formato esperado | Alcance | Método de configuración |
|---|---|---|---|---|
| `OneDriveCommercial` | Ruta de la carpeta sincronizada usada por el script de preparación | `C:\Users\<usuario>\OneDrive - <Organización>` | Usuario | La define el cliente de OneDrive al iniciar sesión |

**Configuración — Windows 11, PowerShell:** no requiere configuración manual.

**Verificación sin exponer secretos:**

```powershell
Test-Path $env:OneDriveCommercial
```

Resultado esperado: `True`.

# Configuración Base para los Laboratorios

## Parámetros comunes

| Parámetro | Valor o convención | Observaciones |
|---|---|---|
| Raíz de trabajo | `OneDrive/Laboratorio_Copilot_ISA/` | Una por participante |
| Carpeta de entregables | `OneDrive/Laboratorio_Copilot_ISA/Entregables/` | La Práctica 13 usa el entregable de la 12 |
| Nomenclatura de entregables | `Nombre_[INICIALES].ext` | Ejemplo: `Reporte_Analitico_LMR.docx` |
| Fecha de referencia del escenario | 6 de noviembre de 2026 | Para atrasos y vencimientos |
| Proyecto común | `INT-MDV-2026` (Subestación Mirador del Valle, ficticia) | Prácticas 3, 4, 5, 7, 9 y 11 |
| Unidad monetaria | Millones de pesos colombianos (MCOP) | En todos los recursos |

## Estructura de carpetas

```text
OneDrive/
└── Laboratorio_Copilot_ISA/
    ├── Practica01/ ... Practica14/   Recursos de cada práctica
    └── Entregables/                  Archivos que crea el participante
```

## Recursos compartidos

| Recurso | Nombre o identificador | Estructura o configuración base | Responsable de creación |
|---|---|---|---|
| Reunión de Teams | `Revisión de preparación INT-MDV-2026` | Programada después del curso, con el cuerpo del guion, el plan adjunto y los participantes como coorganizadores | Instructor |
| Páginas de Loop | `Notas Facilitator INT-MDV 27-oct` y `Notas Facilitator INT-MDV 03-nov` | Contenido de los archivos de notas; compartidas en lectura | Instructor (rol "Coordinación de la intervención") |
| Sitio de SharePoint | `INT-MDV (Laboratorio)` | Biblioteca con plan, matriz de riesgos, informes semanas 44 y 45, registro de decisiones, notas y transcripción | Administrador de SharePoint o instructor |
| Sitio de noticias | `Noticias Laboratorio ISA` | Seis publicaciones de noticias con el contenido de `Practica08/recursos/` | Administrador de SharePoint o instructor |

<a id="preparacion-por-practica"></a>

## Preparación previa por práctica

Completar al menos **48 horas antes** del curso para que Copilot indexe correos, reuniones, chats y archivos.

| Práctica | Preparación requerida | Verificación |
|---|---|---|
| 1 | Cargar `Prioridades_Internas_2027.docx`; confirmar búsqueda web | Investigador responde con citas web |
| 2 | Cargar los dos archivos de Excel | Analista reporta 12 proyectos y 9 meses |
| 3 | Cargar la propuesta | Entrenador de ideas la resume |
| 4 | Crear la reunión con invitación y adjunto; enviar los 3 correos del guion; cargar plan y matriz | Copilot encuentra los correos con asunto `INT-MDV` |
| 5 | Crear las dos páginas de Loop y cargar la transcripción; compartirlas con los participantes | Copilot encuentra las páginas con `/` |
| 6 | Enviar la actividad del guion durante la semana previa; cargar los OKR | El agente lista actividad de la última semana |
| 7 | Crear el sitio `INT-MDV (Laboratorio)` y cargar sus archivos | Project Delta Digest encuentra el proyecto por su código |
| 8 | Publicar las seis noticias en el sitio de noticias | El agente menciona al menos una noticia interna |
| 9 | Cargar ficha técnica y nota interna | El Diseñador de comunicaciones lee la ficha |
| 10 | Cargar la ficha del evento; confirmar búsqueda web | El agente confirma el contexto del evento |
| 11 | Cargar la plantilla; verificar que los archivos de las prácticas 4 y 7 estén en OneDrive | Prompt Coach responde |
| 12 | Cargar escenario y plantilla | Archivos abren en Word |
| 13 | Cargar los tres reportes; confirmar Agent Builder | La opción **Crear agente** está disponible |
| 14 | Cargar caso y datos | Analista lee el Excel; Copilot disponible en Word, Excel y PowerPoint |

## Correcciones de coherencia

| Inconsistencia o dependencia omitida | Configuración unificada | Ajuste necesario en las copias de trabajo |
|---|---|---|
| La estructura de referencia muestra 11 capítulos; el temario define 4 módulos con 14 prácticas | Una carpeta por módulo (`Capitulo01` a `Capitulo04`) y una carpeta por práctica (`Practica01` a `Practica14`), cada una con su `README.md` | Ninguno |
| La Práctica 5 la conduce el instructor según el temario | El README describe los pasos del instructor; los participantes los replican si tienen acceso a las páginas de Loop | Compartir las páginas de Loop si se desea ejecución en paralelo |
| Las notas de Facilitator y la actividad de Microsoft 365 no pueden distribuirse en un repositorio | Se distribuye su contenido y un guion para sembrarlo | Preparación del instructor |
| El logotipo de la plantilla se llama `neteclogo (2).png` | Se renombró a `images/neteclogo.png` | Ninguno |
| El temario indica "Microsoft 365 Copilot Premium" | Se documenta como licencia de Microsoft 365 Copilot | Confirmar con ISA INTERCOLOMBIA el nombre comercial de la licencia |

# Servicios Externos Requeridos

| Servicio | URL, endpoint o región | Uso | Acceso requerido |
|---|---|---|---|
| Aplicación Microsoft 365 Copilot | [m365.cloud.microsoft](https://m365.cloud.microsoft/) | Chat, agentes y Agent Builder | Cuenta con licencia |
| Microsoft Teams | [teams.microsoft.com](https://teams.microsoft.com/) | Reunión y Facilitator | Cuenta corporativa |
| Outlook | [outlook.office.com](https://outlook.office.com/) | Correos sembrados | Cuenta con buzón |
| OneDrive y SharePoint | Tenant de ISA INTERCOLOMBIA | Recursos, sitios y entregables | Cuenta corporativa |
| Búsqueda web de Copilot | Servicio de Microsoft | Prácticas 1, 10 y 14 | Permitida por la organización |

## Configuración de red

| Origen | Destino | Protocolo y puerto | Sentido | Condición |
|---|---|---|---|---|
| Equipo del participante | Endpoints de Microsoft 365 | HTTPS 443 | Saliente | Según la [lista oficial de endpoints](https://learn.microsoft.com/es-es/microsoft-365/enterprise/microsoft-365-endpoints?view=o365-worldwide) |
| Equipo del participante | Endpoints de Microsoft 365 | WSS sobre 443 | Saliente | Respuestas en tiempo real de Copilot |

# Creación de Entornos / Máquinas Virtuales / Emuladores

El curso no requiere máquinas virtuales, contenedores ni emuladores. El entorno es el tenant de Microsoft 365 de ISA INTERCOLOMBIA.

| Elemento | Tipo o plataforma | Imagen y versión | Recursos asignados | Red o región | Persistencia |
|---|---|---|---|---|---|
| Tenant de laboratorio | Entorno cloud de Microsoft 365 | Servicio administrado | Licencias del grupo del curso | Región del tenant | Entregables y agentes persisten en la cuenta del participante |
| Sitios de laboratorio | SharePoint Online | Servicio administrado | Biblioteca y noticias | Región del tenant | Eliminar después del curso |

1. Crear el grupo, asignar licencias y agentes.
2. Crear los sitios, la reunión, las páginas de Loop y sembrar correos y actividad.
3. Cargar los recursos y esperar 48 horas de indexación.
4. Después del curso: eliminar los sitios y la reunión, y retirar los agentes de prueba si la política lo exige.

<a id="validacion-entorno"></a>

# Validación del Entorno

| ID | Componente o capacidad | Procedimiento | Resultado esperado | Evidencia mínima |
|---|---|---|---|---|
| V-01 | Licencia de Copilot | Abrir Copilot en [m365.cloud.microsoft](https://m365.cloud.microsoft/) con una cuenta de participante | Responde con datos de trabajo | Captura |
| V-02 | Acceso a archivos | Escribir `/Indicadores_Proyectos_2026` | El archivo aparece en las sugerencias | Captura |
| V-03 | Agentes del curso | Abrir **Agentes** y buscar los nueve agentes del curso (Investigador, Analista y los siete de los prerrequisitos) | Todos abren una conversación | Lista con el nombre en el tenant |
| V-04 | Investigador y búsqueda web | Consulta corta con fuentes web | Respuesta con citas | Captura |
| V-05 | Analista | Adjuntar `Indicadores_Proyectos_2026.xlsx` y pedir el número de proyectos | 12 proyectos | Captura |
| V-06 | Datos sembrados | Preguntar a Copilot: "¿Qué dice el correo INT-MDV ventana del operador?" | Menciona 30 horas | Captura |
| V-07 | Reunión y Facilitator | Abrir la reunión > Opciones de reunión | Facilitator visible | Captura |
| V-08 | Loop | Escribir `/Notas Facilitator INT-MDV` | Aparecen las páginas | Captura |
| V-09 | Galería de indicaciones | Abrir [la galería](https://m365.cloud.microsoft/copilot-prompts) | Se muestra **Mis indicaciones** | Captura |
| V-10 | Agent Builder | Seleccionar **Crear agente** | Se muestra la pestaña **Describir** | Captura (sin guardar) |
| V-11 | Copilot en las aplicaciones | Abrir Copilot en Word, Excel, PowerPoint y Outlook | Disponible en las cuatro | Captura |

**Criterio de entorno listo:** V-01 a V-11 aprobadas con una cuenta de participante. Si un agente no está disponible (V-03), la práctica correspondiente no puede ejecutarse según el temario; documentar el bloqueo y acordar una alternativa con ISA INTERCOLOMBIA antes del curso.

# Comandos de Verificación

## Recursos del repositorio

**Plataforma y terminal:** Windows 11, PowerShell.  
**Directorio de ejecución:** `C:\Cursos\MS-4004-ISA\`.  
**Prerrequisito:** ZIP del repositorio descomprimido.

```powershell
(Get-ChildItem -Recurse -File -Include *.docx,*.xlsx | Group-Object { $_.Directory.Parent.Name } | ForEach-Object { "$($_.Name)=$($_.Count)" }) -join ' '
```

**Resultado esperado:**

```text
Practica01=1 Practica02=2 Practica03=1 Practica04=3 Practica05=3 Practica06=2 Practica07=3 Practica08=6 Practica09=2 Practica10=1 Practica11=1 Practica12=2 Practica13=3 Practica14=2
```

**Interpretación:** confirma que los 32 recursos están disponibles para cargar. No acredita que Copilot pueda leerlos; para eso se usan V-02 y V-05.

## Servicios de Microsoft 365

Copilot, los agentes, Facilitator, la Galería de indicaciones y Agent Builder se validan únicamente en la interfaz web con V-01 a V-11. No se requiere instalar módulos ni SDK.

# Troubleshooting

| Síntoma | Causa probable | Comprobación | Corrección | Validación posterior |
|---|---|---|---|---|
| Un agente no aparece | No asignado o no disponible en el tenant | Buscar en **Todos los agentes** | Asignarlo al grupo y esperar la propagación | V-03 |
| Un archivo no aparece con `/` | No indexado | Abrirlo en OneDrive web | Esperar o adjuntarlo con **+** | V-02 |
| Investigador tarda más de 10 minutos | Consulta extensa | Revisar el historial | Reabrir la conversación; reducir el alcance | V-04 |
| Copilot no encuentra correos o reunión | Datos no sembrados o no indexados | Buscar en Outlook o Teams | Repetir la siembra del guion | V-06 |
| Facilitator no aparece | Directiva o el participante no es coorganizador | Revisar la directiva | Habilitar transcripción y agregar como coorganizador | V-07 |
| El Agente de actualización de estado no encuentra actividad | Poca actividad en el periodo | Revisar correos de la semana | Enviar la actividad del guion; ampliar el periodo | Práctica 6 |
| Project Delta Digest no reconoce el proyecto | Fuentes fuera del conocimiento del agente | Revisar acceso al sitio `INT-MDV (Laboratorio)` | Otorgar lectura y usar el código `INT-MDV-2026` | Práctica 7 |
| No se puede guardar un prompt | Función no disponible en el cliente | Probar en la aplicación web | Crear la indicación desde la galería | V-09 |
| **Crear agente** no disponible | Creación de agentes restringida | Revisar la configuración de Copilot | Permitirla al grupo del curso | V-10 |

# Checklist Final

- [ ] Equipos con Windows 11, navegador vigente y Microsoft 365 Apps actualizadas.
- [ ] Licencia de Microsoft 365 Copilot asignada a participantes e instructor.
- [ ] Agentes del curso visibles para el grupo (V-03).
- [ ] Agent Builder permitido (V-10) y Galería de indicaciones disponible (V-09).
- [ ] Directiva de reuniones con transcripción y Facilitator (V-07).
- [ ] 30 recursos cargados en `Laboratorio_Copilot_ISA` de cada participante.
- [ ] Reunión, correos, páginas de Loop, actividad semanal, sitio del proyecto y noticias preparados con 48 horas de anticipación.
- [ ] Validaciones V-01 a V-11 completadas y registradas.

# Resumen

Para iniciar el curso, cada participante necesita una cuenta con licencia de Microsoft 365 Copilot, acceso a Investigador, Analista, Facilitator y los siete agentes del temario, permiso para crear agentes, la carpeta `Laboratorio_Copilot_ISA` con los recursos y los datos sembrados del proyecto ficticio INT-MDV-2026 en correo, Teams, Loop y SharePoint.

<a id="registro-validacion"></a>

## Registro de validación

| Fecha | Responsable | Plataforma o entorno probado | Resultado | Limitaciones o acciones pendientes |
|---|---|---|---|---|
| 2026-11-06 | Desarrollo de contenido Netec | Revisión del repositorio: estructura, rutas, imágenes, enlaces, recursos, tiempos y alineación con el temario | APTO para publicación del repositorio | No se ejecutaron las prácticas en el tenant de ISA INTERCOLOMBIA. Pendiente: V-01 a V-11 con una cuenta de participante |

## Referencias oficiales

| Documento o recurso | URL | Fecha de consulta |
|---|---|---|
| Información general de Microsoft 365 Copilot | https://learn.microsoft.com/es-es/copilot/plan/copilot-overview | 2026-11-06 |
| Requisitos de Microsoft 365 Copilot | https://learn.microsoft.com/es-es/copilot/plan/microsoft-copilot-requirements | 2026-11-06 |
| Opciones de licencia de Copilot | https://learn.microsoft.com/es-es/copilot/plan/copilot-license-options | 2026-11-06 |
| Agente Investigador (Researcher) | https://learn.microsoft.com/es-es/copilot/manage/researcher-agent | 2026-11-06 |
| Agent Builder | https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder | 2026-11-06 |
| Crear agentes con Agent Builder | https://learn.microsoft.com/es-es/microsoft-365/copilot/extensibility/agent-builder-build-agents | 2026-11-06 |
| Administrar agentes en el centro de administración | https://learn.microsoft.com/es-es/microsoft-agent-365/admin/manage-copilot-agents-integrated-apps | 2026-11-06 |
| Facilitator en Microsoft Teams | https://learn.microsoft.com/es-es/microsoftteams/facilitator-teams | 2026-11-06 |
| Transcripción de reuniones de Teams | https://learn.microsoft.com/es-es/microsoftteams/meeting-transcription-captions | 2026-11-06 |
| Galería de indicaciones de Copilot | https://m365.cloud.microsoft/copilot-prompts | 2026-11-06 |
| Mejores prácticas para escribir prompts | https://support.microsoft.com/es-es/microsoft-365-copilot/get-better-copilot-responses-with-great-prompting | 2026-11-06 |
| Privacidad de datos de Microsoft 365 Copilot | https://learn.microsoft.com/es-es/copilot/plan/microsoft-365-copilot-privacy | 2026-11-06 |
| URL y rangos de direcciones IP de Microsoft 365 | https://learn.microsoft.com/es-es/microsoft-365/enterprise/microsoft-365-endpoints?view=o365-worldwide | 2026-11-06 |

[Inicio](README.md)
