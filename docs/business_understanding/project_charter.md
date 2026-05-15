# Project Charter - Entendimiento del Negocio

## Nombre del Proyecto

Asistente de apoyo a *threat hunting* basado en LLM y datos de CTI (RAG / ajuste fino en fases posteriores).

## Objetivo del Proyecto

Diseñar una solución alineada al **Team Data Science Process (TDSP)** que evolucione hacia un asistente conversacional para contextualizar amenazas (CVE, MITRE, KEV), apoyar lectura de hallazgos y priorización para el área de seguridad. La **Fase 1** cubre entendimiento del negocio, alcance y carga documentada de datos públicos de referencia (Hugging Face y Kaggle).

## Alcance del Proyecto

### Incluye:

- Marco de proyecto, stakeholders y criterios de éxito (versión documental 1.0 al 4 de junio de 2026).
- Ingesta de CTI público: `Shomi28/cyber-threat-intelligence` (HF) y `prayanshusinghgaur/cybersecurity-threat-intelligence` (Kaggle).
- Diccionarios de datos completos y trazabilidad negocio ↔ variables (ver notebook de Fase 1).
- Fases siguientes: preprocesamiento, EDA, modelado, despliegue y evaluación.

### Excluye:

- Entrenamiento o despliegue en producción de un LLM en la Fase 1.
- Ingesta de logs o datos internos reales del negocio (hasta definir gobierno y permisos).
- Automatización completa de pipelines SOC/CI/CD.

## Metodología

**TDSP:** Entendimiento del negocio → Adquisición y comprensión de datos → Modelado → Despliegue → Aceptación y visualización.

## Cronograma

| Etapa | Duración referencial | Fechas (2026) |
|-------|---------------------|---------------|
| Entendimiento del negocio y carga de datos | 1 semana | **7 mayo – 14 mayo** |
| Preprocesamiento y EDA | 1 semana | *Plan tentativo: 14 mayo - 21 mayo* |
| Modelamiento y extracción de características | 1 semana | *Plan tentativo: 21 mayo - 28 mayo* |
| Despliegue / Evaluación y entrega final | 1 semana | *Plan tentativo: 28 mayo - 4 junio* |

*Cohorte: 2026-II (mayo 2026). Fechas posteriores a la Fase 1 son preliminares.*

## Equipo del Proyecto

- **Líder y desarrollador:** David Martínez (proyecto individual).

## Presupuesto

**COP $25.000.000** (referencial): cómputo en nube, APIs de modelos, almacenamiento CTI, pruebas e integración futura; parte del trabajo académico puede usar infraestructura gratuita o institucional.

## Stakeholders

- **CISO / Director(a) de ciberseguridad:** priorización ejecutiva y trazabilidad CVE/MITRE/KEV.
- **Líder del SOC:** síntesis de incidentes y triage asistido.
- **Analista sénior de threat intelligence:** datos estructurados e informes homogéneos.
- **GRC / auditoría interna:** evidencia y repetibilidad del análisis.
- **Integrador tecnológico:** evaluación de copilotos de seguridad con datos públicos verificables.

## Aprobaciones

- **Revisión documental hasta versión 1.0** (charter, diccionarios, notebook de Fase 1).
- **Responsable:** David Martínez.
- **Cierre v1.0 previsto:** 4 de junio de 2026. *Firma institucional según exija el curso o el empleador.*
