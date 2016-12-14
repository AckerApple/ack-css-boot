# ack-css-boot
A base set of short-hand css helper classes. Includes available classes that are commonly used for styling buttons, form inputs, and such.

Many commonly used short-hand classes, that are found in [Ionic](https://www.npmjs.com/package/ionic) and [Bootstrap](https://www.npmjs.com/package/bootstrap-css), can be found here.

### Table of Contents
- [Usage and Examples](#usage-and-examples)
- [Primary Style File](#primary-style-file)
- [Resources](#resources)

## Usage and Examples
Learn about css short-hand classes such as .pad, .margin, .text-lg, and more...

[tap here to see demos](https://ackerapple.github.io/ack-css-boot/)

All examples seen below, are written in [Sass](http://sass-lang.com/) and then compiled to css in the /dist folder.

> NOTE: ack-css-boot makes every attempt to avoid using the !important declaration. It is highly advised that the ack-css-boot.css file, be the LAST stylesheet file loaded in order to have short-hand css rules override other stylesheet rules.


## Primary Style File

[scss/ack-css-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-css-boot.scss)

```
@import "./ack-text-boot";
@import "./ack-flex-boot";
@import "./ack-color-boot";
@import "./ack-block-boot";
@import "./ack-position-boot";
@import "./ack-form-boot";
@import "./ack-responsive-boot";
```

## Resources
Quick links to examples and source code

- [ack-text-boot](https://ackerapple.github.io/ack-css-boot/#ack-text-boot)
  - [scss/ack-text-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-text-boot.scss)
- [ack-flex-boot](https://ackerapple.github.io/ack-css-boot/#ack-flex-boot)
  - [scss/ack-flex-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-flex-boot.scss)
- [ack-color-boot](https://ackerapple.github.io/ack-css-boot/#ack-color-boot)
  - [scss/ack-color-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-color-boot.scss)
- [ack-block-boot](https://ackerapple.github.io/ack-css-boot/#ack-block-boot)
  - [scss/ack-block-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-block-boot.scss)
- [ack-position-boot](https://ackerapple.github.io/ack-css-boot/#ack-position-boot)
  - [scss/ack-position-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-position-boot.scss)
- [ack-form-boot](https://ackerapple.github.io/ack-css-boot/#ack-form-boot)
  - [scss/ack-form-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-form-boot.scss)
- [ack-responsive-boot](https://ackerapple.github.io/ack-css-boot/#ack-responsive-boot)
  - [scss/ack-responsive-boot.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-responsive-boot.scss)
  - Screen size to size name map
    - xxs > 0 && <= 438
    - xs > 0 && <= 768
    - smx >=576 && < 768
    - sm >= 768 && < 992
    - md >= 992 && < 1200
    - lg >= 1200
  - The following classes, allow for css width/height transistion animations
    - .hide-width-
    - .hide-height-
    - .hide-max-width-
    - .hide-max-height-
- [ack-overrides](https://ackerapple.github.io/ack-css-boot/#ack-overrides)
  - [scss/ack-overrides.scss](https://github.com/AckerApple/ack-css-boot/blob/master/scss/ack-overrides.scss)

> Compiled versions, .css files, can be found in ack-cssboot/dist/
