# Terminal Style Examples

Experimentation in this repository for various website design ideas that are minimalistic & represent the terminal design and TUI interfaces.

## Drafts

View the index page for links to concepts of elements that I might like.

## Functionality

For the o just  tll function, I want the menu to have a concept of the element's top so that if it is a solid bar it scrolls it down corrently & if it is a split box then it appropriately handles it. If there is a title to the block, it should convert it to just a straight line cause there may be embeddeded images, etc.

## Width

Max with of 768 pixels Tailwind md for the border of the sections & center on page. Add spacing when go down to the sm of 640px or less for mobile devices.

## Themes

This will allow a ultiple number of themes that will be defaulted per site & saved in user's profile if selected in menu. I'm just going to use these arch linux themes:

- catppuccin
- catpuccin-latte
- ethereal
- everforest
- gold-rush
- gruvbox
- hackerman
- kanagawa
- mars
- matte-black
- nagai-poolside
- neovoid
- nord
- osaka-jade
- retropc
- ristretto
- rose-pine
- tokyo-night

## Theme Usage with Tailwind CSS

This application utilizes **12 distinct themes** managed by **CSS Custom Properties (CSS variables)** and the `data-theme` attribute on the `<html>` element. Instead of defining variables like --color-red-500, variables are defined based on their purpose in the application (semantic naming). This ensuress utility classes remain consistent across all themes.

### **How it Works:**

1.  **Semantic Variables:** Tailwind CSS is configured to use semantic variable names (e.g., `primary`, `base-100`), which map directly to CSS custom properties (e.g., `--color-primary`).
2.  **Theme Definition:** Each theme's color values are defined within a dedicated CSS selector, such as `[data-theme='dark']` or `[data-theme='ocean-blue']`, overriding the default values.
3.  **Activation:** Themes are switched dynamically at runtime by changing the `data-theme` attribute on the root `<html>` tag using JavaScript.

### **Example:**

To apply a theme, set the attribute:

```javascript
document.documentElement.setAttribute('data-theme', 'ocean-blue');
```

The app's utility classes (e.g., `bg-primary`, `text-base-content`) will automatically reflect the selected theme's colors.

