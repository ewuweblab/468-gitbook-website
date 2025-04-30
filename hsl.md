# HSL

HSL (Hue, Saturation, Lightness) color notation offers several advantages over hexadecimal notation in CSS. Here are the key benefits:

1. Intuitive understanding: HSL represents colors in a way that's more aligned with how humans perceive color - through hue (the color itself), saturation (intensity), and lightness (brightness).
2. Easier adjustments: With HSL, you can easily adjust properties independently:
   * Change only the lightness to create lighter/darker versions
   * Modify saturation to make colors more/less vibrant
   * Shift the hue while maintaining the same saturation and lightness
3. Simpler relationships: Creating color schemes is more straightforward - complementary colors are 180° apart on the hue scale, and analogous colors are close to each other.
4. Better for dynamic colors: When using JavaScript to manipulate colors, HSL makes calculations much more intuitive.

```
/* With hex, not intuitive: */
.dark-blue { color: #00008B; }

/* With HSL, simply reduce lightness: */
.blue { color: hsl(240, 100%, 50%); }
.dark-blue { color: hsl(240, 100%, 27%); }
```

## # HSL and Design Tokens

{% embed url="https://codepen.io/manikoth/pen/VYYrRba" %}



## # FYI

* Future is `color()` for a broader P3 display support\`
* `oklch()` color function will be used with `color()`&#x20;

## References

{% embed url="https://www.joshwcomeau.com/css/color-formats/" %}
