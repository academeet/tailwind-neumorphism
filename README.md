# tailwindcss-neumorphism

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> Generate soft UI CSS code using tailwindcss

## 🤔Why?

This plugin is inspired by [neumorphism.io](https://neumorphism.io/), as well as [this article](https://uxdesign.cc/neumorphism-in-user-interfaces-b47cef3bf3a6) by Michal Malewicz which I highly recommend you check out.

![An example of Neumorphism](https://cdn.dribbble.com/users/2202649/screenshots/9527558/media/13076f9099e978de5f04c1bec809464f.png 'Freebie Neumorphic UX UI Elements by Emy Lascan on Dribbble')

## Getting Started

Install via npm or yarn

```
npm install tailwindcss-neumorphism
```

```
yarn add tailwindcss-neumorphism
```

Then just require it as a plugin.

```js
// tailwind.config.js
module.exports = {
  plugins: [
    require('tailwindcss-neumorphism')
  ]
}
```

### Colors

By default, neumorphism classes will be generated for all of your colors. Alternatively, you can set these colors explicitly in the config.

```js
module.exports = {
  // ...
  theme: {
    neumorphism: {
      red: {
        100: '#FBEBE9',
        200: '#F5CEC7',
        // ...
      }
    }
  }
  // ...
}
```

### Variants

The default variants for neumorphism utilities are `responsive`, `hover` and `focus`. These can configured [like any other tailwind utility](https://tailwindcss.com/docs/configuring-variants/).

```js
module.exports = {
  // ...
  variants: {
    neumorphism: ['responsive']
  }
  // ...
}
```