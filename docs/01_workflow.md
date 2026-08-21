# Workflow (propuesto)

## Estructura de trabajo
- **Fuentes Activas (Upright):** `sources/upright/glyphs/LEM Pro.glyphs`
- **Archivos de Prueba (OTF):** `builds/otf/proof/`

## Exportación
- **Builds de prueba (Proofing):** `builds/otf/proof/`
  - Nombres oficiales de archivo correspondientes a sus nombres PostScript:
    - `LEMProLight.otf`
    - `LEMProRegular.otf`
    - `LEMProSemiBold.otf`
    - `LEMProExtraBold.otf`
- **Release (Distribución oficial):** `builds/otf/release/`
  - Se colocan las versiones empaquetadas (.zip) y carpetas estables de producción una vez aprobadas.

## Registro de cambios
- Todos los cambios de contornos, espaciado, kerning o set de caracteres se documentan detalladamente en `CHANGELOG.md`.
- Los acuerdos internos y notas se organizan en `docs/reuniones/`.
