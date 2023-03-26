# @letea/prettier-config

[![npm version](https://badge.fury.io/js/%40letea%2Fprettier-config.svg)](https://badge.fury.io/js/%40letea%2Fprettier-config)

My [Prettier](https://prettier.io) config.

## Usage

**Install**:

```bash
$ yarn add --dev @letea/prettier-config
```

**Edit `package.json`**:

```jsonc
{
  // ...
  "prettier": "@letea/prettier-config"
}
```

## Style

### arrowParens: "always"
Keep the same style to all functions.
``` javascript
// always
() => { ... };
(x) => { ... };
(x, y) => { ... };

// avoid
() => { ... };
x => { ... };
(x, y) => { ... };
```

### bracketSpacing: true
Add a space for the best reading to developers.
``` javascript
// true
{ foo: bar }

//false
{foo: bar}
```

### jsxBracketSameLine: false
Keep the same position of the bracket for the best reading to developers.
``` jsx
// false
<button
  className="prettier-class"
  id="prettier-id"
  onClick={this.handleClick}
>
  Click Here
</button>

// true
<button
  className="prettier-class"
  id="prettier-id"
  onClick={this.handleClick}>
  Click Here
</button>
```

### semi: true
Make sure where is the end of the line to developers.
``` javascript
// true
console.log("1");
console.log("2");
console.log("3");

// false
console.log("1")
console.log("2")
console.log("3")
```

### singleQuote: false
Keep the same format with [JSON](https://zh.wikipedia.org/wiki/JSON).
``` javascript
// false
let item = "This is double quote";

// true
let item = 'This is single quote';
```

### tabWidth: 2
The best space for reading.
``` javascript
// 2
if (true) {
  console.log("This tabWidth is 2.");
}


// 4
if (true) {
    console.log("This tabWidth is 4.");
}
```

## Reference

* [Prettier](https://prettier.io)
* [@azz/prettier-config](https://github.com/azz/prettier-config)
* [JSON - Wikipedia](https://zh.wikipedia.org/wiki/JSON)
