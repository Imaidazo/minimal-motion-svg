# Contributing to Minimal Motion SVG

First of all, thank you for considering contributing to **Minimal Motion SVG**.

Whether you are reporting a bug, suggesting an improvement, improving the documentation or creating a new animated SVG component, your contribution is greatly appreciated.

Our goal is to build a lightweight, modern and accessible collection of production-ready animated SVG components for web and mobile applications.

---

# Project Philosophy

Every component in this library should follow the same principles.

* Pure SVG
* No JavaScript dependencies
* Transparent background
* Lightweight implementation
* Responsive rendering
* Accessibility by default
* Smooth and meaningful motion
* Consistent visual language
* Production-ready quality

Visual simplicity is preferred over visual complexity.

Animations should communicate interface state clearly without distracting the user.

---

# Before You Start

Please read the following documents before contributing:

* README.md
* ROADMAP.md
* CHANGELOG.md

Understanding the project's goals helps maintain consistency across all components.

---

# Development Workflow

Each new component follows the same workflow.

## 1. Create a Master Component

Only one SVG should be created initially.

This is called the **Master Component**.

The master component is reviewed before any additional variants are created.

---

## 2. Review

During review we evaluate:

* proportions
* animation quality
* visual consistency
* accessibility
* performance
* file size
* rendering quality

Only after approval are new variants generated.

---

## 3. Generate Variants

Once the master component is approved, additional variants may be created.

Examples:

* Light theme
* Dark theme
* Alternative colors
* Different sizes

This workflow avoids duplicated work and keeps the project consistent.

---

# Technical Requirements

Every SVG must:

* be valid SVG
* contain a transparent background
* include embedded CSS only
* avoid JavaScript
* avoid external dependencies
* scale correctly
* support responsive rendering
* contain semantic SVG elements
* include `<title>`
* include `<desc>`
* support `prefers-reduced-motion`

---

# Animation Guidelines

Animations should be:

* smooth
* continuous
* meaningful
* calm
* visually balanced

Avoid:

* abrupt movements
* unnecessary effects
* flashing elements
* distracting animations
* excessive rotation speeds

Animations should enhance the interface rather than compete with it.

---

# Design Guidelines

Use:

* minimalist shapes
* consistent proportions
* subtle motion
* thin and balanced strokes
* transparent backgrounds

Avoid:

* gradients
* shadows
* filters
* textures
* excessive detail

The project intentionally follows a minimalist visual language.

---

# File Naming

Use lowercase kebab-case.

Examples:

```text
video-loader-blue.svg
video-loader-white.svg
ai-processing-blue.svg
upload-loader-white.svg
```

---

# Directory Structure

Components should be placed in the appropriate directory.

```text
src/

    loaders/

    processing/

    status/

    navigation/

    media/

    system/
```

Create a new category only when an existing one is not appropriate.

---

# Commit Messages

Write short and descriptive commit messages.

Examples:

```text
Add AI processing loader

Improve ripple animation

Reduce stroke thickness

Update documentation

Fix accessibility metadata
```

---

# Pull Requests

A good pull request should include:

* a clear description
* screenshots or previews when applicable
* motivation for the change
* accessibility considerations
* documentation updates when necessary

Small, focused pull requests are preferred over large unrelated changes.

---

# Reporting Issues

When opening an issue, please include:

* browser
* operating system
* SVG component
* steps to reproduce
* expected behavior
* actual behavior

Screenshots or screen recordings are always helpful.

---

# Accessibility

Accessibility is a core requirement of this project.

Every component should:

* remain understandable without color alone
* support reduced-motion preferences
* include semantic SVG metadata
* preserve sufficient visual contrast

Accessibility is not considered optional.

---

# Performance

Components should remain lightweight.

Whenever possible:

* minimize SVG markup
* reuse shapes
* avoid unnecessary path complexity
* avoid excessive animation calculations

Smaller files improve loading performance.

---

# Versioning

This project follows Semantic Versioning.

Changes affecting existing components should be documented in the CHANGELOG before release.

---

# Code of Conduct

Please be respectful and constructive.

We value collaboration, kindness and technical excellence.

---

# License

By contributing to this project, you agree that your contributions will be released under the MIT License.

Thank you for helping improve **Minimal Motion SVG**.
