# Mentally Friendly React.js Snippets for Atom

* An [Atom](https://atom.io/) snippet library for React. Using ES6 syntax and promoting best practices for React development.

## Install

Go to `Packages > Settings View > Install Packages/Themes` and search for **atom-react-mf-snippets**

Click Install

Restart Atom

## Features

-	React Snippets
-	React Router Snippets - (These are currently outdated and will be updated shortly)

## Table of Snippets
1. [Import](#import)

## Import Snippets
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

# Development

```sh
$ cd ~/.atom/packages
$ git clone https://github.com/MentallyFriendly/atom-react-mf-snippets
$ cd atom-react-mf-snippets
$ apm install
$ apm link
```

# Contributing

1.	Fork it!
2.	Create your feature branch: `git checkout -b my-new-feature`
3.	Commit your changes: `git commit -m 'Add some feature'`
4.	Push to the branch: `git push origin my-new-feature`
5.	Submit a pull request

# License

[MIT License](http://zenorocha.mit-license.org/) © Zeno Rocha

# Credit

The React.js snippets were originally created by [orktes](https://atom.io/users/orktes) in [Atom React](https://atom.io/packages/react) in ES5 syntax.
