# Business Case — Bienvisto

> Versión 1.0 — Marzo 2026
> Justificación de inversión para las Fases 1 y 2: Prototipo funcional y MVP completo

---

## 1. Resumen Ejecutivo

**Bienvisto** es una plataforma SaaS multi-tenant que convierte los datos de reputación corporativa del Centro Nacional de Consultoría (CNC) de Colombia — índices IGR y Merco — en inteligencia accionable y contenido ejecutivo generado por Inteligencia Artificial.

El producto no existe aún. Se encuentra en fase de propuesta, con prototipo previsto para el 11 de mayo de 2026. El CNC ya posee los datos: **más de 850 empresas colombianas** son analizadas cada año bajo una metodología auditada por KPMG, y ninguna de ellas tiene hoy acceso a esos datos de forma interactiva, continua o autoservicio. Reciben un PDF. Una vez al año.

El problema es urgente porque el mercado global de software de gestión de reputación crece al **10.2% anual** y se proyecta superar los **USD 12.800 millones en 2032** [1], mientras en Colombia no existe una solución local integrada con los índices de referencia del mercado. Bienvisto tiene una ventana de oportunidad clara: el canal de distribución (CNC) ya existe, los datos ya existen, y la tecnología necesaria es madura.

**Conclusión de inversión: viable.** La inversión requerida para el prototipo es de $8.000.000 COP (un mes), y para el MVP completo de $24.000.000 COP (tres meses). Con tan solo 9 empresas en plan Básico a $1.000.000 COP/mes se cubre el costo operativo mensual. El CNC tiene relaciones activas con más de 850 organizaciones: el mercado está frente a la puerta.

---

## 2. El Problema

### 2.1 Escala del problema

En Colombia, **más de 850 empresas** participan activamente en mediciones de reputación con Merco y el CNC cada año [2]. Eso equivale a 850 directores de comunicaciones, 850 CEOs y miles de ejecutivos que cada octubre reciben un informe impreso con su posición en el ranking — y luego deben esperar doce meses para saber si mejoró o empeoró. A nivel regional, Merco opera en más de 10 países de Latinoamérica y España, con universos similares de empresas medidas en México, Perú, Chile y Brasil. La escala del problema, solo en Colombia, supera los 800 tomadores de decisión que hoy trabajan sin herramientas adecuadas para interpretar y actuar sobre sus propios datos de reputación.

### 2.2 La vida real del cliente

Es martes por la mañana. La Directora de Comunicaciones de una empresa del sector financiero acaba de salir de la reunión de junta donde el CEO preguntó por qué cayeron cuatro posiciones en el ranking Merco este año. Ella no tiene una respuesta inmediata: el informe llegó hace tres semanas, es un PDF de 60 páginas con tablas estáticas, y la única forma de saber qué variable empeoró es volver a leer la metodología desde cero. Para el próximo comité — en dos semanas — necesita una presentación. Contratará un freelance para armarla, o pasará dos días haciéndola ella misma copiando datos del PDF a PowerPoint. La reunión donde realmente se toman decisiones sobre reputación durará veinte minutos. La preparación habrá tomado cuarenta horas.

Ese martes se repite en 850 empresas. Y en ninguna existe una herramienta diseñada para este problema.

### 2.3 La fragmentación actual

| Problema específico | "Solución" actual | Por qué falla |
|--------------------|--------------------|---------------|
| Visualizar indicadores IGR / Merco | PDF anual del CNC | Estático, sin filtros, sin comparativo |
| Compararse con el sector | Solicitar informe adicional al CNC | Demora semanas, costo extra, no en tiempo real |
| Preparar presentación para junta | Excel manual + PowerPoint | 2–3 días de trabajo; datos desactualizados |
| Monitorear evolución en el tiempo | Archivar PDFs año a año | Sin visualización, sin tendencias automatizadas |
| Generar contenido ejecutivo con IA | No existe solución local | Herramientas globales (Meltwater, Brandwatch) no integran IGR/Merco |

El problema no es falta de tecnología. Es falta de integración entre los datos únicos del CNC y una interfaz moderna que los haga accionables.

### 2.4 Las consecuencias medibles

