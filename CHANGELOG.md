# Changelog — LEM Pro

Todos los cambios técnicos relevantes del desarrollo y compilación de la familia tipográfica se documentan en este archivo.

---

## [1.1.0] - 2026-08-27
### Added
- **Formatos Web (WOFF):** Compilación e incorporación de los archivos de fuentes web (`.woff`) para las 12 variantes de la familia en `builds/otf/proof/` (`Light`, `Regular`, `Medium`, `SemiBold`, `Bold`, `ExtraBold` tanto en *Upright* como en *Italic*).
- **Acuerdo de Licencia de Usuario Final (EULA):** Creación de `EULA.md` (bilingüe: Español / English), especificando las libertades de uso de escritorio, webfonts, incrustación en apps/documentos, y la protección del Nombre Reservado (*Reserved Font Name*).
- **Espécimen Tipográfico:** Adición del espécimen visual oficial de la familia en `assets/LEMpro.png` e integración en el `README.md`.

### Changed
- **README y Documentación:** Actualización de las especificaciones técnicas para distribución dual (OTF + WOFF), ajuste de tablas de instancias y normalización de enlaces relativos en el repositorio.

---

## [1.0.0] - 2026-08-21
### Added
- **Inicialización del Repositorio:** Configuración inicial del control de versiones y del repositorio siguiendo la estructura estándar para el desarrollo tipográfico.
- **Archivo Fuente (Design Source):** Incorporación del archivo de diseño master `LEM Pro fam.glyphs` (versión Glyphs 3) con soporte para interpolación y un set completo de 954 glifos.
- **Compilación de Instancias Estáticas (OTF/CFF):** Exportación de los 12 estilos estáticos (6 pesos en variantes Upright e Italic) de la familia tipográfica en `builds/otf/release/`:
  - **Light** (Weight Class 300) — Upright (`LEMProLight`) / Italic (`LEMProLightItalic`)
  - **Regular** (Weight Class 400) — Upright (`LEMProRegular`) / Italic (`LEMProRegularItalic`)
  - **Medium** (Weight Class 500) — Upright (`LEMProMedium`) / Italic (`LEMProMediumItalic`)
  - **SemiBold** (Weight Class 600) — Upright (`LEMProSemiBold`) / Italic (`LEMProSemiBoldItalic`)
  - **Bold** (Weight Class 700) — Upright (`LEMProBold`) / Italic (`LEMProBoldItalic`)
  - **ExtraBold** (Weight Class 800) — Upright (`LEMProExtraBold`) / Italic (`LEMProExtraBoldItalic`)
- **Documentación Técnica del Proyecto:** Creación de las guías de contexto histórico, flujo de trabajo de desarrollo y convenciones de nomenclatura para la tabla `name`.

### Font Metrics Summary (Resumen Métrico)
**Family Name:** "LEM Pro"
- **Units Per Em (UPM):** 1024
- **Number of Glyphs (Glyph Count):** 954 (Master Glyphs) / 470 por OTF compilado
- **Version:** 1.000; Glyphs 3.x
- **Axes:** Weight (`wght`: 300-800), Slant/Italic (`ital`: 0-1)

#### Styles Overview (PostScript Names)
- **Light (300):** `LEMProLight` / `LEMProLightItalic`
- **Regular (400):** `LEMProRegular` / `LEMProRegularItalic`
- **Medium (500):** `LEMProMedium` / `LEMProMediumItalic`
- **SemiBold (600):** `LEMProSemiBold` / `LEMProSemiBoldItalic`
- **Bold (700):** `LEMProBold` / `LEMProBoldItalic`
- **ExtraBold (800):** `LEMProExtraBold` / `LEMProExtraBoldItalic`

