# Nomenclatura — LEM Pro

Este documento define la estructura de metadatos y las convenciones de nomenclatura de la tabla `name` (especificación OpenType) para garantizar la compatibilidad multiplataforma (macOS, Windows, Linux) y el agrupamiento correcto de los estilos en los menús de aplicaciones de diseño (Adobe, Figma) y de oficina (Microsoft Word, Google Docs).

---

## 1. Agrupamiento de Familia (Family Naming)

Para evitar problemas de fragmentación en los menús y asegurar que los estilos aparezcan agrupados bajo una misma familia:

* **Family Name (ID 16 - Typographic Family Name):** `LEM Pro`
  - Nombre completo que agrupa a todos los estilos en menús extendidos.
* **Subfamily Name (ID 17 - Typographic Subfamily Name):** `Light` | `Regular` | `SemiBold` | `ExtraBold`
  - Identifica el peso individual de la fuente en menús extendidos.
* **Font Family Name (ID 1 - Family Name):** `LEM Pro`
  - Utilizado para compatibilidad en aplicaciones básicas que solo admiten un modelo de cuatro estilos (Regular, Italic, Bold, Bold Italic). 

---

## 2. Definición de Instancias (Styles & Weights)

La consistencia en la codificación de pesos se define a través de los valores de la tabla `OS/2` (`usWeightClass` y `usWidthClass`):

| Estilo | Style Name (ID 2/17) | Weight Class (`usWeightClass`) | Width Class (`usWidthClass`) |
| :--- | :--- | :---: | :---: |
| **Light** | Light | 300 | 5 (Medium) |
| **Regular** | Regular | 400 | 5 (Medium) |
| **SemiBold** | SemiBold | 600 | 5 (Medium) |
| **ExtraBold** | ExtraBold | 800 | 5 (Medium) |

---

## 3. Vinculación de Estilos (Style Linking)

Para que el atajo de negrita (**B** / **Cmd+B**) funcione correctamente en procesadores de texto de oficina y navegadores web:

* **Regular (Base):**
  - Style Linking Family: `LEM Pro`
  - Style Linking Style: *Ninguno* (es la base).
* **ExtraBold (Bold):**
  - Style Linking Family: `LEM Pro`
  - Style Linking Style: `Bold` (Vinculado a `Regular`).
  - Al presionar **B** sobre un texto en `LEM Pro Regular`, el sistema cambiará dinámicamente el glifo activo al master correspondiente en `LEMProExtraBold`.
* **Light / SemiBold:**
  - No llevan vinculación de estilo (Style Linking) para evitar conflictos en menús simplificados que no soportan pesos intermedios.

---

## 4. PostScript Name (ID 6) y Naming de Archivo

El nombre PostScript es de vital importancia para la generación de PDFs y compatibilidad con RIPs de impresión. No debe superar los 29 caracteres, no contiene espacios y se utiliza exactamente para nombrar el archivo compilado final:

* **Light:** PS Name: `LEMProLight` $\rightarrow$ Archivo: `LEMProLight.otf`
* **Regular:** PS Name: `LEMProRegular` $\rightarrow$ Archivo: `LEMProRegular.otf`
* **SemiBold:** PS Name: `LEMProSemiBold` $\rightarrow$ Archivo: `LEMProSemiBold.otf`
* **ExtraBold:** PS Name: `LEMProExtraBold` $\rightarrow$ Archivo: `LEMProExtraBold.otf`

---

## 5. Parámetros de Versión (ID 5)

* **Metadata de Versión (ID 5):** `Version 1.000; Glyphs 3.x`
* **Git Tags:** `v1.0.0`
