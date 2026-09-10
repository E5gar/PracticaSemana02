# DEBUG_LOG.md — Parte 1: HTML5, CSS3 y Diseño Responsivo

## A. W3C Validator (Nu Html Checker)

### Primera ejecución
- **Errors:** 0
- **Warnings:** 2

**Warning 1**
- Elemento: `<nav role="navigation" aria-label="Menu principal">`
- Mensaje: *"The `navigation` role is unnecessary for element `nav`"*
- Ubicación: línea 16
- **Corrección manual:** se eliminó el atributo `role="navigation"` del `<nav>`, dejando solo `aria-label="Menu principal"`, ya que la etiqueta `<nav>` ya implica ese rol semántico de forma nativa (rol redundante).

**Warning 2**
- Elemento: `<section id="tarjetas">`
- Mensaje: *"Section lacks heading. Consider using h2-h6 elements..."*
- Ubicación: línea 33
- **Corrección manual:** se añadió un encabezado (`<h2>`) dentro de la sección `tarjetas` para darle un título identificable, en lugar de dejarla como contenedor genérico.

### Segunda ejecución
- **Errors:** 0
- **Warnings:** 0
- Resultado: *"Document checking completed. No errors or warnings to show."*

---

## B. WAVE (Web Accessibility Evaluation Tool)

- **Errors:** 0
- **Contrast Errors:** 0
- **Alerts:** 0
- **Features:** 1 (Language)
- **Structural Elements:** 12
  - Heading level 1: 1
  - Heading level 2: 1
  - Heading level 3: 5
  - Unordered list: 1
  - Header: 1
  - Navigation: 1
  - Main content: 1
- **ARIA:** 1 (`aria-label="Menu principal"`)
- **AIM Score:** 10 out of 10

---

## C. Google Lighthouse

- **URL evaluada:** `http://127.0.0.1:5500/parte1/index.html#pie`
- **Dispositivo:** Emulated Mobile

| Categoría | Puntuación Obtenida | Rúbrica |
|---|---|---|
| **Performance** | **100** | Cumple |
| **Accessibility** | **100** | Cumple |
| **Best Practices** | **100** | Cumple |
| **SEO** | **100** | Cumple |