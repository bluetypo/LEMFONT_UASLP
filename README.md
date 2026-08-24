# LEM Pro — Repositorio Tipográfico

**LEM Pro** es la familia tipográfica oficial del **Laboratorio de Experimentación Multimedia (LEM)**, perteneciente a la Facultad del Hábitat de la Universidad Autónoma de San Luis Potosí (UASLP).

Este repositorio aloja los archivos fuente de diseño y las compilaciones de producción de la familia, estructurados bajo estándares profesionales de desarrollo tipográfico y control de versiones.

## Estructura de la Familia (12 Estilos - Release)
La familia compilada en producción en `builds/otf/release/` se compone de **6 pesos** con sus correspondientes variantes **Upright** (Romana) e **Italic** (Cursiva), sumando un total de **12 instancias estáticas OTF**:

| Estilo / Instancia | Upright | Italic | Weight Class | Archivo OTF | PostScript Name |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **Light** | ✓ | ✓ | 300 | `LEMProLight.otf` / `LEMProLightItalic.otf` | `LEMProLight` / `LEMProLightItalic` |
| **Regular** | ✓ | ✓ | 400 | `LEMProRegular.otf` / `LEMProRegularItalic.otf` | `LEMProRegular` / `LEMProRegularItalic` |
| **Medium** | ✓ | ✓ | 500 | `LEMProMedium.otf` / `LEMProMediumItalic.otf` | `LEMProMedium` / `LEMProMediumItalic` |
| **SemiBold** | ✓ | ✓ | 600 | `LEMProSemiBold.otf` / `LEMProSemiBoldItalic.otf` | `LEMProSemiBold` / `LEMProSemiBoldItalic` |
| **Bold** | ✓ | ✓ | 700 | `LEMProBold.otf` / `LEMProBoldItalic.otf` | `LEMProBold` / `LEMProBoldItalic` |
| **ExtraBold** | ✓ | ✓ | 800 | `LEMProExtraBold.otf` / `LEMProExtraBoldItalic.otf` | `LEMProExtraBold` / `LEMProExtraBoldItalic` |

## Especificaciones Técnicas (Font Specs)
* **Formato:** OpenType CFF (OTF) compilado con curvas PostScript (cúbicas).
* **Ubicación de Release:** `builds/otf/release/`
* **Unidades por Em (UPM):** 1024.
* **Set de Glifos por Archivo OTF:** 470 glifos (cobertura Latin extendida con diacríticos, versalitas, figuras numéricas tabulares y elzevirianas, y ligaduras). *Nota: El archivo de diseño fuente master en `sources/` cuenta con 954 glifos.*
* **OpenType Features (GSUB):** 
  * `aalt` — *Access All Alternates*
  * `c2sc` — *Capitals to Small Caps*
  * `case` — *Case-Sensitive Forms*
  * `ccmp` — *Glyph Composition/Decomposition*
  * `liga` — *Standard Ligatures*
  * `lnum` — *Lining Figures*
  * `locl` — *Localized Forms*
  * `onum` — *Oldstyle Figures*
  * `smcp` — *Small Capitals*

## Soporte de Idiomas (Language Support)
Soporte para más de 100 idiomas de base latina:

> Afrikaans • Albanian • Asu • Basque • Bemba • Bena • Bosnian • Catalan • Cebuano • Chiga • Cornish • Corsican • Croatian • Czech • Dutch • Embu • English • Estonian • Filipino • Finnish • Friulian • Galician • German • Guadeloupean Creole • Gusii • Haitian Creole • Ido • Indonesian • Interlingua • Irish • Iskonawa • Italian • Javanese • Jju • Kabuverdianu • Kalenjin • Kamba • Kikuyu • Kinyarwanda • Lojban • Lower Sorbian • Luo • Luxembourgish • Luyia • Machame • Makhuwa-Meetto • Makonde • Malagasy • Malay • Manx • Māori • Martinican Creole • Meru • Morisyen • Nheengatu • North Ndebele • Northern Sotho • Nyanja • Nyankole • Occitan • Oromo • Polish • Portuguese • Romansh • Rombo • Rundi • Rwa • Samburu • Sango • Sangu • Sardinian • Scottish Gaelic • Sena • Serbian • Shambala • Shipibo-Konibo • Shona • Slovak • Slovenian • Soga • Somali • South Ndebele • Southern Sotho • Spanish • Sundanese • Swahili • Swati • Swedish • Swiss German • Taita • Taroko • Teso • Tsonga • Tswana • Turkish • Turkmen • Upper Sorbian • Vunjo • Welsh • Wolastoqey • Xhosa • Zulu

## Estado de Producción
Las **12 instancias estáticas OTF** listas para distribución y producción se ubican en:
[`builds/otf/release/`](file:///Volumes/Mac%20SSD/GitRepo/LEMFONT_UASLP/builds/otf/release)

El archivo fuente master en formato Glyphs (`sources/LEM Pro fam.glyphs`) se encuentra estructurado para facilitar el mantenimiento y la compilación de fuentes variables (Variable Fonts).

## Sobre el Laboratorio
El Laboratorio de Experimentación Multimedia (LEM) es un espacio multidisciplinario de la UASLP enfocado en el diseño paramétrico, la percepción visual y la experimentación digital.
🌐 [Visita el sitio oficial del Laboratorio de Experimentación Multimedia](https://lem.uaslp.mx)

---

## Pruebas de Rendering y QA
1. Descarga las fuentes compiladas desde [`builds/otf/release/`](file:///Volumes/Mac%20SSD/GitRepo/LEMFONT_UASLP/builds/otf/release).
2. Instala los estilos en tu sistema operativo o gestor de fuentes.
3. Para validar la vinculación de estilos (*Style Linking*), comprueba que las variantes responda correctamente a los atajos de teclado (**B** / **N** para negritas y **I** / **K** para itálicas) cuando se seleccionan los estilos base en software compatible.

## Licencia
Esta tipografía se distribuye bajo la licencia abierta **SIL Open Font License 1.1** detallada en el archivo [LICENSE.txt](file:///Volumes/Mac%20SSD/GitRepo/LEMFONT_UASLP/LICENSE.txt).


