# Pure CSS Bottom Tooltip Component

## What does this do?
This adds a lightweight, pure CSS tooltip component that appears directly underneath an element. It features a smooth fade-in and slide-up transition and includes a tiny CSS arrow pointing to the host element.

## How is it used?
Wrap the host element (like a button or a word) inside a container with the `.tooltip-wrapper` class. Place the tooltip text inside a sibling element with the `.tooltip-bottom` class.

Example:
```html
<div class="tooltip-wrapper" tabindex="0">
  <button>Hover me</button>
  <div class="tooltip-bottom" role="tooltip">This is the tooltip text</div>
</div>
```

*Note: Adding `tabindex="0"` to the wrapper ensures the tooltip is keyboard accessible via focus.*

## Why is it useful?
- Enhances accessibility and UI clarity by providing context on demand without cluttering the screen.
- A pure CSS implementation is highly performant because it avoids JavaScript event listeners (no `mouseenter` or `mouseleave` required).
- Completely isolated and works out of the box with zero dependencies.
