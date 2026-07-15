# Frequently Asked Questions (FAQ)

Welcome to the **Minimal Motion SVG** FAQ.

This document answers the most common questions about the project, its philosophy and its technical implementation.

---

# What is Minimal Motion SVG?

Minimal Motion SVG is an open-source collection of lightweight, modern and accessible animated SVG components for web and mobile applications.

The project focuses on creating production-ready interface animations that require no JavaScript and have zero runtime dependencies.

---

# Why use SVG instead of GIF?

SVG offers several advantages over GIF:

* Infinite scalability without quality loss
* Smaller file sizes
* Better rendering on high-resolution displays
* Native CSS animation support
* Better accessibility
* Easy customization
* Transparent backgrounds
* Better integration with modern web technologies

---

# Why doesn't the project use JavaScript?

The goal of Minimal Motion SVG is to keep every component completely self-contained.

Using only SVG and embedded CSS provides:

* Better performance
* Zero runtime dependencies
* Easier integration
* Improved portability
* Simpler maintenance

---

# Can I use these animations commercially?

Yes.

Minimal Motion SVG is released under the MIT License, allowing both personal and commercial use.

Please refer to the LICENSE file for the complete license terms.

---

# Do I need to credit the project?

The MIT License does not require visible attribution in your application.

However, the copyright notice and license must be preserved in copies or substantial portions of the software, as required by the license.

If you find the project useful, starring the GitHub repository is greatly appreciated.

---

# Can I modify the SVG files?

Absolutely.

The SVG files are intended to be customized.

You may change:

* Colors
* Dimensions
* Animation speed
* Stroke thickness
* Timing
* Text
* Motion behavior

---

# Can I remove the "Carregando" text?

Yes.

The loading text is part of the SVG and can be removed or replaced to match your application's language and design.

---

# Are the animations responsive?

Yes.

All components are vector-based and scale without losing quality.

---

# Which browsers are supported?

Minimal Motion SVG supports all modern browsers that implement SVG and CSS animations, including:

* Chrome
* Edge
* Firefox
* Safari
* Opera
* Brave
* Arc

---

# Does the project support dark mode?

Yes.

Whenever appropriate, components are provided in separate variants optimized for light and dark user interfaces.

---

# Does the project support accessibility?

Yes.

Every component is designed with accessibility in mind.

Whenever possible, SVG files include:

* `role="img"`
* `<title>`
* `<desc>`
* Support for `prefers-reduced-motion`

Applications should also provide appropriate alternative text when the animation conveys interface state.

---

# Why are there separate light and dark versions?

Separate versions ensure:

* Better visual contrast
* Consistent appearance
* Improved readability
* Simpler integration

This approach also avoids unnecessary runtime color manipulation.

---

# Why doesn't the white SVG appear when I open it?

The white version uses a transparent background.

When opened in viewers with a white canvas, it may appear invisible.

It is intended for use on dark user interfaces.

---

# Can I contribute?

Yes.

Contributions are welcome.

Please read the project's **CONTRIBUTING.md** before submitting pull requests or proposing new components.

---

# How are new components developed?

Every new component follows the project's development workflow:

1. Create a single master component.
2. Review animation quality and visual consistency.
3. Approve the master component.
4. Generate light, dark and other variants.
5. Update the documentation.
6. Update the demo catalogue.
7. Record the release in the changelog.

This workflow maintains consistency throughout the library.

---

# Will JavaScript components ever be added?

No.

Minimal Motion SVG is intentionally focused on pure SVG animations.

Projects requiring JavaScript, Canvas or WebGL are outside the scope of this library.

---

# What types of components are planned?

Future releases may include:

* AI Processing
* AI Thinking
* Upload
* Download
* Search
* Synchronization
* Success
* Error
* Warning
* Empty States
* Navigation
* Media Controls
* System Indicators

See **ROADMAP.md** for the complete project roadmap.

---

# Where can I report a bug?

Bug reports, feature requests and suggestions can be submitted through the project's GitHub Issues page.

Please include:

* Browser
* Operating system
* Component name
* Steps to reproduce
* Expected behavior
* Actual behavior

Screenshots or screen recordings are always helpful.

---

# Where can I see the animations in action?

The latest public demonstration is available at:

**https://svgs.isavit.dev/**

---

# Still have a question?

If your question is not answered here, please open a discussion or submit an issue on the GitHub repository.

Community feedback helps improve the project for everyone.
