# Repo Structure (VictorOPEX)

Este documento describe la estructura actual del repo y las convenciones para mantenerlo coherente.

## Que es "produccion" aqui

- `README.md` es el artefacto principal: GitHub Profile README.
- Todo lo que `README.md` referencia con rutas locales debe existir y estar trackeado en Git.

## Carpetas

### `images/` (tracked)

Assets que si se publican y se consumen desde `README.md` y docs:

- `images/github-banner.gif`: banner activo (archivo "canonico", sin espacios).
- `images/icons-carousel.gif`: carrusel animado del stack (se regenera).
- `images/divider.gif`: divisor/linea.
- `images/latest-articles-featured.svg`: asset usado como placeholder/ejemplo.
- `images/archive/`: variantes antiguas (trackeadas) para referencia.
- `images/drafts/`: experiments locales (IGNORADO por `.gitignore`).

Regla: si un asset esta en `images/` (fuera de `drafts/`), debe tener un nombre estable y ser apto para GitHub (tamaño/peso razonable).

### `assets/` (local scratch, ignored)

`assets/` se usa como carpeta local para pruebas/plantillas y no forma parte del README publicado.

Diferencia vs `images/`:
- `images/` = assets versionados y usados por el README final.
- `assets/` = borradores/local-only (no garantizado que exista en GitHub).

Nota: por esta razon, los ejemplos de `README_COMPONENTS.md` deben usar `images/` o URLs remotas, no `assets/`.

### `scripts/`

- `scripts/gen_icons_carousel.py`: genera `images/icons-carousel.gif` leyendo `STACK_ICONS.md`.

### `.github/workflows/`

- `icons-carousel.yml`: workflow que regenera y commitea `images/icons-carousel.gif` cuando cambie `STACK_ICONS.md` o el script.

## Archivos clave (source of truth)

- `STACK_ICONS.md`: fuente de verdad de filas `skillicons.dev` para el carrusel.
- `README_LAYOUT_RULES.md`: reglas de layout/medidas para mantener consistencia.
- `README_TEXT_STYLES.md`: galeria de estilos de texto (preview + snippets).
- `README_COMPONENTS.md`: plantilla de componentes reutilizables (ejemplos).

## Convenciones de nombres (recomendado)

- Evitar espacios en nombres de archivos versionados.
- Preferir `kebab-case`:
  - `github-banner.gif`
  - `icons-carousel.gif`
- Mantener variantes antiguas en `images/archive/` con sufijo numerico:
  - `github-banner-2.svg`, etc.

## Auditoria de coherencia (checks)

Antes de push:

1. `README.md` no debe referenciar rutas que no existen.
2. Los ejemplos en `README_COMPONENTS.md` deben usar assets que existen en el repo o URLs remotas.
3. `STACK_ICONS.md` contiene las URLs `skillicons.dev` que el script parsea.
4. `images/drafts/` solo contiene archivos locales (no se comitea).

