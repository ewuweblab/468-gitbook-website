# Print Style Sheets

### Example Repo

{% embed url="https://github.com/mikepqr/resume.md" %}

### Previewing

This is a cumbersome process. May require lots of refreshing without cache. View results with:&#x20;

* Save as PDF
* Dev Tools Print emulator

### Print Media Query

Nest CSS rules in inside of media query.&#x20;

```css
@media print {...}
```

### Hiding Content

```
... {
display: none
}
```

### Showing URLs

```

a[href]::after {
    // empty space then print url
    content: " " attr(href); 
}
```

### Columns

```css
// text columns
... {
columns: 2
}
```

### Hyphenation

```
...{
-moz-hyphens: auto;
-webkit-hyphens: auto;
hyphens: auto;
}
```

### Widows and Orphans

```
... {
widows: 0;
orphans: 0;
}
```

### @page

```
// Set printing margins
@page {
    margin: 0;
}
```

### References

{% embed url="https://www.linkedin.com/learning/css-print-style-sheets" %}

