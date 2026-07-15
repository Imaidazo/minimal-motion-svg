# Customization

Minimal Motion SVG components are designed to be easy to customize while preserving a consistent visual language across the library.

This guide explains the recommended customization options and best practices.

---

# Philosophy

The library follows a simple principle:

> **Customize appearance, not behavior.**

Colors, dimensions and animation speed can be adapted to match an application's design system, while the overall motion language should remain recognizable.

---

# Color

Every component is distributed with two official themes:

* Blue (for light interfaces)
* White (for dark interfaces)

If necessary, colors may be changed by editing the SVG.

Example:

```css
:root{
    --loader-color:#123A73;
}
```

Any valid CSS color may be used.

Examples:

```css
--loader-color:#0F62FE;
--loader-color:#4F46E5;
--loader-color:#009688;
--loader-color:#FFFFFF;
```

Avoid gradients whenever possible.

The project intentionally uses solid colors to maintain clarity and lightweight rendering.

---

# Size

SVG components are fully scalable.

Example:

```html
<img
    src="src/loaders/video-loader-blue.svg"
    width="64"
    height="75"
    alt="Loading">
```

or

```css
.loader{

    width:64px;

}
```

There is no minimum or maximum supported size.

However, sizes below **24 pixels** may reduce visual clarity.

---

# Animation Speed

Animation timing may be adjusted by changing the CSS animation duration.

Original:

```css
animation:spin 2.16s linear infinite;
```

Faster:

```css
animation:spin 1.6s linear infinite;
```

Slower:

```css
animation:spin 2.8s linear infinite;
```

For loading indicators, a moderate and constant speed is recommended.

Abrupt acceleration or deceleration should generally be avoided because it may unintentionally suggest poor application performance.

---

# Stroke Width

Stroke thickness may be adjusted for different visual styles.

Example:

```css
--stroke-core:2px;

--stroke-wave:2px;
```

Increasing stroke width produces a bolder appearance.

Reducing stroke width creates a lighter and more minimalist design.

Maintain proportional relationships between all strokes whenever possible.

---

# Typography

The default font stack is:

```css
Inter,
Manrope,
"SF Pro Display",
"Segoe UI",
Arial,
sans-serif
```

Applications may substitute another font if desired.

The loading text should remain simple and highly legible.

---

# Animation Timing

Ripple timing can be adjusted.

Default:

```css
animation:ripple 2.4s cubic-bezier(.22,.61,.36,1) infinite;
```

Longer ripple durations create a calmer appearance.

Shorter durations communicate faster activity.

---

# Loading Text

The default label is:

```text
Carregando
```

Applications may replace the label.

Examples:

```text
Loading

Processing

Generating

Searching

Uploading

Downloading

Synchronizing
```

The animated dots may also be removed if a simpler presentation is preferred.

---

# Theme Support

Minimal Motion SVG provides dedicated assets for:

* Light interfaces
* Dark interfaces

Applications may automatically switch between them according to the current theme.

Example:

```javascript
const loader =
    prefersDarkMode
        ? "video-loader-white.svg"
        : "video-loader-blue.svg";
```

---

# Accessibility

When customizing a component, preserve:

* `<title>`
* `<desc>`
* `role="img"`
* `prefers-reduced-motion`

These elements are essential for accessibility.

---

# Performance

To preserve performance:

* avoid unnecessary filters
* avoid excessive path complexity
* avoid embedded raster images
* avoid JavaScript animation
* preserve vector geometry whenever possible

SVG components should remain lightweight.

---

# Recommended Customizations

✔ Change color

✔ Change size

✔ Change animation speed

✔ Change loading text

✔ Adapt to application theme

✔ Integrate into existing design systems

---

# Discouraged Customizations

The following modifications are discouraged because they alter the visual identity of the project:

* gradients
* drop shadows
* textures
* heavy blur effects
* complex filters
* multiple colors in a single component
* excessive animation speed
* abrupt motion

---

# Design Consistency

When contributing new components, maintain consistency with the existing collection.

Consistency is more valuable than visual novelty.

Every component should immediately feel like part of the same design system.

---

# Future

As the library grows, additional customization options may become available, including:

* CSS variables
* configurable animation presets
* alternative color palettes
* component themes
* framework-specific wrappers

The core design philosophy will remain focused on simplicity, accessibility and lightweight implementation.
