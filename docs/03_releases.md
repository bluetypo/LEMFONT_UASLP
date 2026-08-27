# Registro de Releases — LEM Pro

Este archivo documenta la hoja de ruta (*roadmap*), lanzamientos de producción e hitos técnicos en la vida del proyecto tipográfico **LEM Pro**.

---

## [v1.1.0] - 2026-08-27 (Actual)
**Estado:** Estable / Compilación de Producción
**Estilos:** Light, Regular, Medium, SemiBold, Bold, ExtraBold (con variantes Upright e Italic, 12 estilos en total).
**Enfoque:** Lanzamiento completo de la familia en formatos OTF y WOFF empaquetados en `builds/release/`.

### Hitos Técnicos:
- Compilación e integración de 12 estilos estáticos en formato OTF (6 pesos en versiones Upright e Italic).
- Sincronización de un set extendido de 954 glifos en el fuente master (cobertura Latin Pro) y 470 glifos compilados por archivo OTF.
- Limpieza integral del archivo fuente y compatibilidad métrica entre los masters de peso e inclinación.
- Implementación de funciones OpenType avanzadas (`aalt`, `c2sc`, `case`, `ccmp`, `liga`, `lnum`, `locl`, `onum`, `smcp`).
- Configuración de la estructura del repositorio de desarrollo y documentación para Git.

---

## Próximos Lanzamientos Planificados (Roadmap)

### [v1.1.0] - Fecha TBD
**Enfoque:** Variable Font (VF) y Fuentes Web (WOFF2)
- Compilación de la versión variable (`LEMPro-VF.ttf` y variante web `.woff2`) con ejes de peso (`wght`: 300-800) e inclinación (`ital`: 0-1).
- Definición de coordenadas para las instancias estáticas intermedias en la tabla `STAT`.
- Pruebas de renderizado y alineación de curvas variables en navegadores web de escritorio y móviles.

