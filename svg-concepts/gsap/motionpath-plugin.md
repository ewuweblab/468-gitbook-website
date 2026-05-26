# MotionPath Plugin

## Basic Motion Path

{% embed url="https://codepen.io/manikoth/pen/EaNwRPg" %}

* The `<path>` needs `fill="none"` — without it SVG fills the path shape solid black.
* The `<text>` starts at `x="0" y="0"` — GSAP ignores those and moves the element with a CSS `transform` instead.
* `id` attributes on both elements are what `path: "#track"` and `gsap.to("#star", …)` target.
* `align: "#track"` tells GSAP to reconcile coordinate systems between the `<text>` and the `<path>` — essential if they're in different transformed containers, or if the SVG is scaled via `width="100%"`.
* `alignOrigin: [0.5, 0.5]` is CSS "transform-origin: 50% 50%"



## Motion Path Helper

{% embed url="https://codepen.io/manikoth/pen/emBGKEz" %}

* two elements: a `<path id="track">` (the curved guide, drawn as a dashed line) and a `<text id="star">` (the moving target, initially at `0,0`).
* `gsap.to("#star", { motionPath: … })` moves the star along the track over 5 seconds. The commented-out `repeat: -1` / `yoyo: true` would loop it back and forth. `autoRotate: true` tilts the star to face the direction of travel.

