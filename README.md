# SCSSETUP

![Mou icon](http://f.cl.ly/items/3G0x1M1i3f112F0N3P3f/scssetup-logo--v21.png)

## Overview

Scssetup **(sĕt′ŭp′)** is a Sass framework for building and maintaing large applications.

## Application.Sass

## Core
#### reset.sass
A style reset.  Using Eric Meyer's [Normalize](http://necolas.github.io/normalize.css/) for now.
#### settings.sass
Mostly `@font-face` declarations.  Add site-wide variable here `$baseFontSize: 16px`.  A great place for newcommers to learn about all of the variables used in the application.

```
// ----- Base Colors ----- //

$base-background: #fff
$base-color: #222
$base-link-color: #0053c9
```
#### helpers.sass
This is where we will set all of functions, extends, mixins, and animations

```
// ----- Image Replacement ----- //

%ir
  background-color: transparent
  border: 0
  overflow: hidden
  &:before
    content: ''
    display: block
    width: 0
    height: 150%
```
#### base.sass
This can be seen as another reset.

```
body
  background: $base-background
  color: $base-color
  font-family: $base-fontFamily
  font-size: 100%
  line-height: $base-lineHeight
```
#### content.sass
A place to setup site-wide Headings, and commonly used utilities.

```
h1, h2, h3,
h4, h5, h6
  font-family: $c-header-fontFamily
  font-weight: bold

h1, .c-h1, %c-h1
  font-size: rem(40px)
```

#### layout.sass

## Modules

