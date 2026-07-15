# Getting Started

Welcome to **Minimal Motion SVG**.

This guide will help you integrate Minimal Motion SVG components into your projects in just a few minutes.

No build tools, JavaScript libraries or package managers are required.

---

# What is Minimal Motion SVG?

Minimal Motion SVG is an open-source collection of lightweight, modern and accessible animated SVG components for web and mobile applications.

Every component is:

* Pure SVG
* Self-contained
* Lightweight
* Responsive
* Transparent
* Accessible
* Production-ready

---

# Installation

No installation is required.

Simply download the SVG file you want to use and include it in your project.

Current components are located in:

```text
src/loaders/
```

Example:

```text
video-loader-blue.svg
video-loader-white.svg
```

---

# Basic Usage

## HTML Image

The simplest integration method.

```html
<img
    src="src/loaders/video-loader-blue.svg"
    alt="Loading video"
    width="180"
    height="211">
```

---

## HTML Object

Useful when you need full SVG interaction.

```html
<object
    type="image/svg+xml"
    data="src/loaders/video-loader-blue.svg"
    aria-label="Loading video">
</object>
```

---

## CSS Background

Ideal for interface elements.

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

# Choosing a Theme

Two themes are currently available.

## Light Interface

Use:

```text
video-loader-blue.svg
```

Designed for light user interfaces.

---

## Dark Interface

Use:

```text
video-loader-white.svg
```

Designed for dark user interfaces.

The SVG uses a transparent background.

---

# Responsive Behavior

SVG components scale without losing quality.

Example:

```css
.loader{

    width:96px;

}
```

or

```css
.loader{

    width:240px;

}
```

The animation remains smooth at any size.

---

# Accessibility

Minimal Motion SVG follows accessibility best practices.

Each component includes:

* semantic SVG
* title
* description
* role="img"
* reduced-motion support

When the animation is decorative:

```html
<img
    src="..."
    alt="">
```

When it communicates interface state:

```html
<img
    src="..."
    alt="Loading video">
```

---

# Performance

All components are optimized for performance.

Design goals include:

* minimal SVG markup
* lightweight files
* embedded CSS animations
* zero runtime dependencies
* hardware-accelerated rendering when supported by the browser

---

# Browser Support

Minimal Motion SVG supports all modern browsers.

* Chrome
* Edge
* Firefox
* Safari
* Opera
* Brave
* Arc

---

# Customization

Most components can be customized.

Typical customizations include:

* color
* size
* animation speed
* positioning

Future releases will introduce additional customization options.

---

# Live Demo

Explore all available components:

https://svgs.isavit.dev/

---

# Source Code

GitHub Repository:

https://github.com/Imaidazo/minimal-motion-svg

---

# Next Steps

After integrating your first component, you may want to explore:

* Architecture
* Accessibility
* Performance
* Customization
* Roadmap

These documents explain the design philosophy and technical decisions behind the project.

---

# Need Help?

If you encounter a problem or have a suggestion, please:

* open an Issue on GitHub
* submit a Pull Request
* contribute to the documentation

Community contributions are always welcome.
