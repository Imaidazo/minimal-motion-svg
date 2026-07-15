# Minimal Motion SVG

> Lightweight, modern and accessible animated SVG components for web and mobile applications.

[![Live Demo](https://img.shields.io/badge/demo-online-success.svg)](https://svgs.isavit.dev/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-0.1.0-informational.svg)](CHANGELOG.md)
[![Pure SVG](https://img.shields.io/badge/Pure-SVG-ff69b4.svg)](docs/architecture.md)
[![No JavaScript](https://img.shields.io/badge/JavaScript-Not%20Required-success.svg)](docs/performance.md)
![Status](https://img.shields.io/badge/status-active-success.svg)

---

## Overview

**Minimal Motion SVG** is an open-source collection of lightweight, modern and accessible animated SVG components designed for web and mobile applications.

The project focuses on delivering production-ready micro-animations that require **no JavaScript**, have **zero runtime dependencies**, and integrate seamlessly into modern user interfaces.

Each component is distributed as a standalone SVG file with embedded CSS animation, making it easy to use in virtually any framework or platform.

🌐 **Live Demo:** https://svgs.isavit.dev/

---

## Features

* Pure SVG animations
* Zero JavaScript dependencies
* Lightweight and optimized assets
* Transparent backgrounds
* Responsive vector rendering
* Infinite and seamless animation loops
* Light and Dark interface variants
* Accessible by default
* `prefers-reduced-motion` support
* Easy integration into existing projects
* Easy customization through SVG and CSS

---

## Current Components

### Loaders

| Component    | Light Theme | Dark Theme | Status |
| ------------ | :---------: | :--------: | :----: |
| Video Loader |      ✅      |      ✅     | Stable |

---

## Project Structure

```text
minimal-motion-svg/
│
├── src/
│   └── loaders/
│       ├── video-loader-blue.svg
│       └── video-loader-white.svg
│
├── demo/
│   ├── index.html
│   └── assets/
│       ├── css/
│       └── js/
│
├── README.md
├── CHANGELOG.md
├── ROADMAP.md
├── CONTRIBUTING.md
├── LICENSE
└── .gitignore
```

---

## Usage

### HTML

```html
<img
    src="src/loaders/video-loader-blue.svg"
    alt="Loading video"
    width="180"
    height="211">
```

---

### HTML Object

```html
<object
    type="image/svg+xml"
    data="src/loaders/video-loader-blue.svg"
    aria-label="Loading video">
</object>
```

---

### CSS Background

```css
.video-loader{

    width:180px;

    aspect-ratio:512/600;

    background:

        center / contain

        no-repeat

        url("../src/loaders/video-loader-blue.svg");

}
```

---

## Theme Selection

### Light Interfaces

```text
src/loaders/video-loader-blue.svg
```

### Dark Interfaces

```text
src/loaders/video-loader-white.svg
```

> The white version uses a transparent background and is intended for dark user interfaces.

---

## Accessibility

Every component includes:

* Semantic SVG structure
* `<title>` element
* `<desc>` element
* `role="img"`
* `prefers-reduced-motion` support

When using decorative animations, prefer:

```html
<img src="..." alt="">
```

When the animation communicates interface state:

```html
<img
    src="..."
    alt="Loading video">
```

---

## Design Principles

Every component in the library follows the same design language.

* Minimal visual language
* Smooth and meaningful motion
* Stable animations
* Thin and consistent line weights
* Transparent backgrounds
* Lightweight implementation
* Production-ready quality
* Accessibility by default
* Zero runtime dependencies
* Consistent visual identity

---

## Browser Support

Minimal Motion SVG works in all modern browsers supporting SVG and CSS animations.

* Chrome
* Edge
* Firefox
* Safari
* Opera
* Brave
* Arc

---

## Roadmap

Upcoming categories include:

* AI Processing
* Search
* Upload
* Download
* Status
* Media
* Navigation
* Empty States
* System Components

See the complete roadmap in:

* [ROADMAP.md](ROADMAP.md)

---

## Documentation

Additional documentation is available in:

* [CHANGELOG.md](CHANGELOG.md)
* [ROADMAP.md](ROADMAP.md)
* [CONTRIBUTING.md](CONTRIBUTING.md)

---

## Contributing

Contributions are welcome.

Before submitting a contribution, please read:

* [CONTRIBUTING.md](CONTRIBUTING.md)

Every new component should preserve the project's visual language, accessibility standards and technical consistency.

---

## Versioning

This project follows **Semantic Versioning**.

Current version:

**v0.1.0**

---

## License

Released under the **MIT License**.

See the complete license in:

* [LICENSE](LICENSE)

---

## Author

**Sandra dos Santos Vitoriano**

---

## Acknowledgements

Minimal Motion SVG was created to provide a lightweight, elegant and reusable collection of animated SVG components for modern user interfaces, emphasizing performance, accessibility and long-term maintainability.
