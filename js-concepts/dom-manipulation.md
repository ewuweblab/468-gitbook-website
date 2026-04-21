# DOM Manipulation

Think of the DOM as a **living document** that JavaScript can reach into and rearrange like Lego blocks. You're not editing the HTML file—you're controlling what the user sees _right now_ in their browser.

### Getting Elements

**getElementById** is like calling someone by their unique name:

```javascript
const header = document.getElementById('main-header')
```

Only one element can have that ID, so you get exactly that person.

**querySelector** is like describing someone: "the first person wearing a red hat"

```javascript
const firstButton = document.querySelector('.btn')
```

CSS selectors work here—`.class`, `#id`, `div > p`, whatever you'd use in CSS.

**querySelectorAll** gets everyone matching the description:

```javascript
const allButtons = document.querySelectorAll('.btn')
```

You get a list back, like an array of all the people wearing red hats.

### Getting Values: Reading the State

Once you have an element, you can **inspect** it:

* `textContent` — the actual words, stripped of formatting (like reading a book with no bold/italics)
* `innerHTML` — the formatted text with HTML tags included (the full manuscript)
* `value` — what's typed in a form field (what the user wrote on the form)

```javascript
const username = document.querySelector('#username-input').value
// If the user typed "Alice", username is now "Alice"
```

Think of it like checking someone's nametag, reading their t-shirt, or peeking at their clipboard.

### Setting Values: Changing Reality

Here's where the magic happens. You **rewrite** what's on screen:

```javascript
element.textContent = 'Updated text'
```

The page _immediately_ changes. No refresh needed. It's like erasing a whiteboard and writing something new.

**innerHTML** lets you add HTML:

```javascript
element.innerHTML = '<strong>Bold</strong> text'
```

This replaces the contents with formatted text. Use carefully—it can wipe out event listeners.

**Styles** change appearance:

```javascript
element.style.backgroundColor = 'yellow'
element.style.display = 'none'  // hide it
```

CSS properties use camelCase (`background-color` → `backgroundColor`).

**Classes** are better for styling (because CSS belongs in CSS files):

```javascript
element.classList.add('hidden')      // add a class
element.classList.remove('active')   // remove one
element.classList.toggle('dark-mode') // flip it on/off
```

### Real Example: A Counter Button

```javascript
// Get the elements
const button = document.querySelector('#counter-btn')
const display = document.querySelector('#count-display')

let count = 0

// When clicked, update the display
button.addEventListener('click', () => {
  count++
  display.textContent = count  // SET the new number
})
```

Every click **gets** the current count, increments it, and **sets** the display. The page updates instantly.

### Creating New Elements: Building Legos

```javascript
const newDiv = document.createElement('div')
newDiv.textContent = 'I am new'
newDiv.classList.add('box')

document.body.appendChild(newDiv)  // Add it to the page
```

You built a div in JavaScript, dressed it up, and placed it on the page. It didn't exist in the HTML file—JavaScript _materialized_ it.

***

**The Core Pattern:**

1. **Get** an element (find the Lego)
2. **Get or Set** a property (read or change it)
3. The browser updates instantly

That's DOM manipulation. You're the puppeteer, and the webpage dances.
