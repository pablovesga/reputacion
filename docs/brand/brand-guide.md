# Guía de Identidad Visual — Reputación

> Plataforma SaaS de Índice de Gestión de la Reputación Empresarial

---

## 1. Concepto de Marca

**Reputación** es una plataforma de datos e inteligencia artificial que convierte el Índice de Gestión de la Reputación (IGR) en información accionable para empresas colombianas. La identidad visual refleja tres valores core:

| Valor | Expresión visual |
|-------|-----------------|
| **Confianza** | Navy profundo, formas sólidas, tipografía directa |
| **Datos / Precisión** | Sky blue, barras de progreso, métricas visibles |
| **Excelencia** | Amber/gold en scores y logros |

---

## 2. Logo

### Composición
El logo combina un **ícono de barras ascendentes** (representando el crecimiento de la reputación) con un **wordmark tipográfico**.

- `logo.svg` — Versión horizontal (fondo claro)
- `logo-dark.svg` — Versión horizontal (fondo oscuro)
- `logo-icon.svg` — Ícono solo (apps, favicons, avatars)

### Zonas de exclusión
Mantener un espacio mínimo igual a la altura de la "R" del wordmark alrededor del logo en todos los lados.

### Usos prohibidos
- No rotar el logo
- No cambiar los colores del ícono
- No agregar sombras externas al ícono
- No usar el wordmark sin el ícono (salvo espacio muy reducido)
- No deformar ni estirar

---

## 3. Paleta de Colores

### Colores primarios

| Token | Hex | Uso |
|-------|-----|-----|
| `--color-primary-800` | `#0F3460` | Color principal de marca, headers, navbar |
| `--color-primary-700` | `#1B4F8A` | Hover sobre elementos primarios |
| `--color-primary-600` | `#2563A0` | Links, acciones secundarias |

### Colores de acento

| Token | Hex | Uso |
|-------|-----|-----|
| `--color-accent-500` | `#0EA5E9` | CTAs principales, highlights, gráficas |
| `--color-accent-400` | `#38BDF8` | Iconos, elementos activos |
| `--color-accent-100` | `#E0F2FE` | Badges, tags, backgrounds informativos |

### Colores de excelencia

| Token | Hex | Uso |
|-------|-----|-----|
| `--color-gold-500`   | `#F59E0B` | Estrellas, scores top, logros |
| `--color-gold-400`   | `#FCD34D` | Ícono de estrella |
| `--color-gold-100`   | `#FEF3C7` | Fondos de distinción |

### Escala de scores IGR

```
90–100  ★ Excelente    #F59E0B  (Amber)
70–89   ↑ Bueno        #10B981  (Emerald)
50–69   → Promedio     #0EA5E9  (Sky Blue)
30–49   ↓ Bajo         #F97316  (Orange)
 0–29   ⚠ Crítico      #EF4444  (Red)
```

---

## 4. Tipografía

### Fuente principal: Inter
```
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
```

| Uso | Peso | Tamaño |
|-----|------|--------|
| Títulos H1 | 700 Bold | 36px / 2.25rem |
| Títulos H2 | 600 SemiBold | 30px / 1.875rem |
| Títulos H3 | 600 SemiBold | 24px / 1.5rem |
| Body | 400 Regular | 16px / 1rem |
| Labels / UI | 500 Medium | 14px / 0.875rem |
| Captions | 400 Regular | 12px / 0.75rem |
| Métricas / datos | 700 Bold | Variable |

### Fuente monoespaciada: JetBrains Mono
Para mostrar scores, códigos, datos numéricos en dashboards.

---

## 5. Componentes visuales clave

### Score Badge
Círculo o píldora con el score IGR. Usa el color semántico del tier correspondiente.

```
┌─────────────────┐
│  ★  87.4        │  ← Color: Emerald (#10B981)
│  BUENA          │
└─────────────────┘
```

### Barra de progreso de reputación
Barra horizontal de 0–100 con gradiente del rojo al amber según progreso. Siempre mostrar el valor numérico.

### Cards de empresa
- Borde izquierdo de 4px con el color del tier
- Sombra `--shadow-md`
- Radius `--radius-lg`

---

## 6. Uso en interfaces

### Navbar / Header
- Fondo: `--color-primary-800` (#0F3460)
- Logo: versión `logo-dark.svg`
- Texto: `--color-text-inverse`

### Dashboard principal
- Fondo: `--color-surface` (#F8FAFC)
- Cards: `--color-surface-raised` (#FFFFFF) con `--shadow-md`
- Métricas principales: `--color-text-primary` en tamaño 2xl–3xl bold

### Botones
```
Primary:   bg #0EA5E9  text blanco   hover #0284C7
Secondary: bg #0F3460  text blanco   hover #1B4F8A
Ghost:     bg trans    text #0F3460  hover bg #EFF6FF  border #0F3460
Danger:    bg #EF4444  text blanco   hover #B91C1C
```

---

## 7. Iconografía

Usar [Lucide Icons](https://lucide.dev/) como set principal:
- Trazo consistente (stroke-width: 1.5–2)
- Tamaños: 16px (inline), 20px (UI), 24px (features)
- Color: heredar del contexto o usar `--color-accent-400`

Icons clave del producto:
- `trending-up` — mejora de reputación
- `star` — score / calificación
- `shield-check` — reputación protegida / verificada
- `bar-chart-2` — métricas IGR
- `building-2` — empresa
- `award` — logros / certificaciones
- `file-presentation` — presentaciones AI
- `video` — videos AI

---

## 8. Voz y tono

| Contexto | Tono |
|----------|------|
| Onboarding | Cálido, guía paso a paso |
| Dashboard | Directo, conciso, basado en datos |
| Errores | Claro, sin culpa, con solución |
| Métricas negativas | Neutral, enfocado en mejora |
| Logros | Celebratorio pero profesional |

**Evitar:** lenguaje técnico innecesario, superlativos vacíos, textos en mayúsculas sostenidas.

---

*Última actualización: 2026-03-20*