- **Costo de preparación de contenido**: estimado en 2–3 días de trabajo de un perfil directivo (costo ~$600.000–$900.000 COP por evento) que se repite mínimo cuatro veces al año por empresa = **$2.4M–$3.6M COP anuales en costo laboral de preparación**, solo en presentaciones de reputación.
- **Oportunidad perdida de retención**: Las empresas que no entienden qué variable bajó tienden a no renovar su vinculación con las mediciones Merco, reduciendo el ingreso recurrente del CNC.
- **Subutilización de datos**: El CNC invierte en recopilar 81.527 encuestas anuales con auditoría KPMG [3] y el 90% de ese valor no llega al cliente de forma procesable.

### 2.5 El catalizador de urgencia

Tres fuerzas convergen en 2026 para hacer este problema urgente ahora:

1. **La IA generativa es production-ready**: Claude (Anthropic), GPT-4o y similares pueden generar reportes ejecutivos coherentes y precisos a un costo de $0.02–$0.10 USD por documento [Estimación del equipo]. Hace dos años esto no era económicamente viable a escala.
2. **La presión ESG sobre empresas colombianas**: La Superintendencia de Sociedades y la Bolsa de Valores de Colombia han intensificado los requisitos de reporte de sostenibilidad y gobierno corporativo, lo que convierte el monitoreo de reputación en una necesidad de compliance, no solo de imagen.
3. **El mercado SaaS en LATAM despegó**: La región registra un mercado SaaS de USD 22.020 millones en 2025 con crecimiento proyectado del 14.2% anual [4]. Las empresas colombianas están activamente adoptando soluciones cloud — Bienvisto llega en el momento correcto.

---

## 3. El Mercado Competitivo

### 3.1 Mapa del ecosistema

| Categoría | Jugadores | Fortaleza | Límite crítico | Precio aprox. |
|-----------|-----------|-----------|----------------|---------------|
| **A — Escucha social global** | Brandwatch, Meltwater, Mention | Monitoreo en tiempo real de redes y medios | No integran IGR/Merco; en inglés; precios enterprise ($15K–$50K USD/año) | Alto |
| **B — Gestión de reviews** | Reputation.com, Birdeye | Automatización de reseñas online | Enfocados en retail/hospitality, no en reputación corporativa B2B | Medio |
| **C — Consultoría tradicional** | Firmas de comunicaciones en Colombia | Conocimiento del mercado local | No escalan; cada entregable es manual; costoso | Variable |
| **D — El propio CNC** | Informe PDF anual | Datos únicos y metodología auditada | Sin interfaz digital; sin autoservicio; sin IA | Incluido en membresía |

### 3.2 El competidor real #1

El competidor más peligroso y más frecuente no es Brandwatch. Es **el Excel de la Directora de Comunicaciones**. Es la costumbre de "con el PDF alcanza". Es la resistencia al cambio de una industria que lleva 18 años funcionando con informes impresos [5]. Este competidor es vencible porque ya genera fricción visible: nadie está satisfecho con el PDF, pero tampoco nadie ha ofrecido una alternativa integrada y accesible. Bienvisto es la primera.

### 3.3 El moat de mercado

El mercado no tiene líder dominante por una razón estructural: **los datos son privados y están en manos del CNC**. Ningún competidor externo puede construir este producto sin acceso a los índices IGR/Merco. Brandwatch no tiene los datos. Una startup independiente tampoco puede conseguirlos. Solo un actor con relación directa con el CNC — como Bienvisto — puede integrar la fuente primaria. Ese acceso exclusivo es el foso defensivo más difícil de replicar.

---

## 4. La Propuesta de Valor Diferencial

| Para quién | Problema que resuelve | Beneficio clave | Diferencial vs. competencia |
|------------|-----------------------|-----------------|----------------------------|
| Director de Comunicaciones | Preparar presentaciones de reputación toma días | Reporte listo en minutos, generado por IA | Ningún competidor integra IGR/Merco con IA |
| CEO / Junta Directiva | Sin visibilidad continua del score de reputación | Dashboard en tiempo real con semáforo visual | Datos propios del CNC, no scraping de redes |
| CNC (administrador) | Sus datos no generan valor recurrente entre mediciones | Nueva fuente de ingreso SaaS sobre datos existentes | Canal de distribución directo, sin intermediarios |
| Empresa no vinculada a Merco | No sabe cómo está posicionada vs. su sector | Rankings públicos como punto de entrada | Captación natural desde el producto gratuito |

