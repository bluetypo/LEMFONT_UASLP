# Changelog — LEM Pro

Todos los cambios técnicos relevantes del desarrollo y compilación de la familia tipográfica se documentan en este archivo.

---

## [1.0.0] - 2026-08-21
### Added
- **Inicialización del Repositorio:** Configuración inicial del control de versiones y del repositorio siguiendo la estructura estándar para el desarrollo tipográfico.
- **Archivo Fuente (Design Source):** Incorporación del archivo de diseño master `LEM Pro.glyphs` (versión Glyphs 3) con soporte para interpolación y un set completo de 954 glifos.
- **Compilación de Instancias Estáticas (OTF/CFF):** Exportación inicial de los 4 estilos estáticos de la familia tipográfica en `builds/otf/proof/`:
  - **Light** (Weight Class 300)
  - **Regular** (Weight Class 400)
  - **SemiBold** (Weight Class 600)
  - **ExtraBold** (Weight Class 800)
- **Documentación Técnica del Proyecto:** Creación de las guías de contexto histórico, flujo de trabajo de desarrollo y convenciones de nomenclatura para la tabla `name`.

### Font Metrics Summary (Resumen Métrico)
**Family Name:** "LEM Pro"
- **Units Per Em (UPM):** 1024
- **Number of Glyphs (Glyph Count):** 954
- **Version:** 1.000; Glyphs 3.x
- **Axes:** Weight (`wght`: 300-800)

#### Styles Overview (PostScript Names)
- **Light (300):** `LEMProLight`
- **Regular (400):** `LEMProRegular`
- **SemiBold (600):** `LEMProSemiBold`
- **ExtraBold (800):** `LEMProExtraBold` (Estilo asignado para vinculación negrita / *Style Linking*).
