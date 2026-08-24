# Nomenclatura — LEM Pro

Este documento define la estructura de metadatos y las convenciones de nomenclatura de la tabla `name` (especificación OpenType) para garantizar la compatibilidad multiplataforma (macOS, Windows, Linux) y el agrupamiento correcto de los estilos en los menús de aplicaciones de diseño (Adobe, Figma) y de oficina (Microsoft Word, Google Docs).

---

## 1. Agrupamiento de Familia (Family Naming)

Para evitar problemas de fragmentación en los menús y asegurar que los estilos aparezcan agrupados bajo una misma familia:

* **Family Name (ID 16 - Typographic Family Name):** `LEM Pro`
  - Nombre completo que agrupa a todos los estilos en menús extendidos.
* **Subfamily Name (ID 17 - Typographic Subfamily Name):** `Light` | `Light Italic` | `Regular` | `Regular Italic` | `Medium` | `Medium Italic` | `SemiBold` | `SemiBold Italic` | `Bold` | `Bold Italic` | `ExtraBold` | `ExtraBold Italic`
  - Identifica el peso e inclinación individual de la fuente en menús extendidos.
* **Font Family Name (ID 1 - Family Name):** `LEM Pro`
  - Utilizado para compatibilidad en aplicaciones básicas que solo admiten un modelo de cuatro estilos (Regular, Italic, Bold, Bold Italic).

---

## 2. Definición de Instancias (Styles & Weights)

La consistencia en la codificación de pesos se define a través de los valores de la tabla `OS/2` (`usWeightClass` y `usWidthClass`):

| Estilo / Peso | Style Name (ID 2/17) | Weight Class (`usWeightClass`) | Width Class (`usWidthClass`) |
| :--- | :--- | :---: | :---: |
| **Light** | Light / Light Italic | 300 | 5 (Medium) |
| **Regular** | Regular / Regular Italic | 400 | 5 (Medium) |
| **Medium** | Medium / Medium Italic | 500 | 5 (Medium) |
| **SemiBold** | SemiBold / SemiBold Italic | 600 | 5 (Medium) |
| **Bold** | Bold / Bold Italic | 700 | 5 (Medium) |
| **ExtraBold** | ExtraBold / ExtraBold Italic | 800 | 5 (Medium) |

---

## 3. Vinculación de Estilos (Style Linking)

Para que los atajos de negrita (**B** / **Cmd+B**) e itálica (**I** / **Cmd+I**) funcionen correctamente en procesadores de texto de oficina y navegadores web:

* **Pares Base / Negrita / Itálica:**
  - `Regular` + **B** $\rightarrow$ `Bold`
  - `Regular` + **I** $\rightarrow$ `Regular Italic`
  - `Regular` + **B** + **I** $\rightarrow$ `Bold Italic`
* **Estilos adicionales (Light, Medium, SemiBold, ExtraBold):**
  - Cada variante Upright se vincula a su correspondiente variante **Italic** con el atajo **I** / **Cmd+I**.

---

## 4. PostScript Name (ID 6) y Naming de Archivo

El nombre PostScript es de vital importancia para la generación de PDFs y compatibilidad con RIPs de impresión. No debe superar los 29 caracteres, no contiene espacios y se utiliza exactamente para nombrar los archivos compilados finales:

* **Light:** `LEMProLight` $\rightarrow$ `LEMProLight.otf` / `LEMProLightItalic` $\rightarrow$ `LEMProLightItalic.otf`
* **Regular:** `LEMProRegular` $\rightarrow$ `LEMProRegular.otf` / `LEMProRegularItalic` $\rightarrow$ `LEMProRegularItalic.otf`
* **Medium:** `LEMProMedium` $\rightarrow$ `LEMProMedium.otf` / `LEMProMediumItalic` $\rightarrow$ `LEMProMediumItalic.otf`
* **SemiBold:** `LEMProSemiBold` $\rightarrow$ `LEMProSemiBold.otf` / `LEMProSemiBoldItalic` $\rightarrow$ `LEMProSemiBoldItalic.otf`
* **Bold:** `LEMProBold` $\rightarrow$ `LEMProBold.otf` / `LEMProBoldItalic` $\rightarrow$ `LEMProBoldItalic.otf`
* **ExtraBold:** `LEMProExtraBold` $\rightarrow$ `LEMProExtraBold.otf` / `LEMProExtraBoldItalic` $\rightarrow$ `LEMProExtraBoldItalic.otf`

---

## 5. Parámetros de Versión (ID 5)

* **Metadata de Versión (ID 5):** `Version 1.000; Glyphs 3.x`
* **Git Tags:** `v1.0.0`

