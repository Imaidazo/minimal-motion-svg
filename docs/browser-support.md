# Browser Support

This document describes the browser compatibility, rendering behavior and implementation considerations for **Minimal Motion SVG**.

The project is designed to work with all modern browsers that support SVG and CSS animations without requiring JavaScript or additional runtime dependencies.

---

# Supported Browsers

Minimal Motion SVG is tested against current versions of the following browsers:

| Browser         | Support |
| --------------- | :-----: |
| Google Chrome   |    ✅    |
| Microsoft Edge  |    ✅    |
| Mozilla Firefox |    ✅    |
| Safari          |    ✅    |
| Opera           |    ✅    |
| Brave           |    ✅    |
| Arc             |    ✅    |

The library targets browsers that fully support:

* SVG 1.1
* CSS Animations
* CSS Transforms
* CSS Variables
* Media Queries
* `prefers-reduced-motion`

---

# Mobile Browsers

Minimal Motion SVG is fully compatible with modern mobile browsers.

| Browser          | Android | iOS |
| ---------------- | :-----: | :-: |
| Chrome           |    ✅    |  —  |
| Firefox          |    ✅    |  —  |
| Edge             |    ✅    |  —  |
| Safari           |    —    |  ✅  |
| Samsung Internet |    ✅    |  —  |

---

# Rendering

All components are vector-based and scale without loss of quality.

SVG rendering is resolution-independent and suitable for:

* Desktop applications
* Mobile applications
* Responsive websites
* Progressive Web Apps (PWAs)
* High-DPI displays
* Retina displays

---

# Embedding Methods

The recommended embedding methods are:

### HTML Image

```html
<img
    src="src/loaders/video-loader-blue.svg"
    alt="Loading video">
```

---

### HTML Object

```html
<object
    type="image/svg+xml"
    data="src/loaders/video-loader-blue.svg">
</object>
```

---

### Inline SVG

Inline SVG is also supported when direct customization of the markup is required.

This approach allows complete control over styling and animation.

---

# CSS Compatibility

The project uses only modern CSS features with broad browser support.

Current features include:

* CSS Animations
* CSS Transforms
* CSS Variables
* Media Queries
* Opacity
* Stroke animation
* Transform Origin

No experimental browser APIs are required.

---

# Reduced Motion

All components respect the user's operating system accessibility preferences.

When the browser reports:

```css
prefers-reduced-motion: reduce
```

Animations are automatically simplified or disabled whenever appropriate.

This improves accessibility for users with vestibular disorders or motion sensitivity.

---

# Transparent Backgrounds

Every component uses a transparent background.

This allows seamless integration into:

* Light interfaces
* Dark interfaces
* Custom themes
* Images
* Videos
* Documentation
* Presentation slides

---

# Browser Limitations

Older browsers that lack support for CSS animations or SVG rendering may display static graphics instead of animated components.

Legacy browsers such as Internet Explorer are **not supported**.

---

# Performance

SVG animations are generally more lightweight than GIF animations because they:

* remain vector-based
* require significantly smaller file sizes
* scale without quality loss
* avoid frame-by-frame image decoding

This makes SVG particularly suitable for modern user interfaces.

---

# Accessibility

Browser support also includes accessibility features such as:

* semantic SVG structure
* `<title>`
* `<desc>`
* `role="img"`
* reduced-motion support

Whenever possible, meaningful alternative text should be provided by the embedding application.

---

# Future Compatibility

Minimal Motion SVG follows established web standards.

Future components will continue using standardized SVG and CSS features to maximize long-term browser compatibility while avoiding vendor-specific implementations.

---

# Summary

Minimal Motion SVG supports all modern browsers and mobile platforms that implement standard SVG and CSS animation features.

The project intentionally avoids proprietary technologies and JavaScript dependencies to ensure long-term compatibility, high performance and broad portability across web and mobile environments.
