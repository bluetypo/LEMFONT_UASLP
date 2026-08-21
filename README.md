# LEM Pro — Repositorio Tipográfico

**LEM Pro** es la familia tipográfica oficial del **Laboratorio de Experimentación Multimedia (LEM)**, perteneciente a la Facultad de Hábitat de la Universidad Autónoma de San Luis Potosí (UASLP).

Este repositorio aloja los archivos fuente de diseño y las compilaciones de producción de la familia, estructurados bajo estándares profesionales de desarrollo tipográfico y control de versiones.

## Estructura de la Familia (Uprights - v1.0.0)
La familia se compone actualmente de **4 pesos estáticos**, generados a partir de un eje continuo de interpolación de peso (`wght`):

| Estilo / Instancia | Upright | Italic | Weight Class | PostScript Name |
| :--- | :---: | :---: | :---: | :--- |
| **Light** | ✓ | - | 300 | `LEMProLight` |
| **Regular** | ✓ | - | 400 | `LEMProRegular` |
| **SemiBold** | ✓ | - | 600 | `LEMProSemiBold` |
| **ExtraBold** | ✓ | - | 800 | `LEMProExtraBold` |

## Especificaciones Técnicas (Font Specs)
* **Formato:** OpenType CFF (OTF) compilado con curvas PostScript (cúbicas).
* **Unidades por Em (UPM):** 1024.
* **Set de Glifos (Charset):** 954 glifos (cobertura Latin Pro extendida con diacríticos combinables, figuras tipográficas avanzadas y ligaduras).
* **OpenType Features:** Soporte integrado para `kern` (clases de kerning de alta densidad), `ccmp` (composición y descomposición glífica), y `liga` (ligaduras estándar).

## Estado de Producción
La versión actual **v1.0.0** representa el primer hito estable de la vertiente romana (Upright). El archivo fuente master en formato Glyphs se encuentra estructurado para facilitar la futura compilación de fuentes variables (Variable Fonts).

Las instancias OTF listas para pruebas de rendimiento y QA se ubican en:
`builds/otf/proof/`

## Sobre el Laboratorio
El Laboratorio de Experimentación Multimedia (LEM) es un espacio multidisciplinario de la UASLP enfocado en el diseño paramétrico, la percepción visual y la experimentación digital.
🌐 [Visita el sitio oficial de la Facultad del Hábitat](https://habitat.uaslp.mx)

---

## Pruebas de Rendering y QA
1. Descarga las fuentes compiladas desde `builds/otf/proof/`.
2. Instala los estilos en tu sistema operativo o gestor de fuentes.
3. Para validar la vinculación de estilos (*Style Linking*), comprueba que la variante `ExtraBold` responda correctamente al atajo de teclado negrita (**B** / **N**) cuando se selecciona el estilo `Regular` en software compatible.

## Licencia
Esta tipografía se distribuye bajo la licencia abierta **SIL Open Font License 1.1** detallada en el archivo `LICENSE.txt`.
