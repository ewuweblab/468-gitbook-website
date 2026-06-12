# Part 3: Astro + GSAP = Google Doodle

## Setup Codespace

* completely empty repo
* setup codespace

## Install Astro

*   Install Astro



    ```
    npm create astro@latest
    ```
* Run dev server
  * ```
    npm run dev
    ```

## Install GSAP

* `npm install gsap`
* confirm in `package.json`

## CodeSpace

* edit `src/index.astro`
* Copy HTML code into `<body>`

## CSS

* Copy CSS code into `<style>` element
* If you used course template add to `<head>` element
  * ```
    <link rel="stylesheet" href="https://codepen.io/manikoth/pen/NNNBYe.css">
    ```

## JS

* Copy JS to `<script>` element

```
// Import GSAP into project
  import gsap from "gsap";

// Optionally, install plubins
  import { GSDevTools } from "gsap/GSDevTools";
  
// Register once, before using them
gsap.registerPlugin(GSDevTools);
  
// GSAP Code
GSDevTools.create();
```

## Reference GSAP Plugins

```
// Core Plugins
import { ScrollTrigger } from "gsap/ScrollTrigger";
import { ScrollToPlugin } from "gsap/ScrollToPlugin";
import { Observer } from "gsap/Observer";
import { Flip } from "gsap/Flip";
import { Draggable } from "gsap/Draggable";
import { MotionPathPlugin } from "gsap/MotionPathPlugin";
import { TextPlugin } from "gsap/TextPlugin";

// Premium Plugins
import { SplitText } from "gsap/SplitText";
import { DrawSVGPlugin } from "gsap/DrawSVGPlugin";
import { MorphSVGPlugin } from "gsap/MorphSVGPlugin";
import { ScrambleTextPlugin } from "gsap/ScrambleTextPlugin";
import { ScrollSmoother } from "gsap/ScrollSmoother";
import { InertiaPlugin } from "gsap/InertiaPlugin";
import { CustomEase } from "gsap/CustomEase";
import { GSDevTools } from "gsap/GSDevTools";
```
