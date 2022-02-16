# Simple React Snippets for Typescript

- Simple React Snippets Extension by burkeholland customized to my own daily uses. (removed classes, add hooks, console log, named functions...)
- Install https://marketplace.visualstudio.com/items?itemName=fulin.react-snippets-typescript

The essential collection of React Snippets and commands.

![snippets in action](images/snippets-in-action.gif)

## Features

Only what you need and nothing more. **No Redux. No React Native.**

Simply, simple React snippets.

These snippets were selected carefully from my own day-to-day React use. Not
everything in React is included here. This is a hand selected set of snippets
that work the way that you would expect, not just a copy of the documentation.

## Snippets

| Snippet | Renders                                       |
| ------- | --------------------------------------------- |
| `imr`   | Import React                                  |
| `imem`  | Import External Module                        |
| `imrd`  | Import ReactDOM                               |
| `ims`   | Import useState                               |
| `imse`  | Import useState useEffect                     |
| `impt`  | Import PropTypes                              |
| `use`   | useEffect Hook                                |
| `uss`   | Declare a new state variable using State Hook |
| `usx`   | Declare a new state variable using X Hook     |
| `clg`   | Console Log                                   |
| `clo`   | Console Log Object                            |
| `nfn`   | Named function                                |
| `anfn`  | Async Named function                          |
| `fc`    | Function Component                            |
| `ffc`   | Function Syntax Component                     |
| `gds`   | getDerivedStateFromProps                      |
| `gsbu`  | getSnapshotBeforeUpdate                       |
| `ren`   | render                                        |
| `rprop` | Render Prop                                   |
| `hoc`   | Higher Order Component                        |
| `cp`    | Context Provider                              |
| `cpf`   | Class Property Function                       |

- Full expansions is not completed. Check `snippets/snippets-ts.json` for all the updated snippets.

## Full Expansions

### imr - Import React

```javascript
import * as React from "react";
```

### imrc - Import React, Component

```javascript
import * as React from "react";
import { Component } from "react";
```

### imrd - Import ReactDOM

```javascript
import ReactDOM from "react-dom";
```

### ims - Import useState

```javascript
import { useState } from "react";
```

### imse - Import useState, useEffect

```javascript
import { useState, useEffect } from "react";
```

### impt - Import PropTypes

```javascript
import PropTypes from "prop-types";
```

### ffc - Function Component

```javascript
function (|) {
    return ( | );
}

export default |;
```

### sfc - Stateless Function Component (Arrow function)

```javascript
const | = props => {
  return ( | );
};

export default |;
```

### use - useEffect Hook

```javascript
useEffect(() => {
  |
}, []);
```

### gds - getDerivedStateFromProps

```javascript
static getDerivedStateFromProps(nextProps, prevState) {
  |
}
```

### gsbu - getSnapshotBeforeUpdate

```javascript
getSnapshotBeforeUpdate(prevProps, prevState) {
  |
}
```

### uss - Declare a new state variable using State Hook

```javascript
const [|, set|] = useState();
```

_Hit Tab to apply CamelCase to function. e.g. [count, setCount]_

### ren - render

```javascript
render() {
  return (
    |
  );
}
```

### rprop - Render Prop

```javascript
class | extends Component {
  state = { | },
  render() {
    return this.props.render({
      |: this.state.|
    });
  }
}

export default |;
```

### hoc - Higher Order Component

```javascript
function | (|) {
  return class extends Component {
    constructor(props) {
      super(props);
    }

    render() {
      return < | {...this.props} />;
    }
  };
}
```

### cpf - Class Property Function

```javascript
  | = (e) => {
    |
  }
```

## Commands

### React: class to className

Changes all occurences of `class` in JSX to `className`. This transform is safe
to run multiple times on any document. No text needs to be selected as the
command is executed on the entire document.

![React: class to className](https://i.imgur.com/i1ZwvOu.gif)

## Thank You! ❤️

While I wrote the initial version of this extension, many people (too many to name) have helped make it what it is today. From providing TypeScript definitions to keeping up with changing API and best practices. If you are enjoying this extension, you have the great React community to thank.
