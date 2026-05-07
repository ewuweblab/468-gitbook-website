# Primitives

```
<!-- Rectangle with rounded corners -->
<rect x="50" y="50" width="100" height="80" 
      rx="15" ry="15" 
      fill="#ff9999" 
      stroke="#ff0000" 
      stroke-width="2"/>
<text x="60" y="90" font-size="12">Rounded Rectangle</text>

<!-- Circle -->
<circle cx="250" cy="90" r="40" 
        fill="#99ff99" 
        stroke="#009900" 
        stroke-width="2"/>
<text x="220" y="90" font-size="12">Circle</text>

<!-- Ellipse -->
<ellipse cx="420" cy="90" rx="60" ry="40" 
         fill="#9999ff" 
         stroke="#0000ff" 
         stroke-width="2"/>
<text x="400" y="90" font-size="12">Ellipse</text>

<!-- Line -->
<line x1="50" y1="200" x2="150" y2="200" 
      stroke="#000000" 
      stroke-width="4"/>
<text x="80" y="190" font-size="12">Line</text>

<!-- Polyline -->
<polyline points="200,180 220,220 240,190 260,210 280,180" 
          fill="none" 
          stroke="#800080" 
          stroke-width="2"/>
<text x="220" y="170" font-size="12">Polyline</text>

<!-- Polygon -->
<polygon points="350,180 400,180 420,220 380,240 340,220" 
         fill="#ffff99" 
         stroke="#808000" 
         stroke-width="2"/>
<text x="360" y="170" font-size="12">Polygon</text>

<!-- Path -->
<path d="M50 300 C70 250, 110 250, 130 300 S190 350, 210 300" 
      fill="none" 
      stroke="#ff00ff" 
      stroke-width="3"/>
<text x="100" y="280" font-size="12">Path (Bezier Curve)</text>

<!-- Text with different styles -->
<text x="300" y="320" 
      font-family="Arial" 
      font-size="20" 
      fill="#000080" 
      font-weight="bold">
    Styled Text
</text>

<!-- Group with transformation -->
<g transform="translate(450, 300) rotate(45)">
    <rect x="-20" y="-20" width="40" height="40" 
          fill="#ff99cc" 
          stroke="#ff0066" 
          stroke-width="2"/>
    <circle cx="0" cy="0" r="5" 
            fill="#000000"/>
</g>
<text x="420" y="350" font-size="12">Transformed Group</text>
```
