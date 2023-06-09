# scope-hoc

Demo of a higher-order utility component that returns a type-safe polymorphic component with a scoped version of the CSS class name. Reduces boilerplate by allowing creating components in a single line.

Usage:

```tsx
// <div class='_my-thing-12345'>
const MyThing = ScopedBox('my-thing');

// <span class='_my-thing-12345'>
<MyThing as='span'>...</MyThing>;
```

```tsx
// <a class='_my-link-12345'>
const MyLink = ScopedBox('my-link', 'a');
```

```tsx
// <button type='button' class='_my-button-12345'>
const MyButton = ScopedBox('my-button', 'button', { type: 'button' });
```
