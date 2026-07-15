# Accessibility

Accessibility is a core design principle of **Minimal Motion SVG**.

Every component is designed to be visually clear, lightweight and usable by the widest possible audience.

Accessibility is considered from the first design iteration and is not treated as an optional feature.

---

# Goals

The project aims to:

* Reduce unnecessary visual complexity
* Communicate interface states clearly
* Respect user accessibility preferences
* Provide semantic SVG metadata
* Support assistive technologies whenever possible

---

# Semantic SVG

Every SVG component should include semantic metadata.

At minimum:

```xml
<svg
    role="img"
    aria-labelledby="title desc">

<title id="title">
Component title
</title>

<desc id="desc">
Component description
</desc>

...
</svg>
```

These elements help screen readers identify the purpose of the graphic.

---

# Alternative Text

When using an SVG with the `<img>` element, always provide meaningful alternative text.

Example:

```html
<img
    src="video-loader-blue.svg"
    alt="Loading video">
```

If the animation is purely decorative:

```html
<img
    src="video-loader-blue.svg"
    alt="">
```

Decorative graphics should not introduce unnecessary verbosity for assistive technologies.

---

# Reduced Motion

Many users prefer reduced motion due to vestibular disorders, migraines or other accessibility needs.

All animated components should respect the user's operating system preference.

Example:

```css
@media (prefers-reduced-motion: reduce){

    .animated-element{

        animation:none;

    }

}
```

Whenever animation is disabled, the component should remain visually understandable.

---

# Motion Principles

Animations should communicate interface state without distracting users.

Preferred characteristics:

* smooth
* continuous
* predictable
* meaningful
* calm

Avoid:

* flashing elements
* abrupt transitions
* excessive speed
* unnecessary motion
* distracting visual effects

Motion should support usability rather than compete for attention.

---

# Color and Contrast

Components should maintain sufficient contrast against their intended backgrounds.

Current themes:

## Light Theme

Dark blue animation on transparent background.

## Dark Theme

White animation on transparent background.

Avoid relying on color alone to communicate interface state.

---

# Responsive Rendering

SVG components should remain sharp at any resolution.

The project uses:

* scalable vector graphics
* transparent backgrounds
* non-scaling strokes when appropriate

Components should render correctly from small interface icons to larger previews.

---

# Keyboard Accessibility

SVG components themselves are not interactive.

Interactive controls surrounding the SVG should:

* be keyboard accessible
* have visible focus indicators
* include accessible names
* support standard keyboard navigation

---

# Screen Readers

Animated SVG components should never be the only mechanism used to communicate application state.

For example:

Instead of displaying only a spinner,

provide accompanying text such as:

```
Loading video...
```

or

```
Generating content...
```

This improves accessibility for users relying on assistive technologies.

---

# Decorative vs Informative Graphics

Decorative SVGs:

* should use an empty `alt` attribute
* should not receive keyboard focus

Informative SVGs:

* should include meaningful descriptions
* should communicate application state clearly

---

# Browser Support

Accessibility features rely on modern browser support for:

* SVG
* CSS animations
* `prefers-reduced-motion`

The project targets current versions of major browsers.

---

# Accessibility Checklist

Before publishing a new component, verify:

* SVG is valid
* `<title>` is present
* `<desc>` is present
* `role="img"` is defined
* `prefers-reduced-motion` is supported
* motion is smooth and meaningful
* contrast is sufficient
* animation communicates state clearly
* no flashing or distracting effects
* responsive rendering is preserved

---

# Accessibility Philosophy

Minimal Motion SVG follows the principle that accessibility should be built into every component rather than added later.

A lightweight animation is only successful if it remains understandable, comfortable and inclusive for all users.