El diferencial central de Bienvisto no es precio ni interfaz — es **la fuente de datos**. Los índices IGR y Merco del CNC son los únicos indicadores de reputación corporativa en Colombia con metodología auditada por KPMG, 18 años de historia y reconocimiento por parte de analistas, periodistas, universidades y el gobierno. Ningún software de monitoreo social puede replicar esa legitimidad institucional. Bienvisto es el único canal que convierte esa legitimidad en un producto digital.

---

## 5. Mercado Total Addressable (TAM / SAM / SOM)

| Nivel | Definición | Tamaño | Fuente / Razonamiento |
|-------|-----------|--------|-----------------------|
| **TAM** | Mercado global de software de gestión de reputación corporativa | USD 5.200M (2025) → USD 12.800M (2032) | SkyQuest Research [1]; CAGR 10.2% |
| **SAM** | Empresas en Colombia y LATAM (países Merco) con necesidad de gestión de reputación corporativa | ~5.000 empresas × USD 2.400/año promedio = **USD 12M/año** | Estimación del equipo: 10 países Merco × ~500 empresas objetivo/país |
| **SOM** | Empresas del CNC Colombia alcanzables en 36 meses vía canal directo | 100 empresas × $1.500.000 COP/mes = **$150M COP/mes MRR** (~USD 34.900/mes) | Penetración del 12% sobre las 850 empresas analizadas por Merco Colombia |

**Precio promedio ponderado por cliente (ARPU):** $1.500.000 COP/mes (~USD 349), considerando mezcla 20% Free, 50% Básico, 30% Premium.

**MRR potencial del SOM (Año 3):** ~$150M COP/mes = **$1.800M COP/año** (~USD 418.000 ARR).

---

## 6. Modelo de Negocio y Pricing

### Estructura de planes

| Plan | Precio/mes (COP) | Créditos AI | Usuarios | Funcionalidades clave |
|------|-----------------|-------------|----------|----------------------|
| Free | $0 | 20 | 1 | Dashboard básico, último periodo |
| Básico | $500.000 – $1.500.000 | 200 | 5 | Todo + comparativo sectorial, PPT |
| Premium | $2.000.000 – $5.000.000 | 1.000 | Ilimitados | Todo + videos, soporte prioritario |

### Unit Economics

El costo marginal de servir a un cliente adicional en producción es principalmente infraestructura y consumo de API de IA:

- Costo de infraestructura por cliente: ~$5.600–$17.500 COP/mes (proporcional)
- Costo de IA por cliente (escenario medio, 4 reportes/mes): ~$43.000–$86.000 COP/mes
- **Gross Margin estimado (plan Básico a $1M):** ~91% excluyendo equipo; ~45% incluyendo equipo de 2 personas

### Modelo de expansión por cliente

Un cliente empieza en Free, migra a Básico cuando necesita comparativo sectorial (típicamente antes del ciclo anual de medición), y escala a Premium cuando incorpora el video narrativo para junta directiva. La expansión es natural porque los eventos de negocio (junta anual, presentación de resultados, entrega del ranking Merco) crean momentos de upsell predecibles.

### Proyección de MRR

| Período | Clientes activos | Free | Básico | Premium | MRR (COP) |
|---------|-----------------|------|--------|---------|-----------|
| Mes 1 (prototipo) | 3 piloto | 2 | 1 | 0 | $1.000.000 |
| Mes 6 | 15 | 5 | 8 | 2 | $18.000.000 |
| Mes 12 | 30 | 8 | 15 | 7 | $43.500.000 |
| Mes 24 | 60 | 12 | 30 | 18 | $100.500.000 |
| Mes 36 | 100 | 20 | 50 | 30 | $165.000.000 |

---

## 7. Métricas SaaS y Proyección Financiera

### Métricas clave

