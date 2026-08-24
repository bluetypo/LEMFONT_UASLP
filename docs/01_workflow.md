# Flujo de Trabajo Tipográfico (Workflow)

Este documento describe el proceso recomendado para la edición, exportación y publicación de la familia tipográfica **LEM Pro**.

## 1. Archivo de Diseño y Edición
* **Archivo Fuente Nivel de Diseño:** `sources/LEM Pro fam.glyphs`
* **Software de Edición:** Glyphs 3.x o superior.
* **Control de Masters:** La edición de formas, anclas y espaciado debe ejecutarse de forma consistente en el espacio de diseño para mantener la interpolación entre los distintos pesos e inclinaciones (Upright e Italic).

## 2. Exportación y Compilación de Instancias Estáticas
Las 12 instancias estáticas definidas en el archivo fuente se compilan en formato OpenType con curvas PostScript (OTF/CFF) y se ubican en:
* **Directorio de Distribución (Release):** `builds/otf/release/`
* **Configuración de Exportación recomendada:**
  - Activar *Remove Overlaps* (Fusión de trazados superpuestos).
  - Activar *Autohinting* (Optimización de renderizado).
* **Nombres de Archivo Oficiales (PostScript Names):**
  - **Light:** `LEMProLight.otf` / `LEMProLightItalic.otf`
  - **Regular:** `LEMProRegular.otf` / `LEMProRegularItalic.otf`
  - **Medium:** `LEMProMedium.otf` / `LEMProMediumItalic.otf`
  - **SemiBold:** `LEMProSemiBold.otf` / `LEMProSemiBoldItalic.otf`
  - **Bold:** `LEMProBold.otf` / `LEMProBoldItalic.otf`
  - **ExtraBold:** `LEMProExtraBold.otf` / `LEMProExtraBoldItalic.otf`

## 3. Publicación y Distribución Oficial (Releases)
Una vez que las instancias estáticas han superado las pruebas de calidad de métricas, rendering y Style Linking:
1. Empaqueta los archivos OTF finales en un archivo comprimido `.zip` con el identificador de la versión (ej. `LEMPro_v1.0.0.zip`).
2. Guarda los archivos en: `builds/otf/release/`.
3. Actualiza el historial en el archivo `CHANGELOG.md` de la raíz del proyecto.
4. Genera la etiqueta correspondiente en Git (ej. `git tag -a v1.0.0`) y haz push a GitHub.

