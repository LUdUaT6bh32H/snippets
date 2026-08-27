# ARIA Attribute Quick Reference

Common ARIA attributes for accessible component patterns.

## `aria-label`

Overrides an element’s accessible name when no visible label exists.

```html
<button aria-label="Close" class="close-btn">×</button>
```

## `aria-expanded`

Indicates whether an expandable element is currently expanded or collapsed.

```html
<button aria-expanded="false" aria-controls="mobile-menu">
  Menu
</button>
```

## `aria-controls`

References the element controlled by the current interactive element.

```html
<button aria-expanded="true" aria-controls="faq-panel">
  FAQ
</button>
<div id="faq-panel">…</div>
```

## `aria-live`

Announces dynamic content updates to screen readers.

```html
<div aria-live="polite" role="status">
  Your changes have been saved.
</div>
```

## `aria-describedby`

Adds additional descriptive text to an element’s accessible name.

```html
<label for="email">Email</label>
<input id="email" type="email" aria-describedby="email-hint" />
<p id="email-hint">We’ll never share your email.</p>
```

## `aria-hidden`

Removes decorative or duplicate content from the accessibility tree.

```html
<span aria-hidden="true">★</span>
```

Use these attributes intentionally and test with a screen reader.