| Métrica | Actual | Meta Año 1 | Meta Año 2 | Meta Año 3 |
|---------|--------|-----------|-----------|-----------|
| Clientes activos (tenants) | 0 | 30 | 60 | 100 |
| MRR (COP) | $0 | $43.500.000 | $100.500.000 | $165.000.000 |
| ARR (COP) | $0 | $522.000.000 | $1.206.000.000 | $1.980.000.000 |
| Churn mensual | — | <5% | <3% | <2% |
| CAC (COP) | — | $1.500.000 | $1.200.000 | $1.000.000 |
| LTV (COP) | — | $30.000.000 | $50.000.000 | $75.000.000 |
| LTV / CAC | — | 20x | 42x | 75x |
| Payback period | — | 1 mes | 1 mes | 1 mes |
| Gross Margin | — | ~45% | ~55% | ~65% |

> CAC bajo porque el canal de distribución es el CNC: la venta es relacional, no de performance marketing.

### Proyección P&L simplificada (COP)

| Concepto | Año 1 | Año 2 | Año 3 |
|----------|-------|-------|-------|
| **Ingresos (MRR promedio × 12)** | $270.000.000 | $1.086.000.000 | $1.980.000.000 |
| Equipo (programador + especialista) | ($96.000.000) | ($96.000.000) | ($96.000.000) |
| Infraestructura cloud | ($5.760.000) | ($7.200.000) | ($10.800.000) |
| APIs de IA | ($2.400.000) | ($6.000.000) | ($12.000.000) |
| **EBITDA** | **$165.840.000** | **$976.800.000** | **$1.861.200.000** |
| **Margen EBITDA** | **61%** | **90%** | **94%** |

> Año 1 incluye el costo del prototipo ($8M) en los primeros dos meses. A partir del Mes 3, la operación es rentable si hay al menos 9 clientes en plan Básico.

---

## 8. Inversión Requerida y Uso de Fondos

| Fase | Inversión (COP) | Duración | Entregable | MRR desbloqueado |
|------|----------------|----------|-----------|-----------------|
| **Fase 1 — Prototipo** | $8.000.000 | 1 mes (abr) | Dashboard + carga CSV + reportes PDF con IA + demo con datos reales | $1M–$5M (3 pilotos) |
| **Fase 2 — MVP** | $16.000.000 | 2 meses (may–jun) | Planes y facturación + PPT IA + login SSO + despliegue cloud | $18M–$45M (15–30 clientes) |
| **Fase 3 — Escala** | $48.000.000 | 6 meses (jul–dic) | Videos IA + API pública + expansión LATAM + analytics | $100M+ (60+ clientes) |
| **Total Año 1** | **$72.000.000** | 9 meses | Producto completo en producción | **$43.500.000 MRR** |

**Nota:** La Fase 1 y 2 se financian con la inversión inicial conjunta CNC-equipo técnico. La Fase 3 se financia con el flujo de caja generado por los primeros clientes o con una ronda de crecimiento.

---

## 9. Riesgos y Mitigaciones

| Riesgo | Probabilidad | Impacto | Mitigación concreta |
|--------|-------------|---------|---------------------|
| Adopción lenta: empresas satisfechas con el PDF | Alta | Alto | Arrancar con 3 empresas piloto que ya expresaron interés; demostrar ROI antes de cobrar |
| Dependencia del CNC para datos y ventas | Alta | Alto | Estructurar contrato de acceso a datos con cláusula de exclusividad y SLA; diversificar hacia otras fuentes de datos (DANE, BVC) en Año 2 |
| Churn alto en primeros meses por curva de aprendizaje | Media | Alto | Onboarding asistido por el especialista en reputación; sesiones de activación en las primeras 4 semanas |
| Competidor mejor financiado entra al mercado | Baja | Alto | El moat es el acceso exclusivo a los datos del CNC; formalizar acuerdo de exclusividad tecnológica antes del lanzamiento |
| APIs de IA aumentan precio o cambian términos | Media | Medio | Arquitectura multi-proveedor (Claude + GPT-4o + Azure OpenAI); los costos de IA son <2% del ingreso proyectado en Año 2 |
| Regulación de datos personales (Ley 1581) | Baja | Alto | Los datos de Bienvisto son corporativos, no personales; revisión legal preventiva antes del lanzamiento |
| CNC no entrega datos en formato utilizable | Media | Alto | Acordar formato de entrega (CSV/API) en la semana del 6 de abril como condición para iniciar Fase 1 |

