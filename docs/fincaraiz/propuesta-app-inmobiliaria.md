# Propuesta: App Inmobiliaria con Escaneo de Letreros y Servicios Integrados

**Version**: Borrador 1.0
**Fecha**: 2026-03-21
**Estado**: En revision

---

## 1. Resumen Ejecutivo

Proponemos una app movil que digitaliza el mercado inmobiliario informal en Colombia mediante dos mecanismos complementarios:

1. **Codigos QR dinamicos** para letreros inmobiliarios (iteracion primaria)
2. **Escaneo OCR de letreros existentes** + contacto automatico por WhatsApp

La app captura un mercado invisible: las propiedades que solo tienen letrero fisico y nunca se publican en portales digitales. En Colombia, el 57% de los contratos de arriendo son verbales, 7.3 millones de hogares viven en arriendo, y el mercado de arriendos mueve ~$60 billones COP anuales. Ninguna plataforma existente atiende este segmento de manera efectiva.

La propuesta integra servicios de valor agregado: verificacion de arrendatarios/compradores, seguros de arrendamiento, generacion de contratos digitales, estimacion de precios y confirmacion de disponibilidad en tiempo real.

---

## 2. Problema y Oportunidad

### 2.1 El problema

| Problema | Dato |
|----------|------|
| Informalidad masiva | 57% de contratos de arriendo son verbales |
| Mercado invisible | Miles de propiedades solo tienen letrero fisico, sin presencia digital |
| Fraude creciente | +35% en denuncias de estafas por arriendos en un ano |
| Anuncios fantasma | Alta tasa de listings desactualizados en portales existentes |
| Sin verificacion | No existe sistema de reputacion para arrendatarios ni arrendadores |
| Brecha digital-transaccional | 92% busca online pero la mayoria cierra informalmente |

### 2.2 La oportunidad

- **Mercado de arriendos**: $60 billones COP/ano, 7.3M hogares (mayor que compraventa: $51.2B)
- **Por primera vez** hay mas hogares en arriendo (7.3M) que en vivienda propia (7.1M)
- **71%** de busquedas en FincaRaiz son para arriendo
- **Vacio de mercado confirmado**: no existe ninguna app que fotografíe letreros fisicos y extraiga datos automaticamente
- **Competencia no enfocada**: Habi (compraventa usada), La Haus (vivienda nueva), FincaRaiz/Metrocuadrado (clasificados). Ninguno atiende el arriendo informal

---

## 3. Solucion Propuesta

### 3.1 Concepto central

Una app movil con tres pilares:

**Pilar 1 — QR Dinamicos (Iteracion primaria)**
Inspirado en Scan A Sign (UK). El propietario/inmobiliaria genera un codigo QR desde la app y lo pega en su letrero. El interesado escanea el QR y accede a ficha completa del inmueble: fotos, precio, contacto, historial de zona, estimacion de valor.

- **Ventaja**: El propietario controla la informacion y la mantiene actualizada
- **Ventaja**: Se elimina el problema de datos desactualizados (el QR apunta a datos en vivo)
- **Dato de mercado**: El mercado global de QR alcanza $13.04 mil millones en 2025, con 41.77M de escaneos y conversion de hasta 13.6% de escaneos a leads

**Pilar 2 — Escaneo OCR + WhatsApp Automatico**
El usuario toma foto de un letrero existente de "Se Arrienda/Se Vende". La app:
1. Extrae texto via OCR (telefono, precio, tipo, direccion)
2. Genera automaticamente un deep link de WhatsApp con mensaje pre-formateado
3. El usuario toca "Contactar por WhatsApp" y se abre WA con el mensaje listo
4. Si el numero ya existe en la base de datos, trae la informacion historica y solicita precio actualizado
5. Las respuestas del propietario se pueden convertir en datos estructurados para la app

**Pilar 3 — Servicios de Valor Agregado**
- Verificacion de arrendatarios y compradores
- Seguros de arrendamiento integrados
- Generacion de contratos digitales con firma electronica
- Estimacion de precios por zona
- Confirmacion de disponibilidad en tiempo real

