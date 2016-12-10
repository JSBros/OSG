# OCD Style Guide v1
The OSG is an attempt to make a universal style-guide for code that aims to be language-agnostic. The use of alphabetization is extremely prevalent in the OSG.

## Official OSG Shield

The easiest way to show off that your repository enforces the OSG is by including the official shield in your `README.md` file.

[![OSGv1](https://img.shields.io/badge/Code%20Style-OSGv1-19AFE4.svg)](https://github.com/JSBros/OSG#readme)

```markdown
[![OSGv1](https://img.shields.io/badge/Code%20Style-OSGv1-19AFE4.svg)](https://github.com/JSBros/OSG#readme)
```

## Purpose
There's certain times we must make styling decisions between the linter rules. Style rules related to organizing your code, as opposed to formatting. Most of the time these decisions fall on the shoulders of developers, and hardly ever are consistent styles kept. Mostly due to a lack of general guidelines to follow, just the discretion of the programmer.

The OCD Style Guide aims to remove these responsibilities from the developer and enforce a more pleasing code organization style.

## Import Statements
* [x] All import levels must be grouped according to their kind, separated by a blank line.
* [x] All module-level imports must come first.
* [x] All project-level imports must come next.
* [x] There must be exactly `1` blank line between the import groups (not counting docs).
* [x] All imports must be alphabetized in their own group.
* [x] PascalCase imports must come before camelCase imports.
* [x] Letters come before symbols (i.e. `import React...` comes before `import { Link }...`


Example of import statements:
```jsx
import React, { PropTypes } from 'react';
import emojione from 'emojione';
import styled from 'styled-components';
import toastr from 'toastr';
import { bindActionCreators } from 'redux';
import { connect } from 'react-redux';
import { emojify } from 'react-emojione';
import { Link, IndexLink } from 'react-router';
import { Row, Column } from 'hedron';

import AdminLink from './AdminLink';
import Button from '../Button';
import LoginLink from './LoginLink';
import Logo from './Logo';
import LogoutLink from './LogoutLink';
import Nav from '../Nav';
```
