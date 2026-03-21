# Propuesta Comercial y Técnica

## Plataforma Bienvisto
### Sistema Inteligente de Gestión de Reputación Corporativa

---

**Preparado para:** Centro Nacional de Consultoría (CNC)
**Fecha:** Marzo 2026
**Versión:** 1.0 — Borrador para revisión

---

## 1. Resumen Ejecutivo

**Bienvisto** es una plataforma SaaS que transforma los datos de reputación corporativa —como los índices Merco e IGR— en inteligencia accionable para las empresas.

La plataforma permite a las organizaciones:

- **Visualizar** su posición en rankings de reputación a través de dashboards interactivos.
- **Analizar** la evolución de sus indicadores en el tiempo y compararse con su sector.
- **Generar automáticamente** reportes ejecutivos, presentaciones y contenido multimedia mediante Inteligencia Artificial.

El modelo de negocio es **freemium**: las empresas acceden a sus datos básicos sin costo y pagan por la generación de contenido AI según el plan contratado.

**Bienvisto convierte los datos del CNC en un producto digital recurrente, escalable y de alto valor percibido para los clientes empresariales.**

---

## 2. Contexto y Oportunidad

### El problema

Las empresas colombianas que participan en mediciones de reputación como Merco reciben resultados en formatos estáticos (informes PDF, presentaciones genéricas). Para convertir esos datos en acciones concretas, necesitan:

- Contratar consultores que interpreten los resultados.
- Crear presentaciones internas manualmente.
- Hacer seguimiento temporal sin herramientas adecuadas.

Esto genera **fricción, costos adicionales y subutilización de los datos** que el CNC ya posee.

### La oportunidad

El CNC cuenta con una base de datos única en Colombia: indicadores de reputación, confianza, satisfacción y responsabilidad social de cientos de empresas, recopilados de manera rigurosa durante años.

Bienvisto convierte esa base de datos en una **plataforma digital de autoservicio** donde cada empresa puede:

1. Consultar sus indicadores en tiempo real.
2. Obtener análisis generados por IA en segundos (en lugar de semanas).
3. Descargar presentaciones listas para su junta directiva.

### Mercado objetivo

- **Primario:** Empresas que ya participan en mediciones Merco/IGR del CNC (cientos de empresas).
- **Secundario:** Empresas que quieran medir y gestionar su reputación pero aún no participan (oportunidad de captación).
- **Terciario:** Expansión a otros países donde Merco opera (México, Perú, Chile, Brasil, etc.).

---

## 3. Producto

### 3.1 Descripción general

Bienvisto es una aplicación web accesible desde cualquier navegador, con tres niveles de acceso:

| Rol | Acceso | Funcionalidades |
|-----|--------|-----------------|
| **Administrador CNC** | Panel de administración | Cargar datos, gestionar empresas, configurar indicadores, ver métricas de uso |
| **Empresa (cliente)** | Dashboard privado | Ver sus indicadores, generar contenido AI, descargar reportes, gestionar créditos |
| **Público** | Rankings abiertos | Consultar rankings generales de reputación (configurable) |

### 3.2 Funcionalidades principales

#### Dashboard de Reputación
- Visualización interactiva de indicadores IGR, Merco Empresas, Merco Talento, Merco Responsabilidad ESG, Merco Digital.
- Evolución temporal: gráficas de tendencia por periodo (trimestral, anual).
- Comparativo sectorial: posición de la empresa vs. promedio del sector.
- Score general de reputación: indicador consolidado con semáforo visual.

#### Generación de Contenido con IA
- **Reportes ejecutivos (PDF):** Análisis narrativo automatizado de los indicadores de la empresa, con gráficas, conclusiones y recomendaciones. Listo para presentar a junta directiva.
- **Presentaciones (PPT):** Diapositivas profesionales con los datos clave, generadas automáticamente. *(Fase 2)*
- **Videos narrativos:** Resúmenes en video con voz sintetizada y visualización de datos, estilo podcast ejecutivo. *(Fase 2)*

#### Sistema de Créditos
- Cada empresa recibe créditos mensuales según su plan.
- Cada generación de contenido consume créditos según su complejidad.
- Historial completo de uso y consumo.
- Recarga automática mensual.

#### Panel de Administración CNC
- Carga masiva de datos vía archivos CSV/Excel.
- Gestión de empresas clientes (crear, editar, asignar planes).
- Gestión de usuarios y roles.
- Configuración de indicadores (cuáles existen, cuáles son públicos).
- Métricas de uso de la plataforma.

