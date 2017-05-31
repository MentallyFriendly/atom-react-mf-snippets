# Mentally Friendly React.js Snippets for Atom

* An [Atom](https://atom.io/) snippet library for React. Using ES6 syntax and promoting best practices for React development.

## Install

Go to `Packages > Settings View > Install Packages/Themes` and search for **atom-react-mf-snippets**

Click Install

Restart Atom

## Features

-	React Snippets
-	React Router Snippets - (These are currently outdated and will be updated shortly)

## Table of Contents
1. [Snippets](#snippets)
1. [Development](#import)
2. [Contributing](#component-lifecycle)
3. [License](#component-api)
4. [Credit](#class-properties)

## Snippets

### Table of Snippets
1. [Import](#import)
2. [Component Lifecycle](#component-lifecycle)
3. [Component API](#component-api)
4. [Class Properties](#class-properties)
5. [PropTypes](#proptypes)
6. [ContextTypes](#contexttypes)
7. [Skeletons](#skeletons)
7. [this](#this)


### Import
**React: import empty**: `_i`
```javascript
import ${1} from '${2}'
```

**React: import**: `_ir`
```javascript
import React from 'react'
```

**React: import with Component**: `_irc`
```javascript
import React, { Component } from 'react'
```

**React: import PropTypes**: `_ip`
```javascript
import PropTypes from 'prop-types'
```

**React: import ReactDOM**: `_ird`
```javascript
import ReactDOM from 'react-dom'
```

### Component Lifecycle

#### Mounting
**React: constructor(props)**: `_cns`
```javascript
constructor(props) {
  super(props)
  this.state = {
    ${1}: props.${2}
  }
}${3}
```

**React: componentWillMount() { ... }**: `_cwm`
```javascript
componentWillMount() {
  ${1}
}${2}
```

**React: render() { return ... }**: `_ren`
```javascript
render() {
  return (
    ${1:<div></div>}
  )
}
```

**React: componentDidMount() { ... }**: `_cdm`
```javascript
componentDidMount() {
  ${1}
}${2}
```

#### Updating
**React: componentWillReceiveProps(np) { ... }**: `_cwr`
```javascript
componentWillReceiveProps(nextProps) {
  ${1}
}${2}
```

**React: shouldComponentUpdate(np, ns) { ... }**: `_scu`
```javascript
shouldComponentUpdate(nextProps, nextState) {
  ${1}
}${2}
```

**React: componentWillUpdate(np, ns) { ... }**: `_cwu`
```javascript
componentWillUpdate(nextProps, nextState) {
  ${1}
}${2}
```

**React: componentDidUpdate(pp, ps) { ... }**: `_cdup`
```javascript
componentDidUpdate(prevProps, prevState) {
  ${1}
}${2}
```

#### Unmounting
**React: componentWillUnmount() { ... }**: `_cwun`
```javascript
componentWillUnmount() {
  ${1}
}${2}
```

### Component API
**React: forceUpdate(...)**: `_fup`
```javascript
forceUpdate(${1:callback})
```

**React: setState({ ... })**: `_sst`
```javascript
this.setState({
  ${1}: ${2}
})
```

### Class Properties
**React: static defaultProps = { ... }**: `_scdp`
```javascript
static defaultProps = {
  ${1}: ${2}
}
```

**React: Class.defaultProps = { ... }**: `_cdp`
```javascript
${1}.defaultProps = {
  ${2}: ${3}
}
```

### PropTypes
**React: Class.propTypes = { ... }**: `_cpt`
```javascript
${1}.propTypes = {
  ${2}: PropTypes.${3:string}
}
```

**React: Class.propTypes = { ... } required**: `_cptr`
```javascript
${1}.propTypes = {
  ${2}: PropTypes.${3:string}.isRequired${4}
}
```

#### static propTypes
**React: static propTypes = { ... }**: `_scpt`
```javascript
static propTypes = {
  ${1}: PropTypes.${2:string}
}
```

**React: static propTypes = { ... } required**: `_scptr`
```javascript
static propTypes = {
  ${1}: PropTypes.${2:string}.isRequired${3}
}
```

#### propType blank
**React: propType blank**: `_pt`
```javascript
${1}: PropTypes.${2:string}
```

**React: propType blank Required**: `_ptr`
```javascript
${1}: PropTypes.${2:string}.isRequired${3}
```

#### propType string
**React: propTypes string**: `_pts`
```javascript
${1}: PropTypes.string${2}
```

**React: propTypes string Required**: `_ptsr`
```javascript
${1}: PropTypes.string.isRequired${2}
```

#### propType number
**React: propTypes number**: `_ptn`
```javascript
${1}: PropTypes.number${2}
```

**React: propTypes number required**: `_ptnr`
```javascript
${1}: PropTypes.number.isRequired${2}
```

#### propType object
**React: propTypes object**: `_pto`
```javascript
${1}: PropTypes.object${2}
```

**React: propTypes object required**: `_ptor`
```javascript
${1}: PropTypes.object.isRequired${2}
```

#### propType array
**React: propTypes array**: `_pta`
```javascript
${1}: PropTypes.array${2}
```

**React: propTypes array required**: `_ptar`
```javascript
${1}: PropTypes.array.isRequired${2}
```

#### propType bool
**React: propTypes bool**: `_ptb`
```javascript
${1}: PropTypes.bool${2}
```

**React: propTypes bool required**: `_ptbr`
```javascript
${1}: PropTypes.bool.isRequired${2}
```

#### propType element
**React: propTypes element**: `_pte`
```javascript
${1}: PropTypes.element${2}
```

**React: propTypes element required**: `_pter`
```javascript
${1}: PropTypes.element.isRequired${2}
```

#### propType function
**React: propTypes function**: `_ptf`
```javascript
${1}: PropTypes.func${2}
```

**React: propTypes function required**: `_ptfr`
```javascript
${1}: PropTypes.func.isRequired${2}
```

#### propType symbol
**React: propTypes symbol**: `_ptsym`
```javascript
${1}: PropTypes.symbol${2}
```

**React: propTypes symbol required**: `_ptsymr`
```javascript
${1}: PropTypes.symbol.isRequired${2}
```

#### propType node
**React: propTypes node**: `_ptnode`
```javascript
${1}: PropTypes.node${2}
```

**React: propTypes node required**: `_ptnoder`
```javascript
${1}: PropTypes.node.isRequired${2}
```

### ContextTypes
**React: Class.contextTypes = { ... }**: `_cct`
```javascript
${1}.contextTypes = {
  ${2}: PropTypes.${3:string}
}
```

**React: static contextTypes = { ... }**: `_scct`
```javascript
static contextTypes = {
  ${1}: PropTypes.${2:string}
}
```

### Skeletons
**React: Stateless Function**: `_rf`
```javascript
const ${1} = ({ ${2} }) => (
  return (
    <div>${3}</div>
  )
)
```

**React: Class**: `_rc`
```javascript
class ${1} extends Component {
  render() {
    return (
      <div>${2}</div>
    )
  }
}
```

**React: Skeleton Stateless Function**: `_srf`
```javascript
import React from 'react'

const ${1} = ({ ${2} }) => (
  return (
    <div>${3}</div>
  )
)

export default ${1}
```

**React: Skeleton Class**: `_src`
```javascript
import React from 'react'

class ${1} extends Component {
  render() {
    return (
      <div>${2}</div>
    )
  }
}

export default ${1}
```

**React: Skeleton Stateless Function w/PropTypes**: `_srfp`
```javascript
import React from 'react'
import PropTypes from 'prop-types'

const propTypes = {

}

const ${1} = ({ ${2} }) => (
  return (
    <div>${3}</div>
  )
)

${1}.propTypes = propTypes

export default ${1}
```

**React: Skeleton Class w/PropTypes**: `_srcp`
```javascript
import React from 'react'
import PropTypes from 'prop-types'

const propTypes = {

}

class ${1} extends Component {
  render() {
    return (
      <div>${2}</div>
    )
  }
}

${1}.propTypes = propTypes

export default ${1}
```

### this
**React: this.props.**: `_props`
```javascript
this.props.${1}
```

**React: this.state.**: `_state`
```javascript
this.state.${1}
```


## Development

```sh
$ cd ~/.atom/packages
$ git clone https://github.com/MentallyFriendly/atom-react-mf-snippets
$ cd atom-react-mf-snippets
$ apm install
$ apm link
```

## Contributing

1.	Fork it!
2.	Create your feature branch: `git checkout -b my-new-feature`
3.	Commit your changes: `git commit -m 'Add some feature'`
4.	Push to the branch: `git push origin my-new-feature`
5.	Submit a pull request

## License

[MIT License](http://zenorocha.mit-license.org/) © Zeno Rocha

## Credit

The React.js snippets were originally created by [orktes](https://atom.io/users/orktes) in [Atom React](https://atom.io/packages/react) in ES5 syntax.
