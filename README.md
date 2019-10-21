<h1 align="center">Original-UI</h1>

<div align="center">

A totally **original** component library built for [React.js](http://reactjs.org/).

[![NPM](https://img.shields.io/npm/v/original-ui.svg)](https://www.npmjs.com/package/original-ui)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
[![Build Status](https://travis-ci.org/JakeAdmire/original-ui.svg?branch=master)](https://travis-ci.org/JakeAdmire/original-ui)
[![Coverage Status](https://coveralls.io/repos/github/JakeAdmire/original-ui/badge.svg?branch=ci-testing-deployment-setup)](https://coveralls.io/github/JakeAdmire/original-ui?branch=ci-testing-deployment-setup)
</div>

## Why?
Why did I build **Original-UI?** Several reasons really: 
- I thought it'd be fun (and it is!)
- I wanted to stay sharp with React & JavaScript while searching for a Front End Engineering role ([hire me!](https://www.linkedin.com/in/jakeadmire/))
- I thoroughly enjoy UI & UX design and this seemed like a great opportunity to practice it

## Directory

- [Install](#install)
- [Components](#components)
	- [TextInput](#textinput)
	- [Icon](#icon)
- [Credits & Dependencies](#credits-&-dependencies)
- [License](#license)

## Install

```bash
npm install --save original-ui
```

## Components

### TextInput

#### Example Usage:

```javascript
import { TextInput } from  'original-ui'

<TextInput 
  placeholderText='ex. "thoughtfulpassword123..."'
  labelText='Enter your password:' 
  isPassInput={this.state.isTextHidden}
  rightIcon={
    <Icon 
      iconName={this.state.isTextHidden ? 'eye' : 'eye-slash'}
      iconSize='24px'
      onPress={this.toggleHiddenText}/>
  }/>
```

**Result:**

<img width="838" alt="Screen Shot 2019-10-20 at 9 14 45 PM" src="https://user-images.githubusercontent.com/44077214/67174278-b931fa80-f37e-11e9-8e9c-fe374a3642cb.png">


#### Parameters:

|Parameter| Data Type | Default Value | Description |
|--|--|--|--|
| `placeholderText` | `String` | `null` | _Pass a string to display as a placeholder_ |
| labelText | `String` | `null` | _Pass a string to display as a label_ |
| labelStyle | `Object` | `{ color: 'orange' }` | _Pass a style object to set the label's style rules_ |
| isPassInput | `Boolean` | `false` | _Pass a boolean to determine whether you want the input's text obscured_ |
| leftIcon | `Component` | `null` | _Pass an [Icon](#icon) component to display on the left side of the input_ |
| rightIcon | `Component` | `null` | _Pass an [Icon](#icon) component to display on the right side of the input_ |
| `width` | `String` | `'100%'` | _Pass a string to constrict the component's width_ |
| `height` | `String` | `'50px'` | _Pass a string to constrict the component's height_ |
| `textStyle` | `Object` | `{ fontSize: '16px', color: 'grey' }` | _Pass a style object to set the input text's style rules_ |
| `onChange` | `Function` | `null` | _Pass a method that will receive the `event` object as a parameter_ |
| `value` | 'String' | `null` | _Pass a string to set the input's value_ |
---

### Icon

**Original-UI** utilizes [Font Awesome](fontawesome.com) to build it's icons. To take advantage of this component you must first follow the instructions at [fontawesome.com](fontawesome.com) and implement the `<script>` tag within the enclosing `<head>` tags of your `index.html` file.

#### Example Usage:

```javascript
import { Icon } from  'original-ui'

<Icon
  iconName='skull'
  iconColor='white'
  backgroundColor='red'/>
<Icon
  iconName='bath'
  iconColor='white'
  backgroundColor='cornflowerblue' />
<Icon
  iconName='bomb'
  iconColor='white'
  backgroundColor='black' />
```

**Result:**

<img width="205" alt="Screen Shot 2019-10-20 at 5 47 46 PM" src="https://user-images.githubusercontent.com/44077214/67168473-22574500-f362-11e9-8c02-961901f03072.png">

#### Parameters:

|Parameter| Data Type | Default Value | Description |
|--|--|--|--|
| `iconName` | `String` | `null` | Pass a string with the name of a Font Awesome icon to build the icon |
| `iconType` | `String` | `'Solid'` | _Pass a string of 'Solid', 'Regular', 'Light', 'Duotone', or 'Brands' to determine the icon style. Only 'Solid' & 'Brands' are included by Font Awesome for free_ |
| `iconSize` | `String` | `'24px'` | _Pass a string to constrict the icon's size_ |
| `iconColor` | `String` | `'#00000033'` | _Pass a string to set the icon's color_ |
| `rotation` | `String` | `null` | _Pass a string of '90', '180', or '270' to rotate the icon to that degree_ |
| `isFlippedVertically` | `Boolean` | `false` | _Pass a boolean to determine whether the icon is flipped vertically_ |
| `isFlippedHorizontally` | `Boolean` | `false` | _Pass a boolean to determine whether the icon is flipped horizontally_ |
| `isSpinning` | `Boolean` | `false` | _Pass a boolean to determine whether the icon spins continuously_ |
| `isPulsing` | `Boolean` | `false` | _Pass a boolean to determine whether the icon pulses continuously_ |
| `onPress` | `Function` | `null` | _Pass a function to be called on icon press. Icon will not behave as a button if `onPress` is null_ |
| backgroundColor | `String` | `null` | _Pass a string to set the icon's background color_ |

## Credits & Dependencies

[create-react-library](https://www.npmjs.com/package/create-react-library) *- React library bootstrap CLI*

[React.js](https://reactjs.org/) *- JavaScript UI library*

[Jest](https://jestjs.io/) *- JavaScript testing framework*

[TravisCI](https://travis-ci.org/) *- Continuous integration*

[Coveralls.io](https://coveralls.io/) *- Code coverage testing*

## License

MIT © [JakeAdmire](https://github.com/JakeAdmire)
