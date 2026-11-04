# Setup Guide General

## IA aplicada al abastecimiento estratégico y negociación con proveedores de Nequi

| Control documental | Valor |
|---|---|
| Curso | IA AB_BA NE (Priv) |
| Repositorio | Organización Netec-Mx; URL por registrar al publicar |
| Alcance | Siete capítulos, siete prácticas, README principal, SETUP_GUIDE.md y recursos de `assets/` |
| Fecha de revisión | 3 de noviembre de 2026 |
| Versión documental | 1.0 |
| Modalidad | Servicios web de IA (Microsoft 365 Copilot Chat o Claude) y aplicaciones de Microsoft 365 |
| Duración | 14 horas · 91.7 % práctica (retos y discusión grupal) · 8.3 % contenidos guiados |

# Objetivo

Preparar un único entorno para todo el repositorio: cuentas, acceso a una herramienta de IA conversacional (Microsoft 365 Copilot Chat con licencia básica o Claude en su plan gratuito), aplicaciones de Microsoft 365 para organizar los entregables y los archivos ficticios del caso transversal.

La guía consolida únicamente preparación, configuración y validación. Los entregables de los retos (matrices, modelos, informes y simulaciones) se construyen durante el curso.

El repositorio contiene documentación, imágenes de apoyo de los laboratorios y archivos ficticios en `assets/`: caso transversal, propuestas de proveedores, datos de mercado y económicos, extractos contractuales, propuesta final, condiciones de referencia y plantillas en Excel. No distribuye instaladores, agentes ni configuraciones de tenant.

**Política de información:** durante la capacitación se utiliza exclusivamente información ficticia y fuentes públicas. Los participantes verifican los resultados generados por IA y respetan las políticas de seguridad y tratamiento de información de su organización.

# Requisitos de Hardware

| Recurso | Requisito consolidado |
|---|---|
| Equipo | Computadora portátil o de escritorio con procesador de 64 bits |
| Memoria | 8 GB de RAM como mínimo |
| Espacio libre | 2 GB para archivos del curso y entregables |
| Pantalla | Mínimo 1366 × 768; recomendado 1920 × 1080 o un segundo monitor para trabajar con la IA y Excel en paralelo |
| Periféricos | Teclado, dispositivo apuntador y audio para las sesiones en línea |
| Conexión | Internet estable y HTTPS saliente por TCP 443 durante toda la sesión |

No se requiere GPU ni virtualización de hardware. Todas las herramientas de IA del curso se ejecutan como servicios web.

# Sistemas Operativos Compatibles

| Sistema | Condición de uso |
|---|---|
| Windows | Sistema con soporte vigente y Microsoft Edge de 64 bits administrado, como configuración común recomendada. |
| macOS | Sistema con soporte vigente y navegador compatible actualizado; validar el acceso a las aplicaciones de Microsoft 365 del tenant. |

Si se utiliza un navegador distinto de Edge, confirmar su autorización institucional y su funcionamiento con Copilot Chat, Claude y Microsoft 365.

# Software Requerido

## Plataforma común

| Componente | Edición o versión requerida | Condición de preparación |
|---|---|---|
| Microsoft 365 Copilot Chat **o** Claude | Copilot Chat (básico), incluido con licencias Microsoft 365 elegibles, o Claude en plan gratuito | Al menos una de las dos herramientas debe estar disponible para cada participante. |
| Microsoft Excel | Microsoft 365, versión web o de escritorio vigente | Crear matrices, fórmulas (incluida `SUMAPRODUCTO`) y gráficos. |
| Microsoft Word | Microsoft 365, versión web o de escritorio vigente | Elaborar informes y documentos de trabajo. |
| OneDrive para la Empresa | Servicio organizacional | Carpeta `/Curso-IA-Abastecimiento` para los entregables. |
| Microsoft Edge | Versión estable vigente, 64 bits, administrada | Acceso a los servicios web. |

No se requiere Copilot integrado en Word ni en Excel: los resultados de la IA se organizan en las aplicaciones convencionales de Microsoft 365.

## Componentes opcionales

| Componente | Cuándo aplica |
|---|---|
| Agentes Researcher y Analyst | Participantes con licencia Microsoft 365 Copilot. Se usan en los retos 2, 3, 4 y 7. Quien no los tenga trabaja con prompts especializados. |
| Claude Projects | Reto 7, según disponibilidad del plan. Alternativa: instrucción especializada al inicio de la conversación. |
| Segunda herramienta de IA | Recomendable para comparar resultados entre herramientas y como respaldo ante límites de uso. |

La guía no exige licencias premium, agentes personalizados, conectores, automatizaciones ni instalación de software adicional.

# Herramientas y Dependencias

## Licencias y cuentas

Antes del curso, TI debe confirmar para cada participante:

