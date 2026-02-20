# Text Motion Styles (README)

Este archivo es una galeria de estilos para el texto animado del header (GitHub Profile README).

Limitacion: en GitHub README no podemos usar JS/CSS propio; el movimiento normalmente viene de una imagen (GIF/APNG) o de un servicio que genera SVG como imagen. Aqui usamos `readme-typing-svg`.

## Quick Use

1. Copia un snippet.
2. Cambia el contenido de `lines=...` (recuerda URL-encode: espacios `+`, coma `,` como `%2C`, `&` como `%26`).
3. Ajusta `width` y `height` si se corta el texto.

Recomendado (para que no se corte):
- `width`: `900` a `1100`
- `height`: `80` a `110`
- `size`: `36` a `64`

---

## A) Executive Slow (2-3 lineas)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Oxanium&size=34&duration=4200&pause=1300&color=F4F7FB&center=true&vCenter=true&width=1000&lines=Operational+Excellence+powered+by+Data+and+AI;Digital+transformation+for+manufacturing+operations;Analytics%2C+automation%2C+and+continuous+improvement"
    alt="typing"
  />
</p>
```

## B) Fast Terminal (1 linea, feeling consola)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Share+Tech+Mono&size=36&duration=1700&pause=900&color=7CFFCB&center=true&vCenter=true&width=1000&lines=OPEX+%7C+Data+Architecture+%7C+Industrial+AI"
    alt="typing"
  />
</p>
```

## C) Industrial Gold (1 linea, mas sobrio)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Rajdhani&size=46&duration=2400&pause=1100&color=D4AF37&center=true&vCenter=true&width=1000&height=90&lines=Industrial+AI+%C2%B7+Data-Driven+OPEX+%C2%B7+Execution+Governance"
    alt="typing"
  />
</p>
```

## D) Tech Wide (Audiowide)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Audiowide&size=38&duration=2600&pause=1000&color=F4F7FB&center=true&vCenter=true&width=1000&height=90&lines=From+shop+floor+signals+to+executive+decisions"
    alt="typing"
  />
</p>
```

## E) Bold Headline (grande, 1 linea)

Nota: sube `height` para evitar que se corte la parte inferior de letras como `g`, `y`, `p`.

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Audiowide&size=56&duration=1&pause=999999&color=F4F7FB&center=true&vCenter=true&width=900&height=100&lines=Let%27s+work+together"
    alt="headline"
  />
</p>
```

## F) Minimal Clean (sin tanto "tech", muy compatible con GitHub)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Inter&size=36&duration=2600&pause=1000&color=C9CED6&center=true&vCenter=true&width=1000&height=90&lines=Systems+that+scale.+Teams+that+adopt."
    alt="typing"
  />
</p>
```

## G) Ultra Compact (para no ocupar tanto alto)

```html
<p align="center">
  <img
    width="100%"
    src="https://readme-typing-svg.herokuapp.com?font=Oxanium&size=28&duration=2200&pause=900&color=C9CED6&center=true&vCenter=true&width=1000&height=70&lines=OPEX+%C2%B7+Analytics+%C2%B7+Automation"
    alt="typing"
  />
</p>
```

---

## Ideas "diferentes" (sin JS)

Estas opciones requieren imagen animada (GIF/APNG). GitHub las muestra bien, pero hay que generarlas y guardarlas en `images/`.

### 1) Glow sweep (texto fijo con brillo que pasa)

```html
<p align="center">
  <img src="images/text-glow-sweep.gif" alt="glow sweep" width="100%" />
</p>
```

### 2) Ticker / marquee (texto desplazandose)

```html
<p align="center">
  <img src="images/text-ticker.gif" alt="ticker" width="100%" />
</p>
```

### 3) Static + Divider (sin animacion, pero con impacto visual)

```html
<h2 align="center">Operational Excellence powered by Data and AI</h2>
<p align="center"><img src="images/divider.gif" alt="divider" width="100%" /></p>
```

