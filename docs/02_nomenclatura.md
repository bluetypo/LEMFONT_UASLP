# Nomenclatura — LEM Pro

Este documento define las convenciones de naming oficiales para la familia tipográfica del **Laboratorio de Experimentación Multimedia**.

Su objetivo es garantizar coherencia entre:
- Metadata interna (Font Info / Tabla `name`)
- Archivos exportados (.otf, .woff2)
- Compatibilidad en sistemas operativos (Windows / macOS)
- Estructura del repositorio y comunicación del LEM.

---

## 1. Family Name

**Family Name oficial:** `LEM Pro` (para visualización en menús)  
**Filenames y PostScript Name base:** `LEMPro` (sin espacios para evitar errores en servidores y código).

Este nombre debe mantenerse idéntico en todos los estilos para asegurar el agrupamiento correcto.

---

## 2. Style Names & Metrics

| Estilo      | Style Name | Weight Class | Width Class |
|-------------|------------|--------------|-------------|
| **Light** | Light      | 300          | 5 (Medium)  |
| **Regular** | Regular    | 400          | 5 (Medium)  |
| **SemiBold** | SemiBold   | 600          | 5 (Medium)  |
| **ExtraBold** | ExtraBold  | 800          | 5 (Medium)  |

---

## 3. Style Linking (Vinculación de Estilos)

Para asegurar que el uso de las teclas rápidas (**B** / **I**) funcione correctamente en software de oficina y diseño:

**Regular (Base):**
- Style Linking Family: `LEM Pro`
- Style Linking Style: `Regular`

**ExtraBold:**
- Style Linking Family: `LEM Pro`
- Style Linking Style: `Bold` (Vinculado a Regular en sistemas que sólo soportan Regular/Bold como par básico).

**Light / SemiBold:**
- Estos estilos no llevan vinculación directa de estilo básica (Style Linking) para evitar conflictos en menús de aplicaciones sencillas que sólo aceptan una variante base y una variante bold.

---

## 4. Naming para exportación (Archivos)

Formato oficial sin espacios para evitar errores en servidores y código. Los archivos se nombran exactamente de acuerdo a su PostScript Name + `.otf`:

- `LEMProLight.otf`
- `LEMProRegular.otf`
- `LEMProSemiBold.otf`
- `LEMProExtraBold.otf`

**Reglas:**
- Sin números de versión en el nombre del archivo (ej. NO usar `LEMProRegular_v1.otf`).
- La versión se controla exclusivamente mediante el `CHANGELOG.md` y la metadata interna.

---

## 5. Versionado

**Formato interno (Metadata):** `Version 1.000; Glyphs 3.x`

**Convención de versión en Repositorio (Git Tags):**
- `v1.0.0` (Lanzamiento inicial estable)

---

## 6. PostScript Name (PS Name)

El nombre PostScript es crítico para la impresión y generación de PDF. No debe exceder los 29 caracteres y no debe contener espacios:

- `LEMProLight`
- `LEMProRegular`
- `LEMProSemiBold`
- `LEMProExtraBold`

---

## 7. Coherencia Institucional

En publicaciones del Laboratorio, la fuente debe referirse siempre como **LEM Pro**.