### 3.2 Diferenciadores vs. competencia

| Competidor | Que hace | Que NO hace (nuestra oportunidad) |
|------------|----------|-----------------------------------|
| FincaRaiz | Clasificados online (370K propiedades) | No captura mercado informal, no verifica, anuncios desactualizados |
| Metrocuadrado | Clasificados + contenido editorial | No genera contratos, no ofrece seguros, no escanea letreros |
| Habi | Compra directa vivienda usada + credito | No cubre arriendos, no atiende mercado informal |
| La Haus | Marketplace vivienda nueva + IA | No cubre usada ni arriendos |
| Ciencuadras | Ecosistema Grupo Bolivar (credito+seguro) | Limitado a su ecosistema financiero |
| DealMachine (EE.UU.) | "Driving for Dollars" para inversores | Solo EE.UU., enfocado en deterioro, no arriendos |

**Nuestra ventaja defensible**: La base de datos de inventario inmobiliario informal — propiedades que no existen en ningun portal digital — es un activo unico. Cada foto y QR subido hace la plataforma mas valiosa y mas dificil de replicar (efecto de red tipo Waze).

---

## 4. Funcionalidades por Fase

### Fase 1 — MVP (Meses 0-6)

**4.1 Generador de QR Dinamicos**
- Propietario crea ficha del inmueble en la app (fotos, precio, tipo, metros, contacto)
- App genera QR unico vinculado a esa ficha
- QR descargable/imprimible para pegar en el letrero fisico
- Interesado escanea QR → ve ficha completa → contacta por WhatsApp o dentro de la app

**4.2 Escaneo de Letreros con OCR**
- Foto del letrero → OCR extrae texto (telefono, precio, tipo, direccion)
- Pipeline: Claude Haiku directo para MVP (extraccion + estructuracion en una llamada)
- Costo estimado: ~$2.60/mes para 1,000 imagenes
- Geolocalización automatica del letrero

**4.3 Contacto por WhatsApp Automatico**
- Deep link `wa.me/{telefono}?text={mensaje}` — gratis, sin API
- Mensaje pre-formateado: "Hola, vi su letrero de arriendo en [direccion]. ¿El inmueble aun esta disponible?"
- Si el numero ya esta en base de datos, muestra historial y solicita precio actualizado
- El usuario decide si envia o no (no es spam)

**4.4 Mapa de Propiedades**
- Geolocalizar cada letrero escaneado y cada QR generado en un mapa interactivo
- Filtros: zona, precio, tipo (arriendo/venta), habitaciones
- Indicador de frescura: "Confirmado hace 2 dias" vs "Sin confirmar hace 30 dias"

**4.5 Confirmacion de Disponibilidad**
- Vencimiento escalonado: 15 dias activo, renovacion con 1 tap, archivado a los 60 dias
- Notificacion push con respuesta rapida: "¿Sigue disponible? [Si] [Ya no]"
- Crowdsourcing: usuarios reportan si un letrero ya no existe, ganando puntos
- WhatsApp de confirmacion periodica (cada 14 dias, modelo Zillow adaptado)

### Fase 2 — Crecimiento (Meses 6-12)

**4.6 Verificacion de Arrendatarios (Vital)**
Integracion con centrales de riesgo y servicios de antecedentes:

| Proveedor | Servicio | Datos |
|-----------|----------|-------|
| DataCredito (Experian) via Apitude | Score crediticio + historial de pagos | Puntaje 150-950, cuentas, comportamiento de pago |
| TusDatos.co | Antecedentes penales, legales, identidad | Listas de buscados, afiliaciones, validacion |
| TransUnion Colombia | Score + Legal Check | Historial, antecedentes judiciales, PEPs, listas OFAC |

- **Flujo**: Arrendatario autoriza consulta → app genera reporte consolidado → arrendador recibe resultado
- **Costo del estudio**: $50K-$150K COP. El costo es una barrera de adopcion significativa — solución: **estudio de credito incluido gratis** cuando el arrendador contrate una poliza de arrendamiento a traves de CazaRaiz. La aseguradora asume el costo del estudio como parte de su proceso de underwriting.
  - Modelo: CazaRaiz integra el estudio como parte del flujo de contratacion del seguro
  - Incentivo para el arrendador: 0 costo extra por verificacion + poliza en el mismo flujo
  - Incentivo para la aseguradora: leads calificados con datos completos del arrendatario
  - Resultado: conversion mas alta en seguros + diferenciador vs FincaRaiz/Metrocuadrado
