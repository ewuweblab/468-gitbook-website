# (Design) Tokens

## Tokens

Design tokens are named entities that store reusable design values like colors, typography, spacing, and animation timing. They serve as the foundational building blocks in design systems, creating a single source of truth that connects design decisions to implementation.

Key characteristics of design tokens:

1. **Abstraction**: They represent design decisions rather than specific values (e.g., "primary-color" instead of "#0047AB")
2. **Hierarchical structure**: Often organized in a semantic hierarchy:
   * Global tokens (most abstract): `color-red-500`
   * Alias tokens (contextual): `color-error`
   * Component tokens (most specific): `button-error-background`
3. **Platform agnostic**: The same tokens can be transformed into different formats for various platforms (CSS variables, Swift constants, Android resources)
4.  **Implementation**:

    ```css
    /* CSS implementation example */
    :root {
      --color-primary: hsl(240, 100%, 50%);
      --spacing-sm: 8px;
      --font-size-heading: 24px;
    }
    ```
5. **Tooling**: Managed through specialized tools or design systems like Figma's variables, which allow you to define and use tokens through aliasing (where one variable references another).

Design tokens bridge the gap between designers and developers by creating a shared language for design decisions, enabling more consistent implementations and making system-wide changes more efficient.

{% hint style="warning" %}
Figma defaults to HEX values for color pickers **and variables**
{% endhint %}

## Figma Dev Mode

{% embed url="https://www.youtube.com/watch?v=__ABPkb0aF8" %}

## References

{% embed url="https://www.youtube.com/watch?v=JyCmacSyDY4" %}
