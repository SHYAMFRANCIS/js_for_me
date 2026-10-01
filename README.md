# js_for_me

![JavaScript](https://img.shields.io/badge/language-JavaScript-yellow)
![HTML](https://img.shields.io/badge/markup-HTML5-orange)
![License](https://img.shields.io/badge/license-MIT-green)

Personal JavaScript learning exercises — one small script per language concept (variables, strings, arrays, objects, constants), plus a minimal `index.html` playground page.

## Features

- `index.js` — variable declarations and naming-rule notes, logged to the console.
- `strings.js` — string/number/boolean basics (`name`, `age`, `isOK`).
- `array.js` — array indexing, `length`, `push`, `pop`, and `typeof` checks.
- `object.js` — object literals with dot-notation and bracket-notation mutation.
- `constants.js` — `const` declaration (`interestRate = 0.3`).
- `function.js` — reserved placeholder for function exercises (currently empty).
- `index.html` — simple "Hello World" page used as a browser playground.

## Tech Stack

- Vanilla JavaScript (Node.js for the `.js` files, browser for `index.html`)
- No dependencies, no build step, no `package.json`

## Structure

```text
js_for_me/
├── index.js       # variables + naming rules
├── strings.js     # primitives
├── array.js       # arrays: index, length, push/pop
├── object.js      # objects: dot vs bracket notation
├── constants.js   # const keyword
├── function.js    # (empty placeholder)
└── index.html     # hello-world playground page
```

## Installation

None — clone and run. You only need [Node.js](https://nodejs.org/) for the `.js` files and any browser for `index.html`.

```bash
git clone https://github.com/SHYAMFRANCIS/js_for_me.git
cd js_for_me
```

## Usage

Run any exercise directly with Node:

```bash
node index.js
node strings.js
node array.js
node object.js
node constants.js
```

Expected output samples (verified from source):

```text
# node array.js
pink black
7
8
7
[ 'red', 'black', 'pink', 'blue', 'shyam', 2, 'francis' ]
object

# node object.js
{
  name: 'Betadine',
  age: 30,
  isCollage: true,
  isParents: true,
  isArrear: false,
  location_native: 'karaikal'
}
```

To view `index.html`, open it directly in a browser (double-click the file). Note: its inline `<script>` block currently contains `src = "index.js"` as script *body* rather than a `src` attribute, so it does not load `index.js` — open devtools console to experiment instead.

## Examples

Dot vs bracket notation (`object.js`):

```js
let person = { name: "john", age: 27, isCollage: true };

// dot notation
person.age = 30;
person.name = "Betadine";

// bracket notation
person["isCollage"] = false;
person["isArrear"] = false;
```

## Configuration

No configuration — each file is standalone with hardcoded values.

## Contributing

1. Fork, branch, and add one file per concept (e.g. `loops.js`, `classes.js`).
2. Keep `console.log` output so each file is self-demonstrating.
3. Open a pull request.

## License

MIT — no license file is currently present; MIT applies by default for reuse of these sample exercises.