### 3.3 Rankings públicos

Página web pública donde se pueden consultar los rankings generales de reputación. Configurable por el CNC:
- Qué indicadores se muestran públicamente.
- Si se muestra el ranking completo o solo el top N.
- Filtros por sector, tamaño de empresa, periodo.

Esto funciona como **herramienta de captación**: empresas que ven los rankings se interesan en tener su propio dashboard.

---

## 4. Modelo de Negocio

### 4.1 Planes propuestos

| Característica | Free | Básico | Premium |
|---------------|------|--------|---------|
| Dashboard de indicadores | ✅ | ✅ | ✅ |
| Evolución temporal | Último periodo | Todos | Todos |
| Comparativo sectorial | ❌ | ✅ | ✅ |
| Créditos AI / mes | 20 | 200 | 1.000 |
| Reportes PDF | ✅ (básico) | ✅ (detallado) | ✅ (detallado) |
| Presentaciones PPT | ❌ | ✅ | ✅ |
| Videos narrativos | ❌ | ❌ | ✅ |
| Usuarios por empresa | 1 | 5 | Ilimitados |
| Soporte | Documentación | Email | Prioritario |

### 4.2 Tabla de consumo de créditos

| Tipo de contenido | Créditos |
|-------------------|----------|
| Reporte PDF básico (resumen ejecutivo) | 10 |
| Reporte PDF detallado (análisis completo) | 25 |
| Presentación PPT (Fase 2) | 20 |
| Video corto — 2 a 3 minutos (Fase 2) | 100 |
| Video completo — 5 a 10 minutos (Fase 2) | 250 |

### 4.3 Precios sugeridos (por definir con CNC)

Los precios deben establecerse conjuntamente con el CNC considerando:
- El valor actual que cobran por informes de reputación.
- El costo marginal de la generación AI (ver sección de costos).
- El mercado objetivo y su disposición de pago.

**Rango sugerido como punto de partida:**

| Plan | Precio mensual sugerido (COP) |
|------|-------------------------------|
| Free | $0 |
| Básico | $500.000 — $1.500.000 |
| Premium | $2.000.000 — $5.000.000 |

*Nota: Estos valores son referenciales. El CNC define la estrategia de precios final.*

---

## 5. Arquitectura Técnica

### 5.1 Visión general

La plataforma se compone de tres servicios principales:

```
┌─────────────────────────────────────────────────────────┐
│                    BIENVISTO                            │
│                                                         │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐   │
│  │  Aplicación  │  │  Base de     │  │  Worker de   │   │
│  │  Web         │  │  Datos       │  │  IA          │   │
│  │  (Next.js)   │  │ (PostgreSQL) │  │  (Python)    │   │
│  │              │  │              │  │              │   │
│  │ • Dashboard  │  │ • Empresas   │  │ • Genera     │   │
│  │ • Admin CNC  │  │ • Usuarios   │  │   reportes   │   │
│  │ • Rankings   │  │ • Indicadores│  │   PDF        │   │
│  │ • API        │  │ • Contenido  │  │ • Llama a    │   │
│  │              │  │ • Créditos   │  │   modelo IA  │   │
│  └──────┬───────┘  └──────┬───────┘  └───────┬──────┘   │
│         │                 │                  │          │
│         └────────┬────────┘                  │          │
│                  │         ┌──────────────┐  │          │
│                  └─────────│    Redis     │──┘          │
│                            │ (Cola de     │             │
│                            │  tareas)     │             │
│                            └──────────────┘             │
└─────────────────────────────────────────────────────────┘
```

### 5.2 Componentes

| Componente | Tecnología | Función |
|-----------|-----------|---------|
| Aplicación web | Next.js 14 + TypeScript | Interfaz de usuario, API REST, autenticación |
| Interfaz visual | shadcn/ui + Tailwind CSS | Componentes de UI, gráficas, tablas |
| Base de datos | PostgreSQL | Almacenamiento persistente de todos los datos |
| ORM | Prisma | Acceso tipado a la base de datos, migraciones |
| Cola de tareas | Redis + BullMQ | Gestión de trabajos asíncronos de generación AI |
| Worker IA | Python + FastAPI | Procesamiento de solicitudes AI, generación de archivos |
| Autenticación | NextAuth.js v5 | Login, roles, sesiones |
| Gráficas | Recharts | Visualización de indicadores en el dashboard |

### 5.3 Flujo de generación de contenido AI