- **Requisito legal**: Autorizacion expresa del titular (Ley 1266/2008)

**4.7 Verificacion para Compradores**
TransUnion Colombia ofrece "Seamless Onboarding" (API unificada de identidad + fraude + credito):
- Score crediticio del comprador
- Legal Check (antecedentes judiciales, listas restrictivas, PEPs)
- Verificacion de identidad
- Util para constructoras, inmobiliarias y vendedores particulares

**4.8 Seguros de Arrendamiento Integrados**
El mercado colombiano ofrece multiples opciones de polizas:

| Aseguradora | Producto | Cobertura | Costo tipico |
|-------------|----------|-----------|--------------|
| SURA | Digital + Tradicional | Canon, admin, servicios, asistencia | ~50% de un canon/ano |
| MAPFRE | Individual / Light | Canon, admin, servicios | ~50% de un canon/ano |
| Zurich | Zuarriendo | 100% canon, admin, servicios, incendio | Tasa ~2.97% anual |
| Seguros Bolivar | Via El Libertador | Canon, admin, servicios | Variable |

- **Modelo**: Actuar como intermediario/comparador de polizas
- **Diferenciador**: Ningun portal ofrece comparacion entre aseguradoras
- **Partnership prioritario**: SURA (lider en digitalizacion, ya tiene alianza con Aptuno)
- **Tendencia**: Modelos sin codeudor (SURA Digital, Aptuno)

**4.9 Estimador de Precios por Zona**
- Rango de precio basado en zona + tipo + tamano usando datos recolectados
- **Alianza estrategica con Habi**: Usar su API/Habimetro como proveedor de datos de valuacion
  - Habi tiene 10M+ propiedades en su base, 24K avaluos mensuales (95% automatizados)
  - Modelo de socio estrategico dado su enfoque en compraventa (complementario a nuestro foco en arriendos)
- Datos catastrales abiertos via IGAC Geoportal (formato GeoJSON/Shapefile)

**4.10 Alertas de Nuevos Inmuebles**
- Notificar cuando aparezca un inmueble en zona de interes del usuario
- Configuracion por zona, rango de precio, tipo de inmueble

### Fase 3 — Expansion (Meses 12-24)

**4.11 Generacion de Contratos Digitales**
Los contratos de arriendo digitales tienen **plena validez legal** en Colombia:
- Ley 527 de 1999: equivalencia funcional de documentos electronicos
- Decreto 2364 de 2012: firma electronica con neutralidad tecnologica
- No se requiere autenticacion notarial para arriendo (contrato consensual)

Integracion con proveedores de firma electronica:

| Proveedor | Modelo | Precio |
|-----------|--------|--------|
| ZapSign | Firma electronica legal Colombia | Gratis hasta 5 docs/mes, desde ~$19 USD/mes |
| Viafirma Colombia | Firma electronica y digital avanzada | Plan gratuito disponible |
| Truora | Firma + verificacion de identidad | Por volumen |

- Reduce errores documentales en 91% y acelera ejecucion de contratos en 45%
- Ninguno de los portales lideres (FincaRaiz, Metrocuadrado) ofrece esto integrado

**4.12 Scanner Web de Direcciones (Inspirado en PropertyRadar)**

> ⚠️ **Alerta de Seguridad**: Esta funcion requiere capas de proteccion anti-fraude. La mayoria de fraudes inmobiliarios en Colombia se originan en grupos de Facebook Marketplace y clasificados informales. No importar listings sin validacion.

- Extension o funcionalidad que escanea paginas web (grupos de Facebook, clasificados) buscando direcciones de propiedades
- Limpia y formatea las direcciones encontradas
- Las agrega al mapa **como "No Verificado"** — nunca directamente como listing activo

