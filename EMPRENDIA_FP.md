# EMPRENDIA_FP.md — Documento EmprendeIA FP

**Proyecto:** EmprendIA FP · **Versión:** 1.0 · **Fecha:** 3 de noviembre de 2026

**Estado:** Fase 0 — definición y documentación del producto. **No existe aplicación ni código.**.

> **Leyenda de estados usada en este documento:**
> - **Aprobado** = decisión tomada por el responsable del proyecto.
> - **Propuesto** = recomendación técnica NO aprobada todavía.
> - **Hipótesis** = afirmación pendiente de validación empírica.
> - **Pendiente** = dato/fuente que no ha podido verificarse; no debe presentarse como cierto.

---

## Índice

1. [Resumen ejecutivo](#1-resumen-ejecutivo)
2. [Problema y oportunidad](#2-problema-y-oportunidad)
3. [Objetivos del proyecto](#3-objetivos-del-proyecto)
4. [Usuarios objetivo y propuesta de valor](#4-usuarios-objetivo-y-propuesta-de-valor)
5. [Análisis de mercado y competencia](#5-análisis-de-mercado-y-competencia)
6. [Funcionalidades de la plataforma](#6-funcionalidades-de-la-plataforma)
7. [Recorridos de usuario y experiencia de uso](#7-recorridos-de-usuario-y-experiencia-de-uso)
8. [Alcance y prioridades del MVP](#8-alcance-y-prioridades-del-mvp)
9. [Modelo de negocio](#9-modelo-de-negocio)
10. [Arquitectura técnica](#10-arquitectura-técnica)
11. [Inteligencia artificial y procesamiento de datos](#11-inteligencia-artificial-y-procesamiento-de-datos)
12. [Relación con los contenidos del curso](#12-relación-con-los-contenidos-del-curso)
13. [Seguridad, privacidad y RGPD](#13-seguridad-privacidad-y-rgpd)
14. [Fuentes oficiales e integraciones](#14-fuentes-oficiales-e-integraciones)
15. [Viabilidad económica y costes](#15-viabilidad-económica-y-costes)
16. [Riesgos y limitaciones](#16-riesgos-y-limitaciones)
17. [Plan de validación del MVP](#17-plan-de-validación-del-mvp)
18. [Hoja de ruta](#18-hoja-de-ruta)
19. [Decisiones pendientes](#19-decisiones-pendientes-requieren-aprobación-del-responsable)
20. [Instrucciones y convenciones para agentes de IA](#20-instrucciones-y-convenciones-para-agentes-de-ia)
21. [Referencias y bibliografía](#21-referencias-y-bibliografía)

---

## 1. Resumen ejecutivo

**EmprendeIA FP** es una plataforma web asistida por IA que acompaña al alumnado de Formación Profesional (cursos de especialización, grados medios y superiores) desde su **proyecto final de curso** hasta la posible puesta en marcha de un negocio. Analiza la idea, evalúa su potencial comercial, identifica necesidades tecnológicas y su coste, calcula la viabilidad económica, localiza ayudas y financiación (España y Castilla-La Mancha), explica los trámites necesarios y genera un plan de lanzamiento personalizado con seguimiento.

La IA **orienta y organiza**; no sustituye el asesoramiento profesional jurídico, fiscal ni laboral, y distingue siempre entre **datos contrastados (con fuente y fecha), estimaciones y hipótesis**.

- **Propuesta de valor:** *"Un tutor IA continuo que toma tu proyecto de FP, lo analiza con fuentes oficiales, te dice qué puede funcionar, cuánto costaría, qué ayudas puedes pedir y qué pasos dar, en un plan claro y adaptado a tu situación."*
- **Diferenciadores:** contexto específico de FP; fuentes oficiales trazables; motor económico determinista (fórmulas auditables, no cifras generadas por el modelo); human-in-the-loop en conclusiones críticas; seguimiento temporal.
- **Contexto académico:** nace en el módulo profesional **"Sistemas de Big Data"** (6 ECTS, 55 h, 2+1 h semanales, programación en Python; docente Sebastián Romero López) del Curso de Especialización en **Inteligencia Artificial y Big Data** de Albacete.
- **Estado:** documentación definida; el MVP está delimitado y priorizado; ninguna decisión tecnológica está aprobada; no se han realizado aún las validaciones previstas.

---

## 2. Problema y oportunidad

### 2.1 Problema concreto

1. **Abandono de proyectos con potencial.** Los proyectos finales se evalúan académicamente y se archivan; no existe un proceso que los convierta en oportunidades reales.
2. **Desconocimiento de ayudas y trámites.** El alumnado ignora qué subvenciones existen, quién las concede, cuándo y con qué requisitos.
3. **Falta de criterio económico.** No se sabe cuánto cuesta montar el negocio, qué ingresos son plausibles ni en qué condiciones se alcanza el punto de equilibrio.
4. **Escasez de acompañamiento.** Los servicios públicos de apoyo al emprendimiento tienen capacidad limitada y no llegan a todo el alumnado al final del curso.
5. **Brecha de edad/experiencia.** Muchos alumnos son jóvenes que desconocen el régimen de autónomos, las obligaciones fiscales y las formas societarias.


### 2.2 Oportunidad

- La IA permite, a coste marginal bajo, realizar análisis que antes requerían consultores o técnicos especializados.
- Los datos de subvenciones y normativa son públicos; el problema es la **filtración y actualización**, no la disponibilidad (pendiente de verificar en cada fuente, §14).
- Los centros de FP tienen incentivos institucionales para mejorar la inserción laboral y el emprendimiento; la plataforma puede integrarse en su actividad.

### 2.3 Oportunidades adicionales

- Ecosistema FP en crecimiento.
- Exigencia institucional de resultados de empleabilidad.
- IA accesible y barata para análisis documentales.
- Producto replicable a otras comunidades autónomas y etapas educativas.
- Base longitudinal de proyectos analizados (valor investigativo y de política pública), **con consentimiento** y limitada a medición y mejora del acompañamiento (no es una base central de ideas: ver §6, funcionalidades descartadas).

---

## 3. Objetivos del proyecto

| # | Objetivo |
|---|---|
| O1 | Convertir proyectos finales de FP en oportunidades evaluadas de autoempleo. |
| O2 | Reducir las barreras económicas, tecnológicas y burocráticas del emprendimiento. |
| O3 | Dar a conocer ayudas y trámites de forma comprensible y actualizada. |
| O4 | Producir un informe de viabilidad y una hoja de ruta accionables. |
| O5 | Crear una base de proyectos analizados que permita mejorar el acompañamiento y medir resultados. |

**Matiz sobre O5 (resolución de ambigüedad):** O5 se refiere a un registro longitudinal de los proyectos de los participantes de la plataforma, con fines de mejora del acompañamiento y medición de resultados, con consentimiento.

---

## 4. Usuarios objetivo y propuesta de valor

| Perfil | Necesidad principal | Momento de uso |
|---|---|---|
| **Alumno/a con proyecto** | Evaluar si su idea puede ser un negocio; saber pasos, costes y ayudas | Durante el proyecto |
| **Profesor/tutor** | Guiar a decenas de alumnos con criterios consistentes; priorizar acompañamiento | Todo el curso |
| **Coordinador/a de FP / centro** | Medir resultados, vincular proyectos a empleabilidad | Fin de curso |
| **Técnico de emprendimiento / incubadora** | Triaje de proyectos, informes previos a mentoría | Post-curso |
| **Institución pública** | Difundir ayudas, detectar vocaciones empresariales | Continuo |
| **Mentor/experto externo** | Contexto estructurado antes de revisar un proyecto | Puntual |

**Valor por colectivo:**

- **Alumno:** claridad sobre el potencial de su idea, plan con pasos concretos, acceso a ayudas desconocidas, estimación honesta del dinero necesario.
- **Centro:** estandarización del análisis de proyectos, evidencias de impacto, vinculación con el tejido empresarial local.
- **Administración:** canal eficaz de difusión de ayudas y detección temprana de proyectos viables.

---

## 5. Análisis de mercado y competencia

Alternativas actuales y limitaciones frente a EmprendeIA FP:

| Alternativa | Qué ofrece | Limitación | Qué añade EmprendeIA FP |
|---|---|---|---|
| Chatbots generales (ChatGPT, etc.) | Análisis conversacional | Sin contexto FP, sin fuentes verificables ni seguimiento, riesgo de datos inventados | Fuentes citadas, modelos económicos auditables, historial y continuidad |
| Asesoramiento presencial (incubadoras, cámaras, asociaciones) | Mentoría de calidad | Capacidad limitada; no llega a todo el alumnado | Triaje previo y cobertura masiva; complementa, no sustituye |
| Portales de ayudas (BDNS, webs autonómicas) | Información oficial | Volumen enorme, difícil de filtrar por proyecto | Filtrado automatizado por proyecto + revisión humana |
| Generadores de planes de negocio | Plantillas | Genéricos, sin ayuda ni financiación contextualizada | Plan generado a partir del proyecto real del alumno |

El **módulo A** de la plataforma (análisis de mercado, §6) aplica este análisis al proyecto concreto del alumno, distinguiendo dato/estimación/hipótesis.

---

## 6. Funcionalidades de la plataforma

### 6.1 Funcionalidades previstas (módulos)

| Módulo | Qué hace | Situación en MVP |
|---|---|---|
| A. Análisis de mercado | Potencial comercial, clientes potenciales, competencia, nichos, necesidades no cubiertas | Versión ligera con fuentes verificables (MVP) |
| B. Financiación y ayudas | Localiza subvenciones, requisitos, plazos, enlaces; financiación y programas de apoyo | Sí: BDNS + catálogos oficiales, con revisión humana |
| C. Necesidades tecnológicas | Hardware, software, cloud, inversión y mantenimiento | Versión básica: checklist + rangos de coste (MVP) |
| D. Viabilidad empresarial | Inversión, costes fijos/variables, ingresos, punto de equilibrio, escenarios | Sí, con modelo determinista de plantilla |
| E. Trámites administrativos | Autónomo/sociedad, fiscalidad, laboral, documentación, enlaces oficiales | Sí, guía estática revisada + disclaimer |
| F. Plan de lanzamiento | Hoja de ruta, hitos, plazos, seguimiento de tareas | Sí |

### 6.2 Funcionalidades complementarias (aplazadas a post-MVP)

- Inventario tecnológico completo (módulo C extendido) con alternativas según presupuesto.
- Alertas de nuevas convocatorias de ayudas relevantes.
- Repositorio documental del expediente del proyecto.
- Conexión con mentores/expertos (marketplace de asesoramiento).
- Integración con sedes electrónicas para iniciación de trámites *(depende de la disponibilidad real de APIs; no se da por hecho)*.
- Cuadro de indicadores para centros y administración.
- Análisis de mercado profundo (series temporales, tendencias sectoriales).

### 6.3 Funcionalidades expresamente descartadas (decisión aprobada del responsable del proyecto)

- **Bloque de empleabilidad tipo "Tinder"** (emparejamiento alumno-oferta).
- **Enlace emprendedor–centro** como canal propio de la plataforma.
- **Base de datos central entre alumnos para mejorar las ideas de empresa** (no se mezcla con el registro longitudinal propio del §3-O5, que sí está previsto).
- **Formación propia basada en el mercado laboral** dentro de la plataforma.

### 6.4 Simplificaciones justificadas (propuestas, coherentes con el alcance)

- **No** construir un buscador de mercado "en tiempo real" en el MVP: una versión ligera con fuentes seleccionadas cubre la mayor parte del valor.
- **No** automatizar la tramitación: explicar y enlazar es suficiente y reduce riesgo legal.
- **No** prometer cifras exactas de ayudas: solo fichas verificadas; el resto como hipótesis "pendiente de confirmar".
- **No** desarrollar el módulo C completo: la mayoría de proyectos de FP son de servicios o software; una checklist y rangos de coste bastan para decidir.

---

## 7. Recorridos de usuario y experiencia de uso

### 7.1 Perfiles y permisos

- **Alumno:** crea/edita su proyecto, recibe informes, sigue el plan.
- **Tutor:** ve proyectos de su grupo, comenta informes, valida datos.
- **Centro/admin:** configuraciones, métricas agregadas.
- **Revisor de contenidos (interno):** aprueba fichas de ayudas y trámites antes de publicarlas.
- **Invitado (futuro):** acceso a guías públicas.

### 7.2 Recorrido principal (entrada → proceso → resultado)

1. **Registro del proyecto.** *Entrada:* cuestionario (qué hace, para quién, fase, presupuesto, ubicación) + memoria del proyecto. *Proceso:* normalización y clasificación (sector, tecnología, fase). *Salida:* ficha de proyecto.
2. **Diálogo de aclaración.** La IA detecta lagunas y pregunta (p. ej., "¿cliente final o empresas?", "¿precio orientativo?"). *Salida:* ficha enriquecida con lagunas etiquetadas.
3. **Estudio de mercado.** *Proceso:* búsqueda en fuentes seleccionadas + síntesis. *Salida:* informe con clientes, competencia y nichos, con cada afirmación etiquetada como *dato (fuente, fecha)*, *estimación* o *hipótesis*.
4. **Necesidades tecnológicas y presupuesto.** Checklist derivada del tipo de proyecto + costes orientativos en rangos.
5. **Viabilidad.** El modelo determinista calcula inversión, costes, punto de equilibrio y tres escenarios con las variables aportadas. *Salida:* tabla y gráficos explicables.
6. **Ayudas y financiación.** Fichas de convocatorias relevantes (requisitos, plazos, organismo, enlace), priorizadas por probabilidad de encaje; aviso explícito de fichas sin verificar.
7. **Trámites.** Guía comparativa (autónomo vs SL, etc.) con documentación, plazos orientativos y enlaces oficiales.
8. **Plan personalizado.** Hoja de ruta secuenciada (validar → formalizar → ejecutar), hitos, plazos, recordatorios y estado de tareas.
9. **Continuidad.** El alumno vuelve, actualiza datos y el plan se recalcula; el tutor ve la evolución.

---

## 8. Alcance y prioridades del MVP

**Funcionalidades del MVP (orden de prioridad; los puntos 1-6 constituyen el núcleo):**

1. Registro/onboarding del proyecto + adjuntos.
2. Diálogo de aclaración con IA.
3. Motor económico determinista (inversión, costes, punto de equilibrio, escenarios).
4. Catálogo de ayudas con búsqueda filtrada y fichas verificadas.
5. Guía de trámites revisada (autónomo vs sociedad, fiscalidad, documentación).
6. Plan de lanzamiento con hitos y seguimiento.
7. Análisis de mercado ligero (competencia, nichos, fuentes citadas).
8. Roles alumno/tutor/admin y panel básico del tutor.
9. Módulo C tecnológico básico (checklist + rangos de coste).

**No entra en el MVP:** alertas de convocatorias, integraciones con sedes electrónicas, marketplace de mentores, repositorio documental avanzado, analytics.

**No alcance por definición:** tramitación automática ante administraciones, asesoramiento jurídico/fiscal individual, promesas de obtención de subvenciones, alertas en tiempo real, y las funcionalidades descartadas del §6.3.

---

## 9. Modelo de negocio

**Principio:** el acceso del alumnado debe ser **gratuito**. Quien paga es la institución o el servicio especializado.

| Vía | Ventajas | Inconvenientes | Barreras |
|---|---|---|---|
| Licencias anuales por centro | Ingresos previsibles; encaja con presupuesto educativo | Procurement lento; decisión colegial | Necesita pilotos y resultados |
| Acuerdos con instituciones públicas (JCCM, consejería, fondos europeos FSE/FEDER) | Escala y legitimidad; gratuidad para alumnos | Concurrencia pública, plazos | Dependencia de convocatorias |
| Suscripción premium (informes avanzados, mentores) | Monetización directa | Riesgo de percibir "pago por lo básico" | El público joven tiene poca disposición de pago |
| Servicios especializados (mentoría, revisión por expertos) | Alto valor añadido | No escalable sin red de profesionales | Gestión de calidad |
| Patrocinio/collaboración (banca, aseguradoras, grandes empresas) | Sin coste para usuarios | Conflictos de interés; imagen comercial | Requiere transparencia |
| **Modelo mixto (recomendado, aún por aprobar)** | Diversifica ingresos | Complejidad | — |

**Escalabilidad:** tras CLM, otras comunidades autónomas; el motor es común y el catálogo de ayudas se parametriza por territorio.

---

## 10. Arquitectura técnica

> **Advertencia: ninguna tecnología está aprobada.** Todo lo siguiente es una propuesta justificada sujeta a decisión del responsable (§19).

### 10.1 Principios de diseño

1. **Coste bajo y operación sencilla** antes que sofisticación (proyecto educativo con presupuesto incierto).
2. **Residencia y cumplimiento europeo** (RGPD/LOPDGDD): datos de alumnos, incluidos menores, en servidores de la UE.
3. **IA con trazabilidad:** toda afirmación externa con cita, URL y fecha; toda cifra con fórmula visible y etiqueta de confianza.
4. **Human-in-the-loop** para contenido crítico (ayudas, trámites, fiscalidad).
5. **Degradable:** si una fuente oficial deja de estar disponible, el sistema sigue funcionando con las restantes.
6. **MVP primero:** solo lo imprescindible.

### 10.2 Diagrama general (MVP propuesto)

```
                        ┌──────────────────────────────┐
                        │        Frontend web (SPA)    │
                        │  Next.js + componentes UI    │
                        └──────────────┬───────────────┘
                                       │ HTTPS
                        ┌──────────────┴───────────────┐
                        │      API Gateway (FastAPI)   │
                        │  Auth, RBAC, rate limiting   │
                        └──┬─────────┬─────────┬────────┘
                           │         │         │
              ┌────────────┴──┐  ┌───┴──────┐  ┌────────────────┐
              │ Motor de análisis│  │ Modelo  │  │ Catálogo de   │
              │ IA + orquestador│  │ económico│  │ ayudas/trámites│
              └────────┬────────┘  └──────────┘  └───────┬───────┘
                       │                                  │
              ┌────────┴────────┐                 ┌───────┴────────┐
              │ RAG: pgvector + │                 │ Ingesta/ETL    │
              │ corpus oficial  │                 │ (BDNS, BOE,    │
              └────────┬────────┘                 │  JCCM, INE…)   │
                       │                          └────────────────┘
              ┌────────┴────────┐
              │ PostgreSQL      │  + objetos (documentos) + cola (Redis/Celery)
              │ (relacional +   │  + registro de auditoría
              │  vectorial)     │
              └─────────────────┘
```

### 10.3 Componentes

| Componente | Función | MVP |
|---|---|---|
| Frontend SPA | Registro, informes, plan, dashboard | Sí |
| API + Auth | Usuarios, roles (alumno, tutor, admin, revisor), sesiones | Sí |
| Motor de análisis IA | Extracción, aclaración, síntesis con citas | Sí |
| Modelo económico | Cálculo determinista (inversión/costes/BEP/escenarios) | Sí |
| Catálogo de ayudas y trámites | Fichas curadas + importación; revisión humana | Sí |
| RAG | Búsqueda semántica sobre corpus normativo/oficial | Sí (versión mínima) |
| ETL/Ingesta | Actualización periódica de fuentes | Sí (manual + scripts) |
| Cola de tareas | Procesos largos (documentos, informes) | Sí |
| Repo documental | Adjuntos del proyecto, versiones | Sí |
| Notificaciones/recordatorios | Email o push del plan | Sí (básico) |
| Marketplace de mentores, integraciones e-gobierno, alertas, analytics avanzado | — | No (fase 5) |

### 10.4 Tecnologías propuestas y justificación (no por moda, sino por necesidad)

| Capa | Propuesta MVP | Justificación | Alternativa y cuándo considerarla |
|---|---|---|---|
| Frontend | Next.js (React) | SSR para guías públicas (SEO/alcance), ecosistema maduro, hiring fácil | Svelte o Angular si el equipo domina otro stack |
| Backend API | Python + FastAPI | El pipeline de IA/ETL es Python; un solo lenguaje reduce complejidad; tipado + OpenAPI | Node.js si el equipo es JS-only |
| Base de datos | PostgreSQL + pgvector | Una sola base cubre relacional y vectorial (RAG); open source, auditable | Vector DB dedicada (Qdrant) solo si el corpus crece mucho |
| IA generativa | LLM de nube en región UE (proveedor a decidir) + modelo local opcional (llama.cpp en GPU propia para prototipo/tareas internas) | Calidad para análisis documental; el local reduce coste y mejora privacidad en tareas no críticas | 100 % local si la normativa del organismo lo exige |
| Embeddings | Modelo abierto o del proveedor, tamaño modesto | Suficiente para corpus normativo en español | — |
| Documentos | Almacenamiento de objetos compatible S3 (UE) | Memorias de proyecto, adjuntos | Disco en VPS para MVP muy reducido |
| Cola | Redis + Celery | Simple, conocido | Workers de la plataforma cloud |
| Infraestructura | 1–2 contenedores Docker en VPS/cloud UE | Coste contenido para piloto | Kubernetes solo con >10.000 usuarios |
| Observabilidad | Logs estructurados + métricas básicas | Necesaria para auditoría | — |

**Imprescindibles para el MVP:** frontend, API, Postgres, auth, LLM, motor determinista, catálogo curado.
**Diferibles:** RAG avanzado, modelo local, integraciones, alertas, analytics.

### 10.5 Escalabilidad

- Motor agnóstico del territorio; catálogo parametrizado por comunidad autónoma.
- Cuello de botella real: la **curación de fuentes**, no la infraestructura.
- Multi-tenant por centro educativo desde el MVP (una organización = un tenant) para facilitar licencias.

---

## 11. Inteligencia artificial y procesamiento de datos

### 11.1 Pipeline de IA (propuesto)

1. **Ingesta y normalización:** parseo de la memoria del proyecto (PDF/docx) → JSON estructurado (idea, sector, cliente, tecnología, fase).
2. **Clarificación:** la IA genera preguntas sobre lagunas; el alumno responde.
3. **RAG:** consulta al corpus (normativa, guías de trámites, convocatorias verificadas) con citas.
4. **Síntesis etiquetada:** cada afirmación se marca como *dato (con fuente)*, *estimación (con fórmula y supuestos)* o *hipótesis (sin evidencia)*.
5. **Cálculo determinista:** el modelo económico se ejecuta con fórmulas explícitas (no generadas por el LLM); el LLM explica resultados.
6. **Revisión humana:** fichas de ayudas y trámites requieren aprobación de un revisor antes de mostrarse.
7. **Evaluación continua:** casos de prueba con respuestas esperadas; monitoreo de alucinaciones y fuentes rotas.

### 11.2 Qué puede automatizar la IA y qué requiere validación humana

| Decisión | IA | Humano |
|---|---|---|
| Extraer y estructurar información del proyecto | Sí | — |
| Detectar lagunas y generar preguntas | Sí | — |
| Clasificar sector/tecnología | Sí | spot-check opcional |
| Cálculos financieros (con fórmulas fijas) | Sí (ejecución) | revisión de metodología |
| Redactar informes y hojas de ruta | Sí | — |
| Fichas de ayudas concretas (importes, plazos) | Borrador | Revisión obligatoria antes de publicar |
| Conclusiones legales/fiscales | No | Revisión siempre |
| Determinar elegibilidad de una subvención | No | Sí (remite a organismo oficial) |
| Priorización de riesgos del proyecto | Sí (ayuda) | Sí (decisiones críticas) |

---

## 12. Relación con los contenidos del curso

El proyecto se apoya en los materiales del módulo **"Sistemas de Big Data"**. Es importante distinguir **los contenidos de los dos PDF de referencia** de las **prácticas de otros módulos** de la especialización.

### 12.1 Contenidos presentes en los PDF de referencia (`referencias/`)

*PDF 1 — "1 Introducción a Sistemas Big Data (SBD).pdf":* ficha de la asignatura (6 ECTS, 55 h, 2+1 h semanales), contenidos básicos (matemática discreta, lógica algorítmica, complejidad, extracción de información, modelado, análisis en tiempo real, costes y calidad del análisis), gestión y almacenamiento (sistemas de gestión; **Flume y Sqoop** como herramientas de importación; integración de datos; **R y Python**), visualización (datos no estructurados, IA en análisis de datos, clusters de máquinas), cuadros de mando y métricas, minería de datos y fases de los modelos; introducción a **Python** y **Google Colab**.

*PDF 2 — "2 Conceptos Básicos de Sistemas de Big Data.pdf":* complejidad computacional (P/NP, Big-O, escalabilidad), **divide y vencerás** (distribuido O(m)+O(K) frente a secuencial O(m·K)), proceso de extracción de información (identificación de datos, almacenamiento, analytics, machine learning, visualización), **tipología de datos** (estructurados, semi-estructurados, no estructurados), preparación de datos (depuración, criba, valores faltantes), modelos de datos (conceptual/lógico/físico, restricciones de integridad, operaciones I/O), ML por tipo (texto, imagen, audio, vídeo) y visualización/cuadro de mando.

### 12.2 Alineación con la arquitectura propuesta

| Concepto/tecnología del curso | Aplicación al proyecto | Decisión (propuesta) |
|---|---|---|
| **Python** (lenguaje del módulo) | Backend FastAPI, ETL, motor económico, scripts de ingesta | **Aprovechar**: refuerza la elección de FastAPI |
| Complejidad computacional (P/NP, Big-O) | Dimensionar pipelines y justificar que el MVP no necesita Spark/Hadoop (cientos de fichas, no terabytes) | Aprovechar como criterio de diseño |
| "Divide y vencerás" / procesado distribuido | Pipeline por módulos paralelizables (cola Celery, workers) | Aprovechar conceptualmente |
| Flume, Sqoop | Ingesta de fuentes oficiales | **No usar en MVP**: sobredimensionados; Python requests/pandas + API REST BDNS cubren la necesidad |
| R y Python | Análisis de datos | Python para análisis |
| Tipología de datos (estructurados/semi/no) | Diseño del modelo: fichas JSON (semi), memorias PDF (no), API BDNS (estructurado) | Aprovechar en el esquema de datos |
| Preparación de datos (depuración, criba, valores faltantes) | Normalización de fichas de ayudas y proyectos | Aprovechar |
| Modelos de datos conceptual/lógico/físico | Diseño de PostgreSQL (relacional) | Aprovechar; refuerza Postgres sobre NoSQL para el core |
| Cuadros de mando, métricas, visualización | Panel de seguimiento del alumno y dashboard de centro (módulo F) | Aprovechar (matplotlib/Chart.js) |
| Minería de datos y ML (clasificación, texto, imagen) | Futuro: clasificación de proyectos por sector, NER sobre memorias | Complementario (post-MVP) |
| Google Colab | Prototipado rápido en Fase 0 | Usable para prototipos; no para producción |

### 12.3 Prácticas de otros módulos de la especialización (no contenidas en los dos PDF)

Los materiales del módulo "Big data aplicado" y otras carpetas del curso incluyen prácticas con **Hadoop, MapReduce, Spark (lab docker-compose), NoSQL, ETL, OLAP, JSON y grafos/NER en Python**, y en otro módulo **TensorFlow.js/Teachable Machine**. Estas tecnologías **no se incorporan al MVP** (justificado por volumen y complejidad), pero son conocimiento disponible en el equipo formativo y candidato para fases futuras (p. ej., analítica avanzada o clasificación de proyectos).

**Conclusión:** la arquitectura propuesta (Python/FastAPI, PostgreSQL, Docker, pipelines de ingesta, dashboards) es coherente con la formación y permite al alumnado autor contribuir directamente. No se fuerzan Hadoop/Spark/Flume/Sqoop.

---

## 13. Seguridad, privacidad y RGPD

**Datos tratados:** identidad del alumno (nombre, contacto, edad), proyecto (memoria, datos económicos), progreso del plan, documentos adjuntos. Posibles **menores de edad** → requisitos reforzados.

**Medidas mínimas del MVP (propuestas):**

- Minimización: solo lo necesario para el análisis.
- Consentimiento informado explícito (y de padre/tutor legal cuando proceda).
- Residencia de datos en la UE; DPA con el proveedor LLM; **prohibición de entrenamiento con datos de usuarios**.
- Roles y permisos RBAC; aislamiento por proyecto.
- Cifrado en tránsito (TLS) y en reposo; contraseñas con hash fuerte.
- Retención definida: plazo acordado (propuesta: 2 años tras el fin de curso; **decisión pendiente**, con base legal a definir).
- Derechos RGPD atendibles (acceso, supresión, portabilidad) con proceso documentado.
- Registro de auditoría de accesos a datos económicos y documentos.
- No se almacenan credenciales de organismos públicos; si algún día se integran sedes electrónicas, esas credenciales nunca pasan por la plataforma.
- Designación de DPO (**pendiente**).
- **EIPD/DPIA** antes del pilotaje real con alumnos.

**Advertencia de contenido (requisito funcional, no cosmético):** la IA debe indicar siempre su nivel de confianza y enlazar a la fuente; nunca presentar estimaciones como hechos.

---

## 14. Fuentes oficiales e integraciones

> Regla: **no se asume ninguna API**. Cada fuente debe comprobarse antes de integrar.

| Fuente | Uso | Disponibilidad (consultado 03/11/2026) | Estado |
|---|---|---|---|
| **BOE** (legislación consolidada) | Normativa de FP, régimen de autónomos, fiscalidad | boe.es accesible; servicios de búsqueda existentes, pero **la API exacta y sus términos deben confirmarse** | Parcialmente verificada |
| **BDNS / Sistema Nacional de Publicidad de Subvenciones** | Convocatorias de ayudas | Portal accesible (subvenciones.gob.es); ficha oficial en datos.gob.es indica exportación CSV/XLS/PDF y **API REST en JSON**. El dominio `bdn.es` no resolvió (error TLS) | **Verificada**; pendiente probar la API y sus límites |
| **JCCM** (catálogo de trámites y ayudas CLM) | Ayudas autonómicas, trámites | Catálogo accesible (jccm.es), p. ej. `/tramites/1024256` (Proyectos de FP y empleo en la empresa) y `/tramites/1024336` (Premios al Mérito Empresarial 2026). Sin API oficial identificada; probable scraping | Parcialmente verificada |
| **Alta de autónomos y constitución de sociedades** | Canal real: TGSS/RETA (alta laboral), AEAT (alta censal) y Registro Mercantil/Registradores (sociedades) | Ninguna sede electrónica específica verificada en la revisión. **Aviso: dgt.es no es fuente válida** (es la Dirección General de Tráfico) | **Pendiente** |
| **INE** | Estadísticas sectoriales y de autoempleo | ine.es accesible; condiciones de uso por confirmar | Parcialmente verificada |
| **Registradores de España** | Formalización societaria | registradores.org accesible | Parcialmente verificada |
| **Kit Digital** | Ayudas de digitalización | Páginas oficiales en Red.es, Acelera pyme y kitdigital.red.es; el dominio histórico kitdigital.gob.es ya no resuelve. **Vigencia y requisitos 2026 sin confirmar** | Parcialmente verificada |
| **AEAT** | Obligaciones fiscales, alta censal | sede.agenciatributaria.gob.es accesible; páginas específicas y API sin confirmar | Parcialmente verificada |
| **TGSS** (seguridadsocial.gob.es), **Fundación Incyco**, **portal de datos abiertos JCCM** | Ayudas y obligaciones fiscales/laborales | No accesibles desde el entorno de análisis (DNS no resuelto o bloqueo) | **Pendientes** |

**Consecuencia de diseño:** el MVP funcionará con **catálogo curado + carga semiautomática** (revisor humano valida las fichas). La ingesta totalmente automática queda condicionada a la verificación de APIs y licencias.

---

## 15. Viabilidad económica y costes

**Costes tecnológicos estimados** (estimaciones orientativas, no hechos; deben contrastarse con tarifas reales del proveedor elegido — pendiente):

| Concepto | Piloto (≤200 usuarios) | Escalado (2.000–5.000 usuarios) |
|---|---|---|
| Infraestructura (VPS/cloud UE, backups) | 20–60 €/mes | 100–300 €/mes |
| LLM (tokens de análisis e informes) | 50–200 €/mes | 500–1.500 €/mes (mitigable con modelo local y caché) |
| Mantenimiento y operación | ~1 persona parcial | ~2 personas |
| Curación de fichas de ayudas | Trabajo humano periódico | Idem |

**Viabilidad del modelo de negocio:** evaluada en §9 (licencias por centro, acuerdos institucionales, servicios especializados, patrocinio; modelo mixto recomendado). El cuello de botella económico principal no es la infraestructura, sino el **coste humano de revisión** y la dependencia inicial de financiación pública/institucional.

---

## 16. Riesgos y limitaciones

### 16.1 Riesgos y mitigaciones

1. **Alucinación/obsolescencia de datos de ayudas** (crítico): una ficha incorrecta genera desconfianza y posibles daños. Mitigación: trazabilidad de fuentes + revisión humana + fecha de verificación visible.
2. **RGPD/privacidad**, con menores implicados: mitigación mediante minimización, consentimientos, DPO, residencia UE, DPIA.
3. **Desmotivación post-curso**: sin incentivos, el seguimiento abandona. Mitigación: integración curricular y recordatorios suaves.
4. **Sostenibilidad económica**: dependencia de subvenciones públicas. Mitigación: modelo mixto con licencias.
5. **Fuentes sin API**: el scraping puede romperse o no estar permitido. Mitigación: verificar condiciones de uso; diseño con fuentes degradables.
6. **Responsabilidad legal** por orientaciones incorrectas. Mitigación: disclaimers, revisión experta, seguros.
7. **División digital**: accesibilidad y competencia digital del alumnado.

### 16.2 Limitaciones estructurales del producto

- La plataforma ofrece **orientación informativa**, no asesoramiento jurídico, fiscal ni laboral.
- Varias fuentes oficiales todavía **pendientes de verificar** (§14); mientras no se confirmen, el catálogo de ayudas se limita a fichas revisadas manualmente.
- Las cifras económicas del informe son **estimaciones con supuestos** o hipótesis, nunca garantías.
- No existe todavía validación empírica de demanda (§17).

---

## 17. Plan de validación del MVP

**Estado:** planificación. **No se han realizado todavía entrevistas ni pruebas.** Todo lo siguiente es diseño de investigación, no resultados.

### 17.1 Hipótesis a comprobar (H1–H6)

| # | Hipótesis | Cómo se comprueba | Criterio de confirmación |
|---|---|---|---|
| H1 | Un porcentaje relevante de proyectos finales de FP tiene potencial empresarial real | Clasificación de 20–30 memorias de proyectos reales por un panel (tutor + técnico) | ≥30 % de proyectos con al menos una vía de monetización identificable *(umbral a consensuar con centros)* |
| H2 | La barrera principal es la falta de acompañamiento e información accionable, no la falta de ideas | Entrevistas a alumnos y tutores | ≥60 % de entrevistados citan "no saber qué ayudas existen" o "no saber qué pasos dar" |
| H3 | Los alumnos usarían la plataforma tras el curso si hay recordatorios y valor claro | Prototipo + encuesta de intención de uso | ≥40 % declararía volver en 3 meses *(indicador débil: confirmar con uso real en piloto)* |
| H4 | El módulo de ayudas es la funcionalidad de mayor valor | Ranking de funcionalidades en entrevistas | Ayudas y trámites entre las 2 funciones más valoradas |
| H5 | El análisis de mercado completo es prescindible en el MVP | Comparar versión ligera vs. completa en prototipo | La versión ligera resuelve las preguntas clave del usuario |
| H6 | Los tutores actuarían como revisores del contenido crítico | Entrevistas a docentes | Disponibilidad real de tiempo y perfil |

### 17.2 Entrevistas previstas

- **Alumnado (15–20 personas):** alumnado de cursos de especialización y FP con proyecto final en los últimos 2 años. Preguntas: ¿qué hizo con su proyecto?, ¿intentó comercializarlo?, ¿qué le frenó?, ¿buscó ayudas?, ¿cómo?, ¿qué le habría hecho falta? (15–20 min, consentimiento informado).
- **Docentes (5–8 personas):** tutores de proyectos finales / módulos de empresa. Preguntas: proyectos con potencial, preguntas repetidas, tiempo disponible para acompañar, confianza en herramientas IA, qué validaría un informe de viabilidad.
- **Técnicos de emprendimiento (3–5):** incubadoras, cámaras, entidades públicas. Preguntas: volumen de solicitudes, perfil, análisis exigidos, encaje de un triaje previo.

Cada entrevista se documenta con fecha, perfil (minimizando datos personales) y respuestas textuales, almacenadas en `referencias/entrevistas/` (carpetas futuras).

### 17.3 Centros candidatos para el piloto

Criterios (sin nombres concretos hasta confirmar contacto y autorización, para no dar por hecho disponibilidad):

- Centros de FP de Castilla-La Mancha con cursos de especialización y tutor interesado.
- 2–4 proyectos reales por centro.
- Implicación del tutor como revisor (1–2 h/mes estimadas, a confirmar).

La lista de centros debe obtenerse de fuentes oficiales de la Consejería de Educación y confirmarse con cada centro.

### 17.4 Prototipo de validación (sin código de producción)

1. Informe de viabilidad generado manualmente (con ayuda de IA) para 3 proyectos reales de alumnos.
2. Hoja de cálculo del modelo económico determinista (inversión, costes, BEP, escenarios).
3. Fichas de 10–20 ayudas verificadas a mano desde BDNS/JCCM con fuente y fecha.
4. Cuestionario de usabilidad y valoración (10 minutos).

### 17.5 Criterios GO / NO-GO

**GO (desarrollar):**

- ≥70 % de entrevistados consideran útiles al menos 2 de los 4 módulos prioritarios.
- Un centro dispuesto a participar en piloto con tutor comprometido.
- Las fichas de ayudas verificadas se pueden construir y mantener (flujo viable).
- Riesgo legal asumible con disclaimers y revisión humana previstos.

**NO-GO o reorientación:**

- Si el valor se concentra solo en el módulo de ayudas → MVP reducido a "ayudas + trámites + plan".
- Si no hay disponibilidad docente para revisar contenido → revisar el modelo (revisión centralizada o solo fuentes oficiales sin interpretación).
- Si los alumnos no retornan tras el curso en el prototipo → evaluar integración curricular obligatoria antes de invertir.

### 17.6 Resultados de la Fase 0 (a rellenar con evidencia real; prohibido rellenar con estimaciones)

- [ ] Entrevistas realizadas: … (fecha, nº)
- [ ] Hipótesis confirmadas/refutadas: …
- [ ] Funcionalidades priorizadas: …
- [ ] Centros confirmados: …
- [ ] Decisión go/no-go: …

---

## 18. Hoja de ruta

> Duraciones **estimativas** de planificación, no compromisos.

| Fase | Duración est. | Prioridad | Dependencias |
|---|---|---|---|
| 0. Investigación y validación | 4–8 semanas | Máxima | Ninguna |
| 1. Definición del MVP | 2–4 semanas | Máxima | F0 |
| 2. Desarrollo inicial | 3–6 meses | Alta | F1, decisiones técnicas aprobadas |
| 3. Pruebas y piloto | 2–3 meses | Alta | F2 |
| 4. Despliegue estable | 2–3 meses | Media | F3 + DPIA y seguridad |
| 5. Evolución futura | Continuo | Media | F4 + modelo de negocio validado |

**Fase 0 — Investigación y validación.** Entrevistas (según §17), análisis de alternativas, verificación de fuentes (§14: BDNS ya verificada; pendientes Kit Digital 2026, AEAT, BOE, INE, TGSS, Incyco, scraping JCCM), revisión legal preliminar (RGPD, menores, alcance del "no asesoramiento"), encuesta a centros piloto. *DoD:* ≥15 entrevistas analizadas; lista confirmada de fuentes utilizables con licencia/acceso documentado; informe de riesgos legales; decisión documentada sobre construir o reorientar el MVP. *Riesgo de la fase:* que el valor real esté solo en el módulo de ayudas; en ese caso el MVP se reduce a ayudas + trámites + plan.

**Fase 1 — Definición del MVP.** Wireframes, esquema de datos (ficha de proyecto, ficha de ayuda, etiquetas de confianza), selección definitiva de stack (pendiente: proveedor LLM, hosting, auth), prototipo no funcional, catálogo inicial de 30–50 fichas de ayudas/trámites CLM y estatales verificadas a mano con fecha, plan de medición (KPIs) y política de datos. *DoD:* alcance firmado; decisiones técnicas aprobadas y registradas; plantilla de informe validada por experto en negocios y jurista; KPIs definidos.

**Fase 2 — Desarrollo inicial (MVP funcional).** Funcionalidades priorizadas del §8. *DoD:* recorrido completo en <30 min; 100 % de fichas con fuente + fecha + revisión humana; informe que distingue visiblemente dato/estimación/hipótesis; cálculos reproducibles; regresión del pipeline con 20 casos de referencia.

**Fase 3 — Piloto.** 2–4 centros de FP de CLM (2–5 proyectos por centro), formación de tutores, feedback, ajuste de fichas y prompts, KPIs. *DoD:* ≥30 proyectos reales analizados; satisfacción tutor/alumno ≥ objetivo de F1; correcciones documentadas; decisión go/no-go de despliegue.

**Fase 4 — Despliegue estable.** DPIA, pentest básico, backups, monitorización, contratos (proveedores, DPA), soporte, continuidad de fuentes. *DoD:* producción con SLA razonable; proceso de actualización de fichas (≤2 revisiones/año por convocatoria o al detectar cambios); modelo de acceso aprobado.

**Fase 5 — Evolución (post-MVP), por prioridad:** alertas de convocatorias; inventario tecnológico completo (C extendido); analíticas para centros/administración; marketplace de mentores; integraciones con sedes electrónicas **solo si se verifican APIs y licencias**; extensión a otras comunidades; repositorio de conocimiento de proyectos (con consentimiento).

**Dependencias críticas transversales:**

- Sin fuentes verificadas no hay módulo B fiable → bloquea F2.
- Sin decisión de titularidad no hay política de datos → bloquea F1/F3.
- Sin presupuesto de LLM no se dimensiona la infraestructura → bloquea F2.
- La revisión humana es obligatoria desde F2: sin persona responsable de curar fichas, el producto no puede lanzarse.

---

## 19. Decisiones pendientes (requieren aprobación del responsable)

**Aprobadas hasta ahora (alcance):**
- Las funcionalidades descartadas del §6.3 (bloque tipo Tinder, enlace emprendedor–centro, base central de ideas, formación propia) están **descartadas**.
- El principio de gratuidad para el alumnado (§9).
- La obligatoriedad de human-in-the-loop y etiquetado de confianza (§11) como requisitos de producto.

**No aprobadas (pendientes):**

1. Nombre/marca definitiva (EmprendeIA FP es provisional).
2. Titularidad y modelo operativo: administración, fundación, empresa privada o consorcio.
3. Territorio piloto (CLM recomendado; centros concretos pendientes de confirmar).
4. Proveedor/modelo de IA principal y presupuesto de tokens (nube UE vs modelo local en prototipo).
5. Hosting y residencia de datos (cloud público UE vs infraestructura pública).
6. Modelo de autenticación del MVP (email + OAuth Google vs Clave/SSO de la administración).
7. Política de retención de datos (propuesta: 2 años post-curso) y designación de DPO.
8. Catálogo inicial de fuentes (tras verificar APIs/licencias de las fuentes "pendientes" del §14).
9. Financiación inicial y modelo de negocio definitivo (licencias vs acuerdo institucional).
10. Stack definitivo del MVP (todas las tecnologías del §10 son propuestas).
11. Destino del archivo heredado `generarMarkDown.py` (vacío, conservado sin tocar).

*Las decisiones aprobadas deben registrarse en un `DECISIONES.md` (aún no creado en el repositorio).*

---

## 20. Instrucciones y convenciones para agentes de IA

> Este documento es la **memoria única del proyecto**. Antes de tocar cualquier archivo, leerlo íntegramente. Si una tarea entra en conflicto con estas reglas, prevalece esta sección; cualquier excepción autorizada explícitamente por el responsable se documenta en `DECISIONES.md`.

### 20.1 Contexto

- Proyecto: **EmprendeIA FP** (provisional), documentado íntegramente en este archivo. Repositorio **público** en GitHub: <https://github.com/JuanTS/emprendeia-fp> (rama `main`). Ubicación de trabajo: `G:\Curso Esp. IA y Big Data\modulos\Sistema Big data\TAREA IA PARA  AUTOEMPLEO` (dos espacios antes de "AUTOEMPLEO"; no crear otra carpeta).
- Fase actual: **Fase 0 — definición y documentación**. No desarrollar la aplicación todavía.

### 20.2 Alcance funcional

- MVP: lo definido en §8. Complementario: §6.2. Descartado: §6.3.
- No ampliar el alcance sin propuesta previa y aprobación.

### 20.3 Estado de la arquitectura

- §10 y §11 son **propuestas no aprobadas**. Un agente **no puede** implementar, instalar dependencias ni elegir stack sin que la decisión esté registrada y aprobada en `DECISIONES.md`.

### 20.4 Convenciones de trabajo

1. **Idioma:** toda la documentación y comentarios en español.
2. **Git:** no hacer commits, pushes ni publicaciones sin autorización explícita del responsable.
3. **Documentación primero:** cualquier cambio de diseño se documenta antes de implementar.
4. **Trazabilidad de decisiones:** cada decisión relevante se añade a `DECISIONES.md` con fecha, autor y justificación; las propuestas no aprobadas se marcan como "propuesta".
5. **Fuentes externas:** toda afirmación sobre normativa, ayudas, plazos o importes debe incluir fuente oficial, enlace y **fecha de consulta**. Lo no verificado se etiqueta "pendiente de verificar". Nunca inventar cifras, subvenciones, convocatorias ni requisitos.
6. **Etiquetas de confianza obligatorias** en cualquier salida de IA: `dato`, `estimación`, `hipótesis`.
7. **No sobrescribir** archivos existentes sin leerlos antes. Conservar los originales markdown como historial y no eliminar `generarMarkDown.py` hasta decidir su finalidad.
8. Tareas de solo lectura no deben generar escrituras.

### 20.5 Restricciones

- No desarrollar la aplicación en esta fase.
- No instalar dependencias ni modificar configuraciones del sistema.
- No presuponer APIs de organismos públicos: verificar antes (§14).
- La plataforma da **orientación informativa**, no asesoramiento profesional: todo informe legal/fiscal/laboral incluye disclaimer y remisión a fuentes o profesionales.
- Datos de posibles menores: RGPD/LOPDGDD estrictos, minimización y consentimiento; no usar datos reales de alumnos para pruebas de modelos sin base legal.
- No presentar resultados de IA como hechos contrastados.
- El repositorio es **público** por decisión del responsable (03/11/2026): en GitHub solo se publican `README.md` y `EMPRENDIA_FP.md`. No subir a GitHub los PDF de la asignatura, los documentos originales ni el material interno. No exponer tokens ni credenciales.

### 20.6 Criterios de calidad

Un informe es válido si: (a) separa dato/estimación/hipótesis; (b) cita fuentes con fecha; (c) los cálculos son reproducibles; (d) las fichas de ayudas tienen revisión humana; (e) incluye disclaimer de no asesoramiento. Los cambios de contenido externo requieren re-verificación y actualización de fecha. Está prohibido contradecir este documento sin registrar la revisión en `DECISIONES.md`.

---

## 21. Referencias y bibliografía

### 21.1 Fuentes oficiales verificadas (acceso: 3 de noviembre de 2026)

- BOE — Real Decreto 1153/2021, de 28 de diciembre, por el que se establece el curso de especialización en Materiales compuestos en la industria aeroespacial y se fijan los aspectos básicos de su currículo: <https://www.boe.es/eli/es/rd/2021-12-28/1153> *(no regula con carácter general los cursos de especialización; el marco general queda **pendiente** de citar con la norma vigente)*
- Sistema Nacional de Publicidad de Subvenciones / BDNS: <https://www.subvenciones.gob.es/bdnstrans/GE/es/index> y ficha de datos abiertos con API REST JSON: <https://datos.gob.es/es/catalogo/e05250001-base-de-datos-nacional-de-subvenciones>
- Catálogo de trámites JCCM: <https://www.jccm.es/tramites/1024256> (Proyectos de FP y empleo en el seno de la empresa), <https://www.jccm.es/tramites/1024336> (Premios al Mérito Empresarial de CLM, MÉEM 2026)
- Kit Digital: <https://www.red.es/es/iniciativas/proyectos/kit-digital>, <https://www.acelerapyme.gob.es/kit-digital>, <https://kitdigital.red.es/> *(vigencia/requisitos 2026 pendientes de confirmar; kitdigital.gob.es ya no resuelve)*
- AEAT (sede electrónica): <https://sede.agenciatributaria.gob.es>
- Seguridad Social (TGSS/RETA) y AEAT: canal real para el alta de autónomos — **pendiente de verificar** su sede electrónica. *(No se cita dgt.es: corresponde a la Dirección General de Tráfico, no al ámbito laboral.)*
- INE: <https://www.ine.es>
- Colegios de Registradores de España: <https://www.registradores.org>

### 21.2 Fuentes pendientes de verificar (no accesibles desde el entorno de análisis el 03/11/2026)

- TGSS: <https://www.seguridadsocial.gob.es> (DNS no resuelto)
- Fundación Incyco: convocatorias actuales de becas/ayudas al autoempleo
- Portal de datos abiertos de la JCCM; APIs exactas de BOE y INE; condiciones de scraping de catálogos autonómicos

### 21.3 Material formativo de referencia (conservado en `referencias/`)

- `referencias/sbd1_introduccion.pdf` — "1 Introducción a Sistemas Big Data (SBD).pdf" (original intacto en la carpeta del módulo)
- `referencias/sbd2_conceptos_basicos.pdf` — "2 Conceptos Básicos de Sistemas de Big Data.pdf" (original intacto en la carpeta del módulo)

### 21.4 Documentos de origen consolidados en este archivo

- `README.md`, `IDEA_AUTOEMPLEO.md`, `ARQUITECTURA.md`, `ROADMAP.md`, `VALIDACION_MVP.md`, `Agent.md` (v0.2, 03/11/2026; `VALIDACION_MVP.md` en v0.1) — conservados en la carpeta del proyecto y en copia de seguridad.