```
1. Empresa solicita "Generar reporte PDF"
           │
2. Se verifican créditos disponibles
           │
3. Se reservan créditos y se encola el trabajo
           │
4. El Worker Python toma el trabajo:
   a. Recopila datos de indicadores de la empresa
   b. Envía datos al modelo de IA con instrucciones
   c. IA genera análisis narrativo
   d. Se construye el PDF con gráficas y texto
   e. Se almacena el archivo
           │
5. Se notifica a la empresa que el reporte está listo
           │
6. Empresa descarga el PDF
```

**Tiempo estimado de generación:** 30 segundos a 2 minutos por reporte.

### 5.4 Seguridad

- **Multi-tenancy estricto:** Cada empresa solo accede a sus propios datos. Validación en cada consulta a base de datos.
- **Autenticación con roles:** SUPER_ADMIN (CNC), ORG_ADMIN (empresa), ORG_VIEWER (usuario de empresa).
- **Variables de entorno:** Ningún secreto en el código fuente.
- **Validación de inputs:** En cada endpoint de la API.
- **HTTPS:** Cifrado en tránsito para todas las comunicaciones.

### 5.5 Modelo de datos simplificado

```
Organización (empresa)
├── nombre, sector, plan, créditos
├── Usuarios (N)
│   └── email, rol, nombre
├── Valores de Indicadores (N)
│   └── indicador, periodo, valor, ranking
├── Contenido Generado (N)
│   └── tipo, estado, archivo, créditos usados
└── Transacciones de Créditos (N)
    └── cantidad, razón, fecha

Indicador (definición global)
├── código, nombre, categoría, unidad
└── visible en rankings públicos (sí/no)
```

---

## 6. Plan de Implementación

### Fase 1 — Prototipo funcional (4 semanas)

**Objetivo:** Demostrar el concepto con datos reales del CNC.

| Semana | Entregable |
|--------|-----------|
| 1 | Infraestructura base: autenticación, multi-tenancy, layout del dashboard, CRUD de empresas y usuarios |
| 2 | Carga de datos CSV/Excel, dashboard con gráficas de indicadores, comparativo temporal |
| 3 | Generación de reportes PDF con IA, sistema de créditos, cola de procesamiento asíncrono |
| 4 | Rankings públicos, empaquetado con Docker, datos de prueba, documentación |

**Resultado:** Plataforma funcional que se puede demostrar a clientes potenciales con datos reales.

### Fase 2 — MVP completo (8 semanas adicionales)

- Generación de presentaciones PPT editables.
- Generación de videos narrativos con voz sintetizada.
- Sistema de planes y facturación.
- Login con Google/Microsoft (SSO).
- Notificaciones por email.
- Despliegue en la nube (Azure o AWS).

### Fase 3 — Producción y escala

- API pública para integraciones.
- Dashboard público elaborado con filtros.
- Soporte multi-idioma.
- Analytics de uso de la plataforma.
- Expansión a otros países (Merco opera en Latam y Europa).

---

## 7. Estimación de Costos

### 7.1 Costos de desarrollo

| Concepto | Costo mensual (COP) | Notas |
|----------|---------------------|-------|
| Programador | $4.000.000 | Desarrollo y mantenimiento |
| **Total desarrollo** | **$4.000.000/mes** | |

**Costo del prototipo (Fase 1):** $4.000.000 (1 mes)
**Costo del MVP completo (Fase 1 + 2):** $12.000.000 (3 meses)

### 7.2 Costos de infraestructura (producción)

| Servicio | Costo mensual estimado (USD) | COP estimado* |
|----------|------------------------------|---------------|
| Servidor aplicación (Azure App Service / AWS EC2) | $30 — $80 | $130.000 — $340.000 |
| Base de datos PostgreSQL (Azure/AWS managed) | $15 — $50 | $65.000 — $215.000 |
| Redis (Azure Cache / AWS ElastiCache) | $15 — $55 | $65.000 — $235.000 |
| Almacenamiento de archivos (Blob/S3) | $5 — $20 | $22.000 — $86.000 |
| **Subtotal infraestructura** | **$65 — $205** | **$280.000 — $876.000** |

*\*TRM referencial: $4.300 COP/USD. Sujeto a variación.*

**Durante el prototipo:** $0 (ejecución local).

### 7.3 Costos de APIs de IA

El costo depende del proveedor y el volumen de uso:

| Proveedor | Costo por reporte PDF estimado (USD) | Notas |
|-----------|--------------------------------------|-------|
| Claude (Anthropic) | $0.02 — $0.10 | Según longitud del análisis |
| OpenAI (GPT-4o) | $0.02 — $0.08 | Similar rango |
| Azure OpenAI | $0.02 — $0.08 | Mismos modelos, facturación Azure |