**Medidas de seguridad obligatorias antes de lanzar:**

| Capa | Mecanismo |
|------|-----------|
| **Detección de duplicados** | Cruzar cada listing importado contra la BD: misma dirección + mismo precio = posible cuenta duplicada para fraude |
| **Scoring de riesgo automático** | Señales de alerta: precio muy por debajo del mercado (>30% menor), fotos robadas (hash de imagen), múltiples listings del mismo número/cuenta |
| **Verificación de identidad del publicador** | Antes de mostrar datos de contacto reales, validar que el arrendador tiene perfil verificado en CazaRaiz (cédula + selfie) |
| **Enmascaramiento de contacto** | Nunca exponer número directo de Facebook — siempre canalizar a través del chat de CazaRaiz para trazabilidad |
| **Reporte comunitario** | Botón "Reportar como fraude" visible en cada listing importado, con revisión humana antes de eliminar |
| **Ventana de cuarentena** | Listings importados permanecen 24h en estado "Pendiente de validación" antes de ser públicos |

**Fase de lanzamiento**: Solo disponible como beta cerrada con revisión manual, no en el MVP público.

**4.13 Computer Vision para Propiedades (Inspirado en Restb.ai)**
- Analisis de fotos del inmueble para extraer datos estructurados: condicion, calidad, caracteristicas
- Restb.ai procesa 2B+ imagenes/mes con 1,000+ data points por propiedad
- Aplicacion: puntuar estado del inmueble automaticamente a partir de fotos

**4.14 Integracion con La Haus**
- La Haus ($163M+ en funding) se enfoca en vivienda nueva con IA
- Oportunidad: conectar usuarios que buscan arriendos con opciones de compra de vivienda nueva
- Modelo de referidos o integracion de catalogo de proyectos nuevos

**4.15 Preparacion para Escrituras Digitales**
- Colombia tiene 13 notarias digitales (11 en Bogota, 1 en Medellin, 1 en Barranquilla)
- Decreto Ley 2106/2019 faculta actos notariales electronicos
- La app puede facilitar: recoleccion de documentos, pre-llenado de minutas, calculadora de gastos notariales, agenda de citas en notarias digitales
- Tiempo de firma reducido de 30 dias a 20 minutos en notarias digitales

### Fase 4 — Escala Regional (Meses 24-36)

**4.16 Expansion a Latinoamerica**

| Pais | Prioridad | Razon |
|------|-----------|-------|
| Mexico | 2 | Mercado US$169B, alta informalidad, Habi ya opera ahi |
| Peru | 3 | Muy alta informalidad, baja competencia digital |
| Argentina | 4 | Recuperacion activa, alta informalidad |
| Brasil | 5 | Mas competitivo (QuintoAndar US$5.1B) pero mayor mercado |
| Chile | 6 | Mas formalizado, Portal Inmobiliario domina con 70%+ |

---

## 5. Stack Tecnologico

### 5.1 OCR e Inteligencia Artificial

| Fase | Solucion | Costo | Razon |
|------|----------|-------|-------|
| MVP (0-1K imgs/mes) | Claude Haiku directo | ~$2.60/mes | Una sola llamada extrae + estructura. Simplifica arquitectura |
| Crecimiento (1K-100K) | Google Cloud Vision + Claude Haiku | ~$200/mes a 100K | Vision extrae texto crudo ($1.50/1K img), Haiku estructura |
| Escala (100K+) | Google Vision + Claude Haiku Batch | ~$1,600/mes a 1M | Batch API (50% descuento) para procesamiento no-urgente |

**Comparativa Claude vs Google Vision**:
- Google Vision: 50% mas barato, optimizado para letreros (TEXT_DETECTION), free tier 1K imgs/mes
- Claude Haiku: extraccion + estructuracion en un paso, comprension contextual superior, ~$0.0026/img
- **Enfoque hibrido recomendado** para escala: Vision ($0.0015/img) + Haiku texto ($0.0006) = ~$0.002/img total

### 5.2 WhatsApp

