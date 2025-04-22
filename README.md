# Tailwind CSS Documentation & Examples

![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

A comprehensive guide to Tailwind CSS with practical examples and explanations.

## Overview

Tailwind CSS is a utility-first CSS framework that allows you to build modern websites without ever leaving your HTML. This documentation provides examples and explanations for all Tailwind CSS features.

## Features Covered

- **Utility-First Approach**: Learn how Tailwind's utility classes work
- **Colors**: Explore Tailwind's color palette system
- **Container & Spacing**: Master layout spacing and containers
- **Typography**: Text styling and formatting
- **Sizing**: Control element dimensions with ease
- **Layout & Position**: Positioning and layout utilities
- **Backgrounds & Shadows**: Apply backgrounds and drop shadows
- **Borders**: Border styling and border radius
- **Filters**: Visual filters for images and elements
- **Interactivity**: Hover, focus, and other interactive states
- **Responsive Design**: Breakpoint system for responsive layouts
- **Column Layouts**: Multi-column layout techniques
- **Flexbox**: Flexible box layout system
- **Grid**: CSS Grid implementation
- **Transforms & Transitions**: Element transformations and transitions
- **Animation**: Built-in animation utilities
- **Customization**: Configure and extend Tailwind
- **Dark Mode**: Implement dark mode with Tailwind

## Getting Started

Each section contains practical examples showing Tailwind classes in action. To get started:

1. Browse the individual sections in the `/01-utility-first/` through `/18-dark-mode/` directories
2. View the examples in your browser to see how they work
3. Examine the HTML to understand how the classes are applied

## Installation

For this project, we're using the CDN version of Tailwind CSS:

```html
<script src="https://cdn.tailwindcss.com"></script>
```

For production projects, consider using npm:

```bash
npm install -D tailwindcss
npx tailwindcss init
```

## Tailwind CSS vs Traditional CSS

### Traditional CSS Approach

Using traditional CSS requires defining styles separately:

```css
/* CSS file */
.button {
  background-color: blue;
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 0.25rem;
}
```

```html
<!-- HTML file -->
<button class="button">Click Me</button>
```

### Tailwind Approach

With Tailwind, you apply utility classes directly in HTML:

```html
<button class="bg-blue-500 text-white py-2 px-4 rounded">
  Click Me
</button>
```

### Benefits of Tailwind's Approach

- **No naming conventions to invent** - Focus on building components, not naming CSS classes
- **Faster development** - Make changes directly in your HTML without switching to CSS files
- **Smaller CSS bundle** - Ship only the CSS you're actually using
- **Responsive design made simple** - Use responsive modifiers like `md:` or `lg:` directly in your HTML

## Example Sections

Browse the following sections to learn more:

- [01-utility-first](./01-utility-first/index.html)
- [02-colors](./02-colors/index.html)
- [03-container-spacing](./03-container-spacing/index.html)
- ...and many more!

## Resources

- [Tailwind CSS Official Documentation](https://tailwindcss.com/docs)
- [Tailwind CSS GitHub Repository](https://github.com/tailwindlabs/tailwindcss)
- [Tailwind UI Components](https://tailwindui.com/)

---

Created by [Prajwal Chandra Nayak](https://github.com/PrajwalChNayak)
