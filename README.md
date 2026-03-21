# Bienvisto

**Sistema Inteligente de Gestión de Reputación Corporativa**

Plataforma SaaS multi-tenant que convierte los datos de reputación del [Centro Nacional de Consultoría (CNC)](https://www.cnccolombia.com) — índices IGR y Merco — en inteligencia accionable para empresas colombianas.

---

## ¿Qué es Bienvisto?

Bienvisto permite a las empresas:

- **Visualizar** su posición en rankings de reputación (IGR, Merco Empresas, Talento, ESG, Digital) a través de dashboards interactivos.
- **Analizar** la evolución de sus indicadores en el tiempo y compararse con su sector.
- **Generar automáticamente** reportes ejecutivos, presentaciones y videos narrativos mediante Inteligencia Artificial.

El modelo es **freemium**: acceso básico sin costo, generación de contenido AI por créditos según el plan contratado.

---

## Documentación

| Documento | Descripción |
|-----------|-------------|
| [Business Case](docs/negocio-business-case.md) | Justificación de inversión: mercado, financieros, riesgos y retorno proyectado |
| [Propuesta Comercial y Técnica](docs/propuesta-bienvisto-cnc.md) | Propuesta completa para el CNC: producto, arquitectura, modelo de negocio, costos y cronograma |
| [Presentación interactiva](docs/bienvisto-propuesta.html) | Pitch deck HTML — abrir en navegador |
| [Guía de identidad visual](docs/brand/brand-guide.md) | Paleta de colores, tipografía, logo y componentes de UI |

---

## Stack tecnológico previsto

| Capa | Tecnología |
|------|-----------|
| Frontend / API | Next.js 14 + TypeScript |
| UI | shadcn/ui + Tailwind CSS |
| Base de datos | PostgreSQL + Prisma |
| Cola de tareas | Redis + BullMQ |
| Worker IA | Python + FastAPI |
| Autenticación | NextAuth.js v5 |

---

## Cronograma

| Fecha | Hito |
|-------|------|
| 6 abr 2026 | Revisión y aprobación de propuesta · Entrega de datos de ejemplo |
| 13 abr 2026 | Definición de precios por plan |
| 11 may 2026 | Prototipo funcional (Fase 1) |
| 18 may 2026 | Demostración a clientes piloto |

---

## Partes involucradas

- **CNC Colombia** — Datos, marca, relación comercial con clientes empresariales
- **Equipo técnico** — Desarrollo, infraestructura y mantenimiento de la plataforma