| Componente | Solucion | Costo |
|------------|----------|-------|
| Contacto desde app | Deep link `wa.me/` | **Gratis** — no requiere API |
| Confirmacion disponibilidad | WhatsApp Business API (Meta Cloud API directo) | ~$0.0009/msg utility (Colombia) |
| Captura de respuestas (futuro) | Webhooks + Claude Haiku para estructurar | Por volumen |

### 5.3 Stack de Desarrollo

| Componente | Tecnologia | Razon |
|------------|-----------|-------|
| App movil | Flutter | Mejor rendimiento de camara, 30-50% mas rapido que nativo |
| Backend | Node.js + NestJS | Escalable, ecosistema maduro |
| Base de datos | PostgreSQL + PostGIS | Queries geoespaciales para mapa |
| Storage de imagenes | AWS S3 o Google Cloud Storage | Escalable, bajo costo |
| Tiempo real | Supabase o Firebase | Actualizaciones de mapa en vivo |
| Firma electronica | ZapSign API | Validez legal Colombia, plan gratuito para MVP |
| Verificacion crediticia | Apitude (DataCredito) + TusDatos API | APIs documentadas, cobertura Colombia |

---

## 6. Modelo de Negocio

### 6.1 Modelo Hibrido en Fases

**Fase 1 (Meses 0-12): Freemium + Crowdsourcing**
- App gratuita para buscar, escanear letreros y generar QR basicos
- Gamificacion para motivar contribuciones (modelo Waze)
- Monetizacion cero — foco en masa critica de datos y usuarios

**Fase 2 (Meses 12-24): Lead Generation + Servicios Premium**
- Venta de leads a inmobiliarias ($5-15 USD por lead calificado)
- Suscripcion para agentes con alertas de nuevos letreros por zona ($30-100 USD/mes)
- Comision por intermediacion de seguros de arrendamiento
- Comision por generacion de contratos digitales

**Fase 3 (Meses 24-36): Data + Verificacion + Escala**
- API de datos para proptechs y constructoras ($500-5,000 USD/mes)
- Verificacion de inventario inmobiliario para bancos y aseguradoras
- Indices de precios basados en datos reales de letreros
- Expansion regional

### 6.2 Unit Economics Proyectados

| Metrica | Valor Estimado |
|---------|---------------|
| CAC (consumidor) | $2-5 USD (organico + referidos gamificados) |
| CAC (B2B: inmobiliaria) | $50-150 USD |
| LTV (suscripcion broker) | $360-1,200 USD/ano |
| LTV (lead generation) | $5-15 USD por lead |
| LTV (data API) | $500-5,000 USD/mes |
| Ratio LTV/CAC objetivo | >5:1 |
| Costo por foto procesada | $0.002-0.005 USD |

### 6.3 Proyeccion (24 meses)

| Escenario | Fotos/mes (M12) | Usuarios | Inmobiliarias | Ingresos M24 |
|-----------|-----------------|----------|---------------|-------------|
| Conservador | 50,000 | 100,000 | 500 | $25,000 USD/mes |
| Optimista | 200,000 | 500,000 | 2,000 | $120,000 USD/mes |

---

## 7. Alianzas Estrategicas

### 7.1 Alianzas Prioritarias

| Socio | Tipo | Valor para el proyecto |
|-------|------|----------------------|
| **Habi** | Socio estrategico / Proveedor API | AVM (Habimetro), 10M+ propiedades, presencia en Colombia y Mexico. Su foco en compraventa es complementario a nuestro foco en arriendos |
| **SURA** | Partnership de seguros | Lider en digitalizacion de seguros de arrendamiento, modelo sin codeudor, ya tiene alianza tech con Aptuno |
| **La Haus** | Integracion / Referidos | Marketplace vivienda nueva ($163M+ funding). Conectar buscadores de arriendo con opciones de compra |
| **Apitude** | Proveedor tech | Intermediario API para DataCredito/Experian. Integracion documentada en Python, JS, Go |
| **TusDatos.co** | Proveedor tech | API REST para verificacion de antecedentes. ~2,000 empresas clientes |
| **ZapSign** | Proveedor tech | Firma electronica con validez legal Colombia. API documentada, plan gratuito |