**Escenario de uso mensual:**

| Escenario | Reportes/mes | Costo IA/mes (USD) | COP estimado |
|-----------|-------------|---------------------|--------------|
| Bajo (50 empresas, 2 reportes c/u) | 100 | $2 — $10 | $9.000 — $43.000 |
| Medio (150 empresas, 4 reportes c/u) | 600 | $12 — $60 | $52.000 — $258.000 |
| Alto (300 empresas, 8 reportes c/u) | 2.400 | $48 — $240 | $206.000 — $1.032.000 |

**Nota:** Los costos de IA para video (Fase 2) serán significativamente mayores por el componente de síntesis de voz (TTS). Se estimarán cuando se defina el proveedor de TTS.

### 7.4 Resumen de costos mensuales en producción

| Concepto | Escenario conservador (COP) | Escenario medio (COP) |
|----------|---------------------------|----------------------|
| Programador | $4.000.000 | $4.000.000 |
| Infraestructura cloud | $280.000 | $600.000 |
| APIs de IA | $43.000 | $258.000 |
| **Total mensual** | **$4.323.000** | **$4.858.000** |

### 7.5 Punto de equilibrio estimado

Con el costo operativo mensual de ~$4.500.000 a $5.000.000:

| Si el plan Básico cuesta | Empresas necesarias para cubrir costos |
|--------------------------|----------------------------------------|
| $500.000/mes | 10 empresas |
| $1.000.000/mes | 5 empresas |
| $1.500.000/mes | 4 empresas |

*Sin contar empresas en plan Free ni Premium. El punto de equilibrio es alcanzable con una fracción mínima del mercado del CNC.*

---

## 8. Propuesta de Valor para el CNC

### ¿Por qué Bienvisto?

1. **Monetización de datos existentes:** Los datos de Merco/IGR que el CNC ya recopila se convierten en un producto digital recurrente.

2. **Diferenciación competitiva:** Ningún otro proveedor de rankings de reputación en Colombia ofrece una plataforma de autoservicio con generación AI.

3. **Escalabilidad:** Una vez construida, la plataforma puede atender 10 o 1.000 empresas con el mismo equipo.

4. **Retención de clientes:** Las empresas que usan la plataforma regularmente tienen más razones para seguir participando en las mediciones del CNC.

5. **Expansión geográfica:** Merco opera en múltiples países. Bienvisto puede replicarse sin cambios significativos.

### Modelo de asociación sugerido

- **CNC aporta:** Datos, marca, relación comercial con clientes, validación metodológica.
- **Equipo técnico aporta:** Desarrollo, mantenimiento, infraestructura tecnológica.
- **Esquema de ingresos:** A definir conjuntamente (licenciamiento, revenue share, o modelo mixto).

---

## 9. Próximos Pasos

| Paso | Responsable | Fecha estimada |
|------|-------------|----------------|
| Revisión y aprobación de esta propuesta | CNC + Equipo técnico | Semana del 23 de marzo |
| Entrega de archivo de datos de ejemplo (Merco/IGR) | CNC | Semana del 23 de marzo |
| Definición de precios por plan | CNC | Semana del 30 de marzo |
| Entrega del prototipo funcional | Equipo técnico | 20 de abril de 2026 |
| Demostración a clientes piloto | CNC + Equipo técnico | Semana del 27 de abril |

---

## 10. Anexo: Indicadores Soportados (Configurables)

La plataforma está diseñada para soportar cualquier indicador que el CNC defina. Ejemplos iniciales basados en Merco:

| Indicador | Categoría | Descripción |
|-----------|-----------|-------------|
| Merco Empresas | Reputación | Ranking general de reputación corporativa |
| Merco Líderes | Reputación | Ranking de líderes empresariales |
| Merco Talento | Talento | Capacidad de atraer y retener talento |
| Merco Responsabilidad ESG | Sostenibilidad | Responsabilidad social, ambiental y de gobernanza |
| Merco Digital | Digital | Reputación y presencia digital |
| IGR General | Gestión | Índice de Gestión de la Reputación (CNC) |
| Índice de Satisfacción | Satisfacción | Satisfacción del cliente/ciudadano |

*El CNC puede agregar, modificar o eliminar indicadores desde el panel de administración sin necesidad de cambios en el código.*

---

**Documento preparado por el equipo de desarrollo de Bienvisto.**
**Marzo 2026 — Versión 1.0**
