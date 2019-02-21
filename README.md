## react-radio-toggle

[![npm version](https://badge.fury.io/js/react-radio-toggle.svg)](https://badge.fury.io/js/react-radio-toggle)

A simple radio button toggle component

## Install

``` js
yarn add react-radio-toggle
```

## Use

``` js
import Toggle from 'react-radio-toggle'
import ReactDOM from 'react-dom'
import React, { Component } from 'react'

class TestComponent extends Component {
  toggled(value) {
    console.log(value)
  }

  render() {
    let items = ['apple', 'orange', 'lemon', 'peach']
    return (
      <div>
        <Toggle
          items={items}
          checked="apple"
          name="toggleFruits"
          onToggle={this.toggled.bind(this)}
        />
      </div>
    )
  }
}

ReactDOM.render(<TestComponent />, document.getElementById('root'))
```

## Styles

Uses styled-components 💅 for the base styling.

## Development
    yarn
    npm run dev

## Build
    yarn
    npm run build
    npm login
    npm version patch
    git add -A
    git push origin master
    npm publish

## License

[MIT](http://isekivacenz.mit-license.org/)