### 7.2 Alianzas Secundarias

| Socio | Tipo | Valor |
|-------|------|-------|
| TransUnion Colombia | Proveedor verificacion | Legal Check + Score crediticio. Seamless Onboarding API |
| IGAC | Datos abiertos | Geoportal con datos catastrales en GeoJSON/Shapefile |
| Notarias digitales | Integracion de servicios | 13 notarias digitales para escrituracion |
| Aseguradoras (MAPFRE, Zurich) | Comparador de seguros | Ampliar opciones del comparador de polizas |

---

## 8. Marco Legal

### 8.1 Cumplimiento Regulatorio

| Aspecto | Ley / Norma | Requisito | Riesgo |
|---------|-------------|-----------|--------|
| Fotografiar letreros en via publica | Ley 1581/2012 Art. 10 | Dato manifiestamente publico — **Permitido** | Bajo |
| Numeros de telefono | Ley 1581/2012 | Dato personal. Enmascarar o intermediar contacto | Medio |
| Consulta crediticia | Ley 1266/2008 | Requiere autorizacion expresa del titular | Alto |
| Datos de arrendatarios | Ley 1581/2012 | Autorizacion previa y politica de tratamiento | Alto |
| Contratos digitales | Ley 527/1999 + Decreto 2364/2012 | Plena validez. Firma electronica con equivalencia funcional | Bajo |
| Costo estudio arrendamiento | Regulacion 2025 | NO se puede cobrar al arrendatario | Medio |
| Escrituras digitales | Decreto Ley 2106/2019 | Solo en notarias digitales autorizadas (13 actualmente) | Bajo |

### 8.2 Acciones de Cumplimiento desde Dia 1

1. **Politica de privacidad y aviso de tratamiento de datos** (obligatorio)
2. **Enmascarar telefonos**: No publicar numero completo (310-XXX-XX34)
3. **Intermediar contacto**: Boton "Contactar" sin revelar dato directo (crea lock-in)
4. **Mecanismo de opt-out** para propietarios que quieran retirar su numero
5. **Flujo de consentimiento** explicito para verificacion crediticia
6. **Consultar asesor juridico** para determinar si la app puede ofrecer verificacion crediticia directamente o requiere intermediario autorizado

---

## 9. Viabilidad Financiera

### 9.1 Inversion Estimada para MVP

| Componente | Rango Bajo | Rango Alto |
|-----------|-----------|-----------|
| App movil (Flutter) | $50,000 | $80,000 |
| Backend (NestJS + PostgreSQL) | $20,000 | $40,000 |
| OCR e IA (Claude Haiku + Google Vision) | $8,000 | $15,000 |
| Infraestructura cloud (12 meses) | $6,000 | $18,000 |
| Diseno UX/UI | $8,000 | $15,000 |
| QA y testing | $5,000 | $10,000 |
| **Total MVP** | **$97,000** | **$178,000** |

### 9.2 Equipo Minimo (3-4 meses)

- 1 desarrollador Flutter senior
- 1 desarrollador backend (NestJS)
- 1 especialista ML/Vision (part-time)
- 1 disenador UX/UI (part-time)
- 1 product manager / founder

### 9.3 Costos Operativos Mensuales (Post-MVP)

| Concepto | 10K usuarios | 100K usuarios | 1M usuarios |
|----------|-------------|--------------|-------------|
| OCR (hibrido Vision+Haiku) | $20 | $200 | $1,600 |
| WhatsApp Business API | $9 | $90 | $900 |
| Infraestructura cloud | $500 | $1,500 | $5,000 |
| Firma electronica (ZapSign) | $19 | $99 | Custom |
| **Total estimado** | **~$550** | **~$1,900** | **~$7,500** |

### 9.4 Financiamiento

- **Objetivo**: Pre-seed/seed de $100K-200K USD
- **Ecosistema favorable**: Proptech recibio $16,700M globalmente en 2025 (+68% interanual)
- **Fondos activos en proptech Latam**: Kaszek, ALLVP, Magma Partners
- **Revenue multiples**: Proptech promedia 8.8x en 2025

---

