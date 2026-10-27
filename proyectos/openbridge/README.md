<div align="center">

<img src="assets/hero.svg" alt="OpenBridge: menos búsqueda, mejores decisiones. Portada oficial de presentación conceptual." width="100%" />

<br/>

**OPEN SOURCE DISCOVERY · AI-ASSISTED ARCHITECTURE · DEVELOPER TOOLS**

**Proyecto colaborativo · No Country 2026 · Vista de presentación / versión de prueba**

[**El desafío**](#el-desafio) · [**La solución**](#la-solucion) · [**Arquitectura**](#arquitectura-propuesta) · [**Documentación**](#centro-de-documentacion) · [**Equipo**](#nuestro-equipo)

</div>

---

> ### Una mejor arquitectura comienza con mejores decisiones.
>
> **OpenBridge** plantea un puente entre el universo de herramientas open source y las necesidades reales de los equipos que construyen software. Descubrir, evaluar, conectar y recomendar: **menos tiempo explorando opciones dispersas; más criterio para crear productos.**

## El desafio

En el escenario definido por **No Country**, arquitectos y líderes técnicos dedican **entre 15 y 20 horas por proyecto** a investigar manualmente librerías, herramientas y servicios open source. Comparar información dispersa dificulta valorar mantenimiento, compatibilidad y posibilidades de integración.

**Nuestra oportunidad:** convertir múltiples fuentes técnicas en un recorrido de descubrimiento claro y recomendaciones contextualizadas.

> **Nota metodológica:** las 15–20 horas son un dato del [brief del desafío](https://drive.google.com/file/d/1jl3HN2pWct3DZLqGiusHl49pQeCpu_EO/view). No representan un ahorro medido ni un resultado obtenido por el equipo.

## La solucion

| | Capacidad propuesta | Valor para quien desarrolla |
|---|---|---|
| **01** | **Catálogo inteligente** | Descubrir proyectos según categoría, lenguaje, licencia y señales de mantenimiento. |
| **02** | **Fichas técnicas útiles** | Revisar métricas, actividad, licencias y posibilidades de uso. |
| **03** | **Integraciones con contexto** | Entender cómo conectar herramientas mediante API, SDK, Docker o webhooks. |
| **04** | **Asistente de arquitectura con IA** | Recibir alternativas de stack justificadas según el problema del negocio. |

**Alcance objetivo del desafío:** catálogo de al menos **100 repositorios**, filtros y búsqueda, ficha de salud del proyecto, ingesta automatizada desde GitHub y asistente con recuperación contextual (RAG).

> Estas capacidades son **objetivos de desarrollo**, no funcionalidades declaradas como terminadas.

## De una idea a una arquitectura

**Ejemplo ilustrativo, no una demostración del software:**

**Necesidad:** «Estoy creando un e-commerce B2B para operaciones logísticas».

```text
NECESIDAD DEL NEGOCIO
        │
        ▼
CONTEXTO + REQUISITOS
        │
        ▼
CATÁLOGO DE REPOSITORIOS
        │
        ▼
RELEVANCIA + MANTENIMIENTO + LICENCIA
        │
        ▼
STACK SUGERIDO + PATRONES DE INTEGRACIÓN
        │
        ▼
EXPLICACIÓN Y REVISIÓN HUMANA
```

El sistema debe apoyar decisiones técnicas, no reemplazar la evaluación de seguridad, licencias, costos, soporte o compatibilidad.

## Arquitectura propuesta

```mermaid
flowchart LR
    U["Usuario / necesidad"] --> WEB["Interfaz web"]
    WEB --> API["Servicios / API"]
    G["GitHub REST / GraphQL"] --> PIPE["Ingesta y normalización"]
    PIPE --> DB[("Catálogo y metadatos")]
    DB --> API
    DB --> RAG["Recuperación semántica / RAG"]
    RAG --> IA["Recomendaciones justificadas"]
    IA --> API
    API --> WEB
```

**Puntos de diseño pendientes de validar:**

- Estrategia de sincronización y límites de las API de GitHub.
- Modelo de indicadores de salud y actualización del repositorio.
- Recuperación semántica, calidad de las fuentes y trazabilidad de recomendaciones.
- Estructuración de integraciones, compatibilidad y ejemplos reproducibles.
- Contrato frontend/backend, pruebas, despliegue y seguridad.

**Tecnologías:** el desafío sugiere Next.js/React, FastAPI o Node.js, PostgreSQL/pgvector o Qdrant y herramientas para RAG. **Ninguna de estas alternativas se declara aquí como tecnología implementada sin validación del equipo.**

## Centro de documentacion

> **Evaluadores:** pueden comenzar por el documento de requisitos, continuar por el espacio de gestión y revisar las tareas y decisiones. Estos enlaces llevan a fuentes existentes, pero su **acceso público debe verificarse antes de la entrega final**.

| Fuente | Qué permite consultar |
|---|---|
| [**Brief oficial de No Country**](https://drive.google.com/file/d/1jl3HN2pWct3DZLqGiusHl49pQeCpu_EO/view) | Problema, alcance, entregables y tecnologías sugeridas. |
| [**Gestión del proyecto · Notion**](https://app.notion.com/p/3ff997f897ee81f3a11cea1379ea28a6?pvs=204) | Centro de coordinación y organización del equipo. |
| [**Documentación y entregables**](https://app.notion.com/p/3ff997f897ee81d6bc48d1d36b2603fd?pvs=204) | Requisitos, evidencias y control de entrega. |
| [**Tablero de tareas**](https://app.notion.com/p/9aa45edd39dd45ec96f91a1962b9b932?pvs=204) | Avances, responsables y criterios de aceptación. |
| [**Decisiones y riesgos**](https://app.notion.com/p/def7d0d2fd044dd0a5ec18cfcf964659?pvs=204) | Registro de acuerdos, incertidumbres y bloqueos. |
| [**Reuniones**](https://app.notion.com/p/d798a39cb79b4d5284d80650516b6123?pvs=204) | Registro del trabajo colaborativo. |
| [**Carpeta OpenBridge · Drive**](https://drive.google.com/drive/folders/1EQS0Utv815jEGypP3ApMJfVABJA02h7B) | Recursos y archivos compartidos del proyecto. |

**Pendientes para completar esta navegación:** enlace del repositorio de código del equipo, prototipo UX/UI, documentación técnica validada, demo navegable, video de presentación y resultados de pruebas. No se incluyen vínculos ficticios.

## Nuestro equipo

<div align="center">

### El talento detrás de OpenBridge

**Cuatro disciplinas. Un objetivo: transformar problemas reales en productos tecnológicos.**

Diseño, coordinación, inteligencia artificial y datos: conocé a las personas detrás de cada decisión.

</div>

<table>
<tr>
<td align="center" width="50%" valign="top">
<img src="assets/team/david-card.svg" width="100%" alt="Tarjeta de David Vergara, Project Manager, con avatar ilustrado circular y borde luminoso" />
<br />
<strong>David Vergara</strong><br />
<sub>Project Manager</sub><br /><br />
<a href="https://github.com/marcketingdigital-cloud" title="Visitar GitHub de David Vergara"><img src="assets/team/github-active.svg" width="42%" alt="Abrir GitHub de David Vergara" /></a>
<img src="assets/team/linkedin-pending.svg" width="42%" alt="LinkedIn pendiente de confirmar para David Vergara" />
</td>
<td align="center" width="50%" valign="top">
<img src="assets/team/fabian-card.svg" width="100%" alt="Tarjeta de Fabián, Frontend · UX/UI, con avatar ilustrado circular y borde luminoso" />
<br />
<strong>Fabián</strong><br />
<sub>Frontend · UX/UI</sub><br /><br />
<a href="https://github.com/fabianmartinezcaro" title="Visitar GitHub de Fabián"><img src="assets/team/github-active.svg" width="42%" alt="Abrir GitHub de Fabián" /></a>
<a href="https://www.linkedin.com/in/fabianmartinezcaro/" title="Conectar con Fabián en LinkedIn"><img src="assets/team/linkedin-active.svg" width="42%" alt="Conectar con Fabián en LinkedIn" /></a>
</td>
</tr>
<tr>
<td align="center" width="50%" valign="top">
<img src="assets/team/andres-card.svg" width="100%" alt="Tarjeta de Andrés, Ingeniería de IA, con avatar ilustrado circular y borde luminoso" />
<br />
<strong>Andrés</strong><br />
<sub>Ingeniería de IA</sub><br /><br />
<a href="https://github.com/andigles" title="Visitar GitHub de Andrés"><img src="assets/team/github-active.svg" width="42%" alt="Abrir GitHub de Andrés" /></a>
<img src="assets/team/linkedin-pending.svg" width="42%" alt="LinkedIn pendiente de confirmar para Andrés" />
</td>
<td align="center" width="50%" valign="top">
<img src="assets/team/jeison-card.svg" width="100%" alt="Tarjeta de Jeison, Datos · Machine Learning, con avatar ilustrado circular y borde luminoso" />
<br />
<strong>Jeison</strong><br />
<sub>Datos · Machine Learning</sub><br /><br />
<a href="https://github.com/Jeisz" title="Visitar GitHub de Jeison"><img src="assets/team/github-active.svg" width="42%" alt="Abrir GitHub de Jeison" /></a>
<a href="https://www.linkedin.com/in/jeison-zapata" title="Conectar con Jeison en LinkedIn"><img src="assets/team/linkedin-active.svg" width="42%" alt="Conectar con Jeison en LinkedIn" /></a>
</td>
</tr>
</table>

> **Perfiles profesionales:** los cuatro GitHub están enlazados. LinkedIn está disponible para Fabián y Jeison; los demás se muestran como pendientes sin enlace. Los avatares siguen siendo ilustraciones temporales hasta recibir fotografías autorizadas. Solo se presentan las dos redes acordadas.

La distribución técnica detallada se confirmará con el equipo. Backend, integración y pruebas siguen con responsables por acordar.

<a id="open-to-opportunities"></a>

<div align="center">

<img src="assets/team/opportunities.svg" alt="Open to Opportunities: conectemos talento con desafíos reales. Invitación a reclutadores de perfiles en Project Management, Frontend, IA y Machine Learning." width="100%" />

### ¿Reclutás talento para tu próximo proyecto?

**Conocé al equipo que está construyendo OpenBridge.** Explorá la propuesta, evaluá nuestras especialidades y conectá por GitHub o LinkedIn con perfiles identificados.

<a href="https://github.com/marcketingdigital-cloud/marcketingdigital-cloud/tree/main/proyectos/openbridge"><img src="assets/team/cta-project.svg" width="43%" alt="Explorar OpenBridge en GitHub" /></a>
<a href="https://github.com/marcketingdigital-cloud"><img src="assets/team/cta-pm.svg" width="43%" alt="Ver GitHub del Project Manager" /></a>

<sub>La disponibilidad para oportunidades laborales debe ser confirmada por cada integrante. Los enlaces restantes se activarán cuando cada integrante confirme su URL.</sub>

</div>

## Estado y transparencia

| Dimensión | Estado en esta presentación |
|---|---|
| Problema de negocio y requisitos | **Documentados** en el brief. |
| Dirección del producto | **Propuesta definida**. |
| Coordinación y documentación | **Espacio real identificado** en Notion. |
| Arquitectura | **Conceptual**, pendiente de validación técnica. |
| Catálogo, asistente, ingesta y datos | **Entrega y evidencias pendientes de verificar**. |
| Demo pública y despliegue | **No confirmados**. |
| README visual | **Versión de prueba publicada**, complementable por el equipo. |

## Camino hacia la demo

1. **Alinear alcance:** validar las funciones mínimas que se mostrarán.
2. **Construir un recorrido completo:** búsqueda → ficha → recomendación.
3. **Integrar y probar:** datos reales, contratos entre componentes y respuesta reproducible.
4. **Documentar con evidencia:** capturas, instrucciones de ejecución, resultados y limitaciones.
5. **Presentar al jurado:** demo, decisiones técnicas, aportes del equipo y próximos pasos.

---

<div align="center">

### Menos búsqueda. Mejores decisiones.

**OpenBridge** · Descubrir tecnologías es el comienzo; integrarlas con criterio es el objetivo.

[Inicio](#el-desafio) · [Documentación](#centro-de-documentacion) · [Equipo](#nuestro-equipo)

<sub>Simulación laboral No Country · Documento de presentación conceptual · Octubre de 2026</sub>

</div>