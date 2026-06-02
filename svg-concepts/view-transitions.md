# View Transitions

The View Transitions API animates between two DOM states by capturing a screenshot of the old state, applying your mutation, then crossfading to the new state — all in one call:

```js
document.startViewTransition(() => updateDOM());
```

Without any CSS, you get a free crossfade. To animate a specific element across states, give it a `view-transition-name` — **the same name in both the old and new state** — and the browser interpolates its position and size automatically. Names must be unique per page.

```css
.card { view-transition-name: my-card; }
```

The generated `::view-transition-old()` and `::view-transition-new()` pseudo-elements are what you target to customize:

```css
::view-transition-old(root) { animation: 150ms ease slide-out; }
::view-transition-new(root) { animation: 200ms ease slide-in;  }
```

A few things worth keeping in mind:

* **Always wrap in a fallback.** `document.startViewTransition` doesn't exist in Firefox (without a flag) or older browsers, so `if (!document.startViewTransition) { fn(); return; }` is a one-liner that keeps everything working.
* **The callback can be async.** The browser waits for the returned promise before capturing the new state, so you can `await fetch(...)` inside it for SPA-style page navigations.
* **`view-transition-name` must be unique per page** at the moment the transition fires — duplicates silently break the animation for those elements.
* **MPA support is landing.** Same-origin navigations between separate HTML pages can opt in via `@view-transition { navigation: auto; }` in CSS, no JS required — though browser support is still catching up.

The API is a thin wrapper around what the browser already does when you navigate; it just exposes the hooks.
