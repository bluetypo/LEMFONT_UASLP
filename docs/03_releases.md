# Registro de Releases — LEM Pro

Este archivo documenta la hoja de ruta (*roadmap*), lanzamientos de producción e hitos técnicos en la vida del proyecto tipográfico **LEM Pro**.

---

## [v1.0.0] - 2026-08-21 (Actual)
**Estado:** Estable / Primera Compilación de Producción
**Estilos:** Light, Regular, SemiBold, ExtraBold.
**Enfoque:** Estructuración del design space y lanzamiento de la vertiente romana (Upright).

### Hitos Técnicos:
- Sincronización de un set extendido de 954 glifos (cobertura Latin Pro).
- Limpieza integral del archivo fuente y compatibilidad métrica entre los dos masters de peso.
- Implementación de las funciones OpenType básicas (`kern`, `ccmp`, `liga`).
- Configuración de la estructura del repositorio de desarrollo y documentación para Git.

---

## Próximos Lanzamientos Planificados (Roadmap)

### [v1.1.0] - Fecha TBD
**Enfoque:** Variable Font (VF)
- Compilación de la versión variable (`LEMPro-VF.ttf` y su variante web `.woff2`).
- Configuración del eje de peso (`wght`: 300-800) y definición de coordenadas para las instancias estáticas intermedias en la tabla `STAT`.
- Pruebas de renderizado y alineación de curvas variables en navegadores web de escritorio y móviles.

### [v1.2.0] - Fecha TBD
**Enfoque:** Vertiente Itálica (Slanted/Italics)
- Diseño y desarrollo de los estilos cursivos/itálicos correspondientes para los pesos Light, Regular, SemiBold y ExtraBold.
- Definición de un eje de inclinación (`slnt` / `ital`) en el archivo de diseño Glyphs.
- Vinculación cruzada de estilos (Style Linking) romana-itálica para atajos del sistema.
