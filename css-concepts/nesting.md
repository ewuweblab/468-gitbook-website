# Nesting

## Why?

1. **Improved Code Organization**\
   CSS nesting allows you to write more logically structured code that mirrors your HTML hierarchy. This makes your stylesheets easier to read and maintain as related styles are grouped together.
2. **Reduced Selector Repetition**\
   With nesting, you can avoid repeatedly writing the same parent selectors, resulting in cleaner code with less redundancy. This makes your CSS more concise and easier to work with.
3. **Better Specificity Management**\
   Nesting helps maintain appropriate specificity levels without resorting to unnecessary ID selectors or !important declarations, leading to more predictable styling behavior and fewer specificity conflicts.
4. **Enhanced Modularity**\
   By keeping related styles together, components become more self-contained and modular. This approach aligns well with component-based development methodologies like those used in modern frameworks.
5. **Native Browser Support**\
   CSS nesting is now supported natively in all major browsers, eliminating the need for preprocessors like Sass or Less solely for this feature, which simplifies your development toolchain.

## How?

```
/* Without nesting */
.card { background: white; }
.card .title { font-size: 1.2rem; }
.card .body { padding: 1rem; }
.card .footer { border-top: 1px solid #eee; }

/* With nesting */
.card {
  background: white;
  
  .title { font-size: 1.2rem; }
  .body { padding: 1rem; }
  .footer { border-top: 1px solid #eee; }
}

```

&#x20;`&` symbol is essential when you need to reference the parent selector itself rather than creating a descendant selector relationship. Without it, the CSS engine assumes you're targeting a child element.

```
.nav-link {
  color: black;
  
  &:hover,
  &:focus {
    color: blue;
  }
  
  &::before {
    content: "→";
  }
}
```

## References

{% embed url="https://ishadeed.com/article/css-nesting/" %}

{% embed url="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_nesting/Using_CSS_nesting" %}