- Cuenta organizacional Microsoft Entra ID con acceso a Microsoft 365 (Excel, Word y OneDrive).
- Acceso a Microsoft 365 Copilot Chat habilitado por el tenant, **o** cuenta de Claude en el plan gratuito, si la política de la organización lo permite.
- Opcional: licencia Microsoft 365 Copilot para usar Researcher y Analyst.
- MFA y requisitos de dispositivo satisfechos, si los exige el tenant.

Consideraciones por herramienta:

- **Copilot Chat (básico):** chat con información web, carga y análisis de archivos y protección de datos empresariales. La disponibilidad de funciones depende de la configuración del tenant. Consulta la [información general de Copilot Chat](https://learn.microsoft.com/es-es/copilot/overview).
- **Claude gratuito:** tiene límites de uso que se renuevan por periodos; la búsqueda web y las funciones disponibles dependen del plan. Consulta los [planes de Claude](https://claude.com/pricing) y las [buenas prácticas de límites de uso](https://support.claude.com/en/articles/9797557-usage-limit-best-practices).
- **Researcher y Analyst:** requieren licencia Microsoft 365 Copilot. Consulta [Researcher](https://support.microsoft.com/es-es/topic/e63ab760-f3de-4c47-ae87-dad601b0e9c4) y [Analyst](https://support.microsoft.com/es-es/microsoft-365-copilot/get-started-with-analyst-in-microsoft-365-copilot).

## Matriz de herramientas por reto

| Reto | Herramienta base | Opcional | Funciones utilizadas |
|---|---|---|---|
| 1. Oportunidades | Copilot Chat o Claude | — | Chat y prueba de prompts |
| 2. Mercado | Copilot Chat o Claude con búsqueda web | Researcher | Búsqueda web con citas |
| 3. Propuestas | Copilot Chat o Claude | Analyst | Carga y análisis de archivos |
| 4. Economía | Copilot Chat o Claude | Analyst | Carga de Excel o CSV y propuesta de fórmulas |
| 5. Riesgos y contratos | Copilot Chat o Claude | Researcher o Analyst | Carga de archivos y análisis de texto |
| 6. Negociación | Claude o Copilot Chat | — | Simulación de rol en conversación prolongada |
| 7. Recomendación | Copilot Chat o Claude | Claude Projects, Researcher, Analyst | Instrucciones especializadas y carga de archivos |

## Permisos

| Ámbito | Permiso necesario |
|---|---|
| Microsoft 365 | Crear, editar y guardar archivos de Excel y Word en OneDrive. |
| Copilot Chat | Acceso habilitado y carga de archivos permitida por el tenant. |
| Claude | Uso permitido por la política de la organización para información ficticia. |
| Red | Acceso a los dominios de Microsoft 365 y de Claude a través del proxy institucional. |

El participante no necesita permisos de administrador.

# Instalación y Configuración

## 1. Preparar el acceso web

1. Actualizar el navegador mediante el mecanismo institucional.
2. Usar un perfil con la cuenta organizacional del curso.
3. Abrir [Microsoft 365 Copilot Chat](https://m365copilot.com) y verificar que se puede iniciar una conversación.
4. Si se usa Claude, iniciar sesión en `claude.ai` con la cuenta autorizada y verificar que se puede iniciar una conversación.
5. Abrir Excel y Word desde el iniciador de Microsoft 365 y comprobar edición y guardado.

## 2. Habilitar funciones de las herramientas de IA

1. En Copilot Chat, confirmar que es posible cargar un archivo y que las respuestas incluyen información web cuando se solicita.
2. En Claude, habilitar la búsqueda web si está disponible en el plan ([guía oficial](https://support.claude.com/en/articles/10684626-enabling-and-using-web-search)) y verificar la carga de archivos ([guía oficial](https://support.claude.com/en/articles/8241126-upload-files-to-claude)).
3. Si el participante tiene licencia Microsoft 365 Copilot, confirmar que Researcher y Analyst aparecen en la sección de agentes.
4. Si el plan de Claude lo permite, confirmar que se puede crear un proyecto ([What are projects?](https://support.claude.com/en/articles/9517075-what-are-projects)).

## 3. Preparar la carpeta de trabajo

Crear en OneDrive:

```text
/Curso-IA-Abastecimiento/
├── Reto01/
├── Reto02/
├── Reto03/
├── Reto04/
├── Reto05/
├── Reto06/
└── Reto07/
```

## 4. Descargar los archivos del curso

Descargar la carpeta [assets/](assets/) del repositorio y guardarla en `/Curso-IA-Abastecimiento/assets`.

# Configuración Base para los Laboratorios

## Archivos ficticios del caso

| Archivo | Reto | Contenido |
|---|---|---|
| [caso-transversal-nequi.docx](assets/caso-transversal-nequi.docx) | Todos | Contexto, contrato vigente y proveedores alternativos ficticios |
| [plantillas-retos.xlsx](assets/plantillas-retos.xlsx) | 1, 2, 3, 5, 7 | Plantillas de matriz de oportunidades, benchmark, evaluación, riesgos, seguimiento y biblioteca |
| [reto02-datos-ficticios-mercado.xlsx](assets/reto02-datos-ficticios-mercado.xlsx) | 2 | Datos comerciales ficticios para cuando no hay información pública |
| [reto03-propuesta-renovacion-tecnosoporte.docx](assets/reto03-propuesta-renovacion-tecnosoporte.docx) | 3 | Propuesta de renovación del proveedor actual |
| [reto03-oferta-nubia.docx](assets/reto03-oferta-nubia.docx) | 3 | Oferta ficticia del proveedor alternativo A |
| [reto03-oferta-orbital.docx](assets/reto03-oferta-orbital.docx) | 3 | Oferta ficticia del proveedor alternativo B |
| [reto04-datos-economicos.xlsx](assets/reto04-datos-economicos.xlsx) | 4 | Datos económicos y supuestos |
| [reto04-datos-economicos.csv](assets/reto04-datos-economicos.csv) | 4 | Formato alternativo de los datos económicos |
| [reto05-extractos-contrato.docx](assets/reto05-extractos-contrato.docx) | 5 | Cláusulas del contrato vigente y de la propuesta de renovación |
| [reto07-propuesta-final.docx](assets/reto07-propuesta-final.docx) | 7 | Propuesta final común del proveedor actual |
| [reto07-condiciones-referencia-nequi.docx](assets/reto07-condiciones-referencia-nequi.docx) | 7 | Condiciones de referencia para la evaluación final |

Todos los nombres de proveedores, cifras y condiciones son ficticios. En el reto 2 se investigan proveedores reales únicamente con fuentes públicas.

## Datos de referencia del caso

| Dato | Valor |
|---|---|
| Tarifa vigente | COP 180 M mensuales antes de IVA |
| Propuesta de renovación | +18 % (COP 212,4 M mensuales) |
| Horizonte de análisis | 36 meses |
| Volumen de tickets | 260 mensuales |
| Costo interno de transición | COP 90 M |

## Gestión de la contrapropuesta del reto 6

La contrapropuesta del reto 6 es material del instructor y **no se publica en el repositorio**, porque su efecto didáctico depende de que sea inesperada. El instructor la comparte con los participantes durante la Actividad 2 del reto 6 por el canal del curso.

# Servicios Externos Requeridos

| Servicio | Acceso |
|---|---|
| Microsoft Entra ID | Autenticación y MFA. |
| Microsoft 365 Copilot Chat | Conversaciones, información web y carga de archivos. |
| Claude (Anthropic) | Alternativa de herramienta de IA conversacional. |
| Microsoft 365 web y OneDrive | Edición y almacenamiento de entregables. |
| Sitios públicos de proveedores | Investigación de mercado del reto 2. |
| GitHub | Consulta y descarga de la documentación del curso. |

TI debe revisar las [URL y rangos de direcciones IP de Microsoft 365](https://learn.microsoft.com/es-es/microsoft-365/enterprise/urls-and-ip-address-ranges) y permitir el acceso a los dominios de Claude si su uso está autorizado. No se abren puertos entrantes.

# Validación del Entorno

Completar la siguiente validación con una cuenta de participante antes del curso:

| Comprobación | Resultado esperado |
|---|---|
| Herramienta de IA | Copilot Chat o Claude responde a un prompt de prueba. |
| Carga de archivos | La herramienta lee `caso-transversal-nequi.docx` y resume el contexto. |
| Búsqueda web | La herramienta responde con al menos una fuente citada. |
| Excel | Se crea un archivo con `SUMAPRODUCTO` y un gráfico de barras. |
| Word | Se crea, guarda y vuelve a abrir un documento. |
| OneDrive | Existe la carpeta `/Curso-IA-Abastecimiento` con las subcarpetas de los retos. |
| Agentes (opcional) | Researcher y Analyst visibles para quien tenga licencia Microsoft 365 Copilot. |

## Pruebas mínimas de preparación

1. **Prompt de prueba:** enviar «Resume en cinco viñetas el documento adjunto» con `caso-transversal-nequi.docx`.
2. **Búsqueda web:** pedir «Lista tres fuentes públicas sobre servicios gestionados de soporte tecnológico, con URL».
3. **Excel:** cargar `reto04-datos-economicos.xlsx` en la herramienta de IA y pedir un resumen de los componentes de costo.
4. **Cierre:** eliminar las conversaciones de prueba si se trabaja en un equipo compartido.

# Comandos de Verificación

El curso funciona en navegador y no necesita CLI. Los comandos siguientes son diagnósticos opcionales del puesto.

## Windows PowerShell

```powershell
Get-CimInstance Win32_OperatingSystem |
    Select-Object Caption, Version, OSArchitecture
Get-CimInstance Win32_ComputerSystem |
    Select-Object @{Name='RAM_GB';Expression={[math]::Round($_.TotalPhysicalMemory / 1GB, 1)}}

$serviceHosts = @('m365copilot.com', 'login.microsoftonline.com', 'claude.ai', 'github.com')
foreach ($serviceHost in $serviceHosts) {
    Test-NetConnection -ComputerName $serviceHost -Port 443 -InformationLevel Quiet
}
```

Resultado esperado: sistema de 64 bits, 8 GB de RAM o más y `True` para cada servicio si la red permite salida directa. En redes con proxy, contrastar con el acceso real del navegador.

## macOS, terminal

```bash
sw_vers
sysctl -n hw.memsize
curl -L -sS -o /dev/null -w 'HTTP final: %{http_code}\n' --max-time 30 https://m365copilot.com/
```

Resultado esperado: sistema identificado, al menos 8 GB de memoria (el comando devuelve bytes) y un código HTTP de respuesta. Una página de inicio de sesión no demuestra acceso a las funciones de IA.

# Troubleshooting

| Problema | Comprobación y corrección |
|---|---|
| Copilot Chat no aparece | Verificar la licencia de Microsoft 365 y la habilitación de Copilot Chat en el tenant. |
| No se pueden cargar archivos en Copilot Chat | Revisar la configuración del tenant; copiar el texto del documento en la conversación como alternativa. |
| Claude alcanza el límite de uso | Continuar con Copilot Chat; escribir prompts completos y abrir conversaciones nuevas con un resumen del contexto. |
| La búsqueda web no está disponible | Activarla en la herramienta o usar los datos ficticios del reto 2, documentando la limitación. |
| Researcher o Analyst no aparecen | Requieren licencia Microsoft 365 Copilot; usar prompts especializados. |
| Claude Projects no está disponible | Usar una instrucción especializada al inicio de la conversación. |
| La herramienta no lee el Excel | Usar `reto04-datos-economicos.csv` o pegar la tabla en la conversación. |

# Checklist Final

- [ ] Equipo de 64 bits, 8 GB de RAM y conexión estable.
- [ ] Acceso a Copilot Chat o Claude verificado por participante.
- [ ] Carga de archivos y búsqueda web probadas.
- [ ] Excel, Word y OneDrive operativos.
- [ ] Carpeta `/Curso-IA-Abastecimiento` creada con subcarpetas por reto.
- [ ] Archivos de `assets/` descargados.
- [ ] Participantes con licencia premium identificados (Researcher y Analyst).
- [ ] Política de uso de información ficticia comunicada.

# Resumen

El curso utiliza herramientas de IA conversacional accesibles con licencias básicas o planes gratuitos, complementadas con Excel y Word para organizar los entregables. Los agentes premium son opcionales y los ejercicios están diseñados para que todos los participantes alcancen los objetivos con la herramienta disponible.

## Alcance de la revisión y pendientes del cliente

Se revisaron las siete prácticas, el README principal y los archivos de `assets/` para consolidar los requisitos. No se tuvo acceso al tenant del cliente: la disponibilidad de Copilot Chat, la política de uso de Claude, la carga de archivos y las licencias premium deben validarse allí antes de impartir el curso.

## Referencias oficiales

- [Información general de Microsoft Copilot Chat](https://learn.microsoft.com/es-es/copilot/overview)
- [Privacidad y protecciones de Copilot Chat](https://learn.microsoft.com/es-es/copilot/privacy-and-protections)
- [Información general de Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview)
- [Introducción a Researcher](https://support.microsoft.com/es-es/topic/e63ab760-f3de-4c47-ae87-dad601b0e9c4)
- [Introducción a Analyst](https://support.microsoft.com/es-es/microsoft-365-copilot/get-started-with-analyst-in-microsoft-365-copilot)
- [Planes de Claude](https://claude.com/pricing)
- [Claude: usage limit best practices](https://support.claude.com/en/articles/9797557-usage-limit-best-practices)
- [Claude: upload files](https://support.claude.com/en/articles/8241126-upload-files-to-claude)
- [Claude: web search](https://support.claude.com/en/articles/10684626-enabling-and-using-web-search)
- [Claude: projects](https://support.claude.com/en/articles/9517075-what-are-projects)
- [URL y rangos de direcciones IP de Microsoft 365](https://learn.microsoft.com/es-es/microsoft-365/enterprise/urls-and-ip-address-ranges)
- [Test-NetConnection](https://learn.microsoft.com/es-es/powershell/module/nettcpip/test-netconnection)