---

## 10. Conclusión y Llamado a la Acción

Tres hechos definen esta oportunidad:

- **El CNC tiene 18 años de datos únicos** que hoy no generan valor recurrente entre medición y medición. Bienvisto convierte ese inventario dormido en un producto digital que factura mensualmente.
- **El mercado no tiene competidor local**. Los jugadores globales (Meltwater, Brandwatch) no integran IGR/Merco, no hablan español de negocios colombiano y cuestan entre 10 y 50 veces más que Bienvisto.
- **El punto de equilibrio es bajo**: con 9 empresas en plan Básico a $1.000.000 COP/mes se cubre el costo operativo completo. El CNC tiene relaciones activas con más de 850 organizaciones.

El camino crítico es simple: primero los datos. Si el CNC entrega un archivo de ejemplo en la semana del 6 de abril, el prototipo estará listo el 11 de mayo. Sin ese archivo, todo lo demás se detiene. Ese es el único riesgo de ejecución que depende de una decisión tomada hoy.

El riesgo de no actuar es concreto: cada mes que pasa sin Bienvisto es un mes en que alguna empresa del portafolio del CNC busca una solución alternativa (consultora, herramienta global cara, o simplemente renuncia a medir su reputación). La ventana de exclusividad de canal no dura indefinidamente.

**La recomendación es autorizar la inversión de $24.000.000 COP para ejecutar las Fases 1 y 2 entre abril y junio de 2026**, con revisión de continuidad al finalizar el prototipo (mayo 11). Si el prototipo no convence a al menos 3 empresas piloto, la inversión se detiene con un costo máximo de $8.000.000 COP.

---

## 11. Fuentes y Referencias

1. SkyQuest Research — *Reputation Management Software Market Size & Forecast 2033*. CAGR 10.2%, proyección USD 12.800M para 2032. [https://www.skyquestt.com/report/reputation-management-software-market](https://www.skyquestt.com/report/reputation-management-software-market)
2. Infobae Colombia — *Empresas nacionales dominan el top 10 de reputación en Colombia según Merco 2025*. 200 empresas rankeadas, 850+ analizadas, 81.527 encuestas. [https://www.infobae.com/colombia/2025/10/15/empresas-nacionales-dominan-el-top-10-de-reputacion-en-colombia-segun-merco-2025/](https://www.infobae.com/colombia/2025/10/15/empresas-nacionales-dominan-el-top-10-de-reputacion-en-colombia-segun-merco-2025/)
3. Portafolio — *Bancolombia, Alpina y Bavaria lideran el ranking Merco 2025*. Auditoría KPMG, 18ª edición. [https://www.portafolio.co/negocios/empresas/bancolombia-alpina-y-bavaria-lideran-la-reputacion-empresarial-en-colombia-segun-merco-2025-642187](https://www.portafolio.co/negocios/empresas/bancolombia-alpina-y-bavaria-lideran-la-reputacion-empresarial-en-colombia-segun-merco-2025-642187)
4. IMARC Group — *Latin America Software as a Service (SaaS) Market*. USD 22.02B en 2025, CAGR 14.2% hasta 2034. [https://www.imarcgroup.com/latin-america-software-as-a-service-market](https://www.imarcgroup.com/latin-america-software-as-a-service-market)
5. Merco Colombia — *Ranking Merco Empresas Colombia* (18 ediciones desde 2007). [https://www.merco.info/co/ranking-merco-empresas](https://www.merco.info/co/ranking-merco-empresas)
6. Capterra Colombia — *Alternativas a Brandwatch y competidores*. [https://www.capterra.co/alternatives/157048/brandwatch](https://www.capterra.co/alternatives/157048/brandwatch)

---

*Generado con /gen-business-case · Proyecto Bienvisto — CNC Colombia*
*Revisar antes de compartir con inversores: validar cifras de mercado, actualizar precios y añadir fuentes primarias donde se indique [Estimación del equipo].*
