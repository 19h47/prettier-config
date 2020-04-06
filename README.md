# prettier-config

19h47's [`prettier`](https://prettier.io) configuration.

## Installation

### yarn

```sh
yarn install 19h47/prettier-config
```

If you don't have it installed already, also install `prettier` as a devDependency.

```sh
yarn install --dev prettier
```

## Usage

We export Prettier configurations for your usage.

### Default Config

Create a `prettier.config.js` file at the root of your project that contains:

```js
module.exports = require('@19h47/prettier-config');
```

## [Editor Integration](https://prettier.io/docs/en/editors.html)

### Visual Studio Code

1. Install Prettier extension: `View → Extensions` then find and install Prettier - Code formatter
2. Reload the editor
3. In your user settings `Code -> Preferences -> Settings` add `editor.formatOnSave: true`

## Enforced Rules

Check out all of Prettier's [configuration options](https://prettier.io/docs/en/options.html).

- **Print Width**

  Line wrap at 100 characters.

- **Tab Width**

  2 spaces per indentation-level.

- **Tabs**

  Indent lines with spaces, not tabs.

- **Semicolons**

  Always print semicolons at the ends of statements.

  ```js
  const greeting = 'hi';
  ```

- **Quote**

  Use single quotes instead of double quotes.

  ```js
  const quote = 'single quotes are better';
  ```

- **Trailing Commas**

  Use trailing commas wherever possible.

  ```js
  const obj = {
    a: 'hi',
    b: 'hey',
  };
  ```

- **Bracket Spacing**

  Print spaces between brackets in object literals.

  ```js
  {
    foo: bar;
  }
  ```

- **JSX Brackets**

  Put the `>` of a multi-line JSX element at the end of the last line instead of being alone on the next line (does not apply to self closing elements).

  ```jsx
  <button className="prettier-class" id="prettier-id" onClick={this.handleClick}>
    Click Here
  </button>
  ```

- **Arrow Function Parentheses**

  Omit parens when possible.

  ```js
  x => x;
  ```
