# Composition

```
<!-- Sun with rays -->
<g transform="translate(300, 80)">
    <!-- Main sun circle -->
    <circle r="25" fill="#FFD700" />
    
    <!-- Sun rays using lines -->
    <g stroke="#FFD700" stroke-width="3">
        <line x1="0" y1="-40" x2="0" y2="-30" />
        <line x1="28" y1="-28" x2="21" y2="-21" />
        <line x1="40" y1="0" x2="30" y2="0" />
        <line x1="28" y1="28" x2="21" y2="21" />
        <line x1="-28" y1="-28" x2="-21" y2="-21" />
        <line x1="-40" y1="0" x2="-30" y2="0" />
        <line x1="-28" y1="28" x2="-21" y2="21" />
    </g>
</g>

<!-- Clouds using multiple ellipses -->
<g transform="translate(100, 100)">
    <ellipse cx="0" cy="0" rx="30" ry="20" fill="white" />
    <ellipse cx="-20" cy="5" rx="25" ry="15" fill="white" />
    <ellipse cx="20" cy="5" rx="25" ry="15" fill="white" />
</g>

<g transform="translate(250, 150)">
    <ellipse cx="0" cy="0" rx="35" ry="25" fill="white" opacity="0.8" />
    <ellipse cx="-25" cy="5" rx="30" ry="20" fill="white" opacity="0.8" />
    <ellipse cx="25" cy="5" rx="30" ry="20" fill="white" opacity="0.8" />
</g>

<!-- Mountains using polygons -->
<polygon points="0,300 150,100 300,300" fill="#4B6455" />
<polygon points="100,300 250,150 400,300" fill="#3A4F42" />

<!-- Trees using combinations of shapes -->
<g transform="translate(50, 250)">
    <rect x="-5" y="-20" width="10" height="20" fill="#5D432C" />
    <polygon points="-15,-20 15,-20 0,-50" fill="#2D5A27" />
    <polygon points="-12,-15 12,-15 0,-40" fill="#3A7230" />
</g>

<g transform="translate(90, 260)">
    <rect x="-4" y="-15" width="8" height="15" fill="#5D432C" />
    <polygon points="-12,-15 12,-15 0,-40" fill="#2D5A27" />
    <polygon points="-10,-12 10,-12 0,-32" fill="#3A7230" />
</g>

<!-- Lake using path with curve -->
<path d="M0,280 Q200,260 400,280 L400,300 L0,300 Z" fill="#5B9BD5" opacity="0.8" />

<!-- Rain drops using small lines -->
<g stroke="#4A90E2" stroke-width="2">
    <line x1="100" y1="140" x2="95" y2="155" />
    <line x1="120" y1="150" x2="115" y2="165" />
    <line x1="140" y1="145" x2="135" y2="160" />
    <line x1="90" y1="160" x2="85" y2="175" />
    <line x1="110" y1="170" x2="105" y2="185" />
</g>
```