## 10. Roadmap

| Hito | Plazo |
|------|-------|
| Validacion de concepto (OCR + prototipo QR) | Semanas 1-6 |
| MVP funcional (app + backend + QR + escaneo + WhatsApp) | Meses 2-5 |
| Beta cerrada (1 ciudad piloto: Bogota) | Meses 5-7 |
| Integracion verificacion + seguros | Meses 7-10 |
| Lanzamiento publico Colombia | Meses 8-10 |
| Contratos digitales + estimador de precios | Meses 10-14 |
| Expansion a Mexico | Meses 14-20 |
| Expansion a Peru/Argentina | Meses 20-28 |

### Cold-Start: Resolver el problema del huevo y la gallina

Antes del lanzamiento publico:
1. Equipo de 10-20 personas fotografiando letreros en zonas clave de Bogota (2-4 semanas)
2. Objetivo: 5,000-10,000 propiedades como base minima
3. Alianza con 50-100 inmobiliarias para generar QR desde el dia 1
4. Seed data de precios via portales publicos (IGAC, datos abiertos)

---

## 11. Riesgos y Mitigaciones

| Riesgo | Severidad | Mitigacion |
|--------|----------|-----------|
| Cold-start (sin datos = sin usuarios) | Alta | Seed data con equipo propio + QR con inmobiliarias aliadas |
| Portales grandes copian la funcionalidad | Alta | Moverse rapido, construir base de datos propietaria, efecto de red |
| Precision OCR en letreros manuscritos | Media | Pipeline hibrido (Vision + LLM), preprocesamiento de imagen |
| Regulacion de datos personales (telefonos) | Media | Enmascarar + intermediar, mecanismo opt-out, asesoria juridica |
| Fatiga de gamificacion | Media | Recompensas tangibles (descuentos en mudanzas, servicios) + beneficio directo (el usuario tambien busca) |
| Dependencia de Google Vision API | Baja | ML Kit on-device como fallback |
| Costos de almacenamiento de imagenes | Baja | Cloud escalable, costos decrecientes |

---

## 12. Gamificacion (Modelo Waze)

| Principio | Aplicacion |
|-----------|-----------|
| Puntos por contribucion | Puntos por cada foto de letrero verificada o QR generado |
| Rangos progresivos | "Explorador Novato" → "Cazador de Inmuebles Elite" |
| Beneficio inmediato | El usuario tambien busca arriendo/compra; contribuir mejora sus resultados |
| Pay-it-forward | "Otros contribuyeron las fotos que tu usaste, ahora contribuye tu" |
| Comunidad local | Rankings por barrio/zona, lideres comunitarios |
| Recompensas tangibles | Descuentos en mudanzas, seguros, servicios del hogar |

**Resultados documentados**: +22% en retencion de usuarios con gamificacion bien implementada.

---

## 13. Fuentes Principales

Esta propuesta se basa en tres investigaciones de mercado realizadas el 2026-03-21:

1. **Investigacion de App de Escaneo de Letreros** — Apps similares, tecnologia OCR, modelos AVM, verificacion de arrendatarios
2. **Mercado Inmobiliario Digital en Colombia** — Plataformas lideres, tamano de mercado, problemas, ecosistema proptech
3. **Viabilidad y Expansion a Latinoamerica** — Mercados regionales, modelos de negocio, crowdsourcing, marco regulatorio, viabilidad financiera

Investigaciones complementarias:
4. **Seguros de Arrendamiento en Colombia** — Tipos, proveedores, costos, oportunidades de integracion
5. **Contratos Digitales y Notarias** — Validez legal, plataformas, firmas electronicas, escrituracion digital
6. **Claude vs Google Vision para OCR + WhatsApp API** — Comparativa de precios, latencia, precision, deep links
7. **TransUnion Colombia + Disponibilidad de Inmuebles** — Productos, APIs, mecanismos de confirmacion

Todas las fuentes detalladas se encuentran en los documentos de investigacion en [docs/research/](docs/research/).

---

*Borrador generado el 2026-03-21. Pendiente de revision y aprobacion antes de pasar a fase de arquitectura.*
