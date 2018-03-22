# @itrulia/nova-skeletons
> CSS Utility library to create beautiful skeleton screens

This CSS utility library allows you to create beautiful skeleton screens without much hassle. It has been built for simplicity and maintainability.


## Demos

* [Card with image and text](https://codepen.io/Itrulia/pen/dmWxzw)

## Installing / Getting started

To install it you need to require it like this:

```shell
npm install --save @itrulia/nova-skeletons
```

This will add the @itrulia/nova-skeletons dependency in to your package.json.

## How to use

You should attach the base class `c-skeleton` to the root of your skeleton screen HTML. While this class has no styles attached to it, you can use it if you need to increase the specifity of your CSS if needed. + It also helps to keep the HTML a little bit more grouped.

### Text

The simplest skeleton you can create is one of text that is loading. For this we can use the `c-skeleton__text` class.

```html
<div class="c-skeleton">
    <div class="c-skeleton__text"></div>
</div>
```

#### Modifiers

```css
/* Removes the margin on top/bottom of the text */
.c-skeleton__text--small-height {...}

/* Makes the display style inline block */
.c-skeleton__text--inline {...}

/* Makes the text width full width */
.c-skeleton__text--full {...}

/* Makes the text width big */
.c-skeleton__text--big {...}

/* Makes the text width bigger */
.c-skeleton__text--bigger {...}

/* Makes the text width small */
.c-skeleton__text--small {...}

/* Makes the text width smaller */
.c-skeleton__text--smaller {...}

/* Makes the text width very tiny */
.c-skeleton__text--tiny {...}
```

### Image / Video / etc.

If you want to skeleton an image/video, you can use the class `c-skeleton__figure`. This class adjusts to the parents width and height.

```html
<div class="c-skeleton" style="width: 50px; height: 50px;">
    <div class="c-skeleton__figure"></div>
</div>
```

**Pro tip**: If the non loading state has a border radius, you simply can add a class to it that adds the border radius to the skeleton aswell. In most cases, the skeleton can have the same classes attached as the loaded state!

## Developing

Here's a brief intro about what a developer must do in order to start developing
the project further:

```shell
git clone https://github.com/Itrulia/nova-skeletons
cd nova-skeletons/
npm install
```

This will download all dependencies so that you are ready to go.

### Deploying / Publishing

You will need to publish this to the github and npm repository.

To do this you will need to do the following steps:

* As soon as you are done with development (don't forget the tests if necessary please ;) ) please commit your code
* After that you will need to update the version number of the package.json, please do this via the [npm version](https://docs.npmjs.com/cli/version) tool. Don't forget to set the correct version number according to the [SEMVER](http://semver.org/) guidelines.
* Please push your code to master now and set a tag (same version as you set earlier) with a `v` prefix (e.g. `v1.1.0`) and add release notes for what has changed so everyone knows what to do when there are breaking changes and what has changed for them.
* Now you are ready to publish it to the npm repository. You can do this via `npm publish`. Further information can be founde on the official [npm documentation page](https://docs.npmjs.com/cli/publish).

## Features

* Works with **every** frontend framework you are using!
* Supports texts, images, videos and much more.
* Font size agnostic
* Multiple modifiers for your likings
* Override colors via SCSS
* Written with BEM
* Low specificity
* No dependencies

## SCSS Configuration

### nova-color-skeleton-background
Type: `color`
Default: `#eee`

### nova-color-skeleton-spinner
Type: `color`
Default: `#e7e7e9`

## Contributing

When you publish something open source, one of the greatest motivations is that
anyone can just jump in and start contributing to your project.

To make it easier for everyone to contribute to this project and understand it,
please always update the documentation when you create or modify anything.

Also always try to improve atleast 1 small thing when you are already there so that over time
the project gets better and better, this is also known as [The Boy Scout Rule](http://programmer.97things.oreilly.com/wiki/index.php/The_Boy_Scout_Rule).

## Links

- Repository: https://github.com/Itrulia/nova-skeletons
- Issue tracker: https://github.com/Itrulia/nova-skeletons/issues
  - In case of sensitive bugs like security vulnerabilities, please contact
    karlmerkli@gmail.com directly instead of using issue tracker. We value your effort
    to improve the security and privacy of this project!
- Related posts:
  - https://www.viget.com/articles/a-bone-to-pick-with-skeleton-screens/


## Licensing

Copyright (c) 2018 Karl Merkli

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.