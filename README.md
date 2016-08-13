# ack-css-boot
A base set of short-hand css helper classes. Includes available classes that are commonly used for styling buttons, form inputs, and such.

Many commonly used short-hand classes, that are found in [Ionic](https://www.npmjs.com/package/ionic) and [Bootstrap](https://www.npmjs.com/package/bootstrap-css), can be found here.

### Table of Contents
- [Usage and Examples](#usage-and-examples)
- [ack-css-boot](#ack-css-boot)
- [ack-text-boot](#ack-text-boot)
- [ack-flex-boot](#ack-flex-boot)
- [ack-color-boot](#ack-color-boot)
- [ack-block-boot](#ack-block-boot)
- [ack-position-boot](#ack-position-boot)
- [ack-form-boot](#ack-form-boot)
- [ack-responsive-boot](#ack-responsive-boot)

## Usage and Examples
Learn about css short-hand classes such as .pad, .margin, .text-lg, and more...

[tap here to see demos](https://ackerapple.github.io/ack-css-boot/)

All examples seen below, are written in [Sass](http://sass-lang.com/) and then compiled to css in the /dist folder.


## ack-css-boot

> scss/ack-css-boot.scss

```
@import "./ack-text-boot";
@import "./ack-flex-boot";
@import "./ack-color-boot";
@import "./ack-block-boot";
@import "./ack-position-boot";
@import "./ack-form-boot";
@import "./ack-responsive-boot";
```


## ack-text-boot

> scss/ack-text-boot.scss

```
.nowrap {white-space:nowrap}

.font-arial {font-family:Arial}
.font-times {font-family:Times New Roman}
.font-helvetica {font-family:Helvetica}

.text-overflow {text-overflow:ellipsis;white-space:nowrap;overflow:hidden}

.text-underline,.underline {text-decoration:underline}
.strong, .bold, .text-bold {font-weight:bold}

.text-left {text-align:left}
.text-right {text-align:right}
.text-center {text-align:center}

.text-uppercase {text-transform: uppercase}
.text-lowercase {text-transform: lowercase}
.text-capitalize {text-transform: capitalize}

.text-5x {font-size:200%}
.text-4x {font-size:185%}
.text-3x {font-size:160%}
.text-2x {font-size:145%}
.text-lg {font-size:130%}
.text-md {font-size:115%}
.text-sm {font-size:90%}
.text-smx {font-size:85%}
.text-xs {font-size:75%}
.text-xxs {font-size:65%}

.line-height-0 {line-height:0}
.line-height-half {line-height:50%}
.line-height-third {line-height:33.3%}
.line-height-quarter {line-height:25%}
.line-height-2x {line-height:150%}
.line-height-3x {line-height:200%}
```


## ack-flex-boot

> scss/ack-flex-boot.scss

```
.flex, .display-flex {display:flex}
.flex-1 {flex-grow:1}
.flex-2 {flex-grow:2}
.flex-3 {flex-grow:3}
.flex-4 {flex-grow:4}
.flex-5 {flex-grow:5}
.flex-6 {flex-grow:6}

.flex-flow-inline, .flex-wrap {
  flex-flow:row wrap;
  flex-wrap:wrap;flex-direction:row;/*required for safari*/
}

.flex-left, .justify-left {justify-content:flex-start}
.flex-center, .justify-center {justify-content:center}
.flex-right, .justify-right {justify-content:flex-end}
.flex-apart, .flex-space-between, .justify-apart, .justify-space-between {justify-content:space-between}
.flex-evenly, .flex-space-around, .justify-space-around {justify-content:space-around}

.flex-valign, .flex-valign-top, .align-center {align-items:center}
.flex-valign-bottom, .align-bottom,.align-end {align-items:flex-end}
.flex-fill, .align-fill, .align-stretch {align-items:stretch}
.align-baseline {align-items:baseline}
```


## ack-color-boot

> scss/ack-color-boot.scss

```
.text-primary {color:#337ab7}
.text-success {color:#3c763d}
.text-info {color:#31708f}
.text-warning {color:#8a6d3b}
.text-danger {color:#a94442}

.text-muted-lg {color:#333}
.text-muted-md {color:#555}
.text-muted {color:#777}
.text-muted-sm, .text-muted-2x {color:#AAA}
.text-muted-xs, .text-muted-3x {color:#BAB}

.text-green,.font-green {color: #060}
.text-orange,.font-orange {color: #C60}
.text-red,.font-red {color:#900}
.text-blue,.font-blue {color: #009}
.text-purple,.font-purple {color: #60C}
.text-black,.font-black {color: #000}
.text-white,.font-white {color: #FFF}

.bg-white,.bg-lite {background-color:white}
.bg-black {background-color:black}

.bg-primary {background-color:#337ab7}
.bg-success {background-color:#dff0d8}
.bg-info {background-color:#d9edf7}
.bg-warning {background-color:#fcf8e3}
.bg-danger {background-color:#f2dede}
.bg-grey {background-color:#777}
.bg-grey-xs {background-color:#999}
.bg-grey-xxs {background-color:#BBB}

.bg-stable {background-color:#f8f8f8}
.bg-positive {background-color:#387ef5}
.bg-calm {background-color:#11c1f3}
.bg-balanced {background-color:#33cd5f}
.bg-energized {background-color:#ffc900}
.bg-assertive {background-color:#ef473a}
.bg-royal {background-color:#886aea}
.bg-dark {background-color:#444444}

.border-positive {border-color:#0c60ee}
.border-calm {border-color:#0a9dc7}
.border-balanced {border-color:#28a54c}
.border-energized {border-color:#e6b500}
.border-assertive {border-color:#e42112}
.border-royal {border-color:#6b46e5}
.border-dark {border-color:#111111}
.border-danger {border-color:#d43f3a}
.border-warning {border-color:#eea236}
.border-info {border-color:#46b8da}
.border-success {border-color:#4cae4c}
.border-primary {border-color:#2e6da4}

.border-1-0,.border-1-black {border-color:#000;border-width:1px;border-style:solid}
.border-1-f,.border-1-white {border-color:#FFF;border-width:1px;border-style:solid}
.border-1-positive {border-color:#0c60ee;border-width:1px;border-style:solid}
.border-1-calm {border-color:#0a9dc7;border-width:1px;border-style:solid}
.border-1-balanced {border-color:#28a54c;border-width:1px;border-style:solid}
.border-1-energized {border-color:#e6b500;border-width:1px;border-style:solid}
.border-1-assertive {border-color:#e42112;border-width:1px;border-style:solid}
.border-1-royal {border-color:#6b46e5;border-width:1px;border-style:solid}
.border-1-dark {border-color:#111111;border-width:1px;border-style:solid}
.border-1-danger {border-color:#d43f3a;border-width:1px;border-style:solid}
.border-1-warning {border-color:#eea236;border-width:1px;border-style:solid}
.border-1-info {border-color:#46b8da;border-width:1px;border-style:solid}
.border-1-success {border-color:#4cae4c;border-width:1px;border-style:solid}
.border-1-primary {border-color:#2e6da4;border-width:1px;border-style:solid}


.hover-text-shadow-grey-blur:hover{
  text-shadow:0 0 4px #777
}
.hover-text-shadow-white-blur:hover{
  text-shadow:0 0 4px #FFF
}
```


## ack-block-boot

> scss/ack-block-boot.scss

```
$em-xxs: 0.2em;
$em-xs: 0.4em;
$em-sm: 0.6em;
$em: 0.8em;
$em-md: 1em;
$em-lg: 1.5em;



a, .cursor-pointer {cursor:pointer}


.overflow-hidden {overflow:hidden}
.overflow, .overflow-auto {overflow:auto}
.overflow-y-auto {overflow-y:auto}
.overflow-y-hidden {overflow-y:hidden}
.overflow-x-auto {overflow-x:auto}
.overflow-x-hidden {overflow-x:hidden}


.visible, .visibility-visible {visibility:visible}
.invisible, .visibility-hidden {visibility:hidden}


.inline-block, .display-inline-block {display:inline-block}
.block, .display-block {display:block}


.opacity-90 {opacity: 0.9}
.opacity-80 {opacity: 0.8}
.opacity-75 {opacity: 0.75}
.opacity-70 {opacity: 0.7}
.opacity-60 {opacity: 0.6}
.opacity-50, .opacity-half {opacity: 0.5}
.opacity-40 {opacity: 0.4}
.opacity-30 {opacity: 0.3}
.opacity-25, .opacity-third {opacity: 0.25}
.opacity-20 {opacity: 0.2}
.opacity-10 {opacity: 0.1}


.border-radius-0 {border-radius:0}
.border-radius-3 {border-radius:3px}
.border-radius-4 {border-radius:4px}
.border-radius-5 {border-radius:5px}
.border-radius-6 {border-radius:6px}
.border-radius-7 {border-radius:7px}
.border-radius-8 {border-radius:8px}
.border-radius-9 {border-radius:9px}
.border-radius-10 {border-radius:10px}
.border-radius-15 {border-radius:15px}
.border-radius-20 {border-radius:20px}
.border-radius-25 {border-radius:25px}
.border-radius-half {border-radius:50%}
.border-spacing-0 {border-spacing:0}
.border-collapse {border-collapse:collapse}
.border-separate, .border-collapse-seperate {border-collapse:separate}
.border.border-1 {border-width:1px;border-style:solid;border-color:black;}
.border-2 {border-width:2px;border-style:solid;border-color:black;}
.border-3 {border-width:3px;border-style:solid;border-color:black;}
.border-4 {border-width:4px;border-style:solid;border-color:black;}
.border-5 {border-width:5px;border-style:solid;border-color:black;}
.border-6 {border-width:6px;border-style:solid;border-color:black;}
.border-7 {border-width:7px;border-style:solid;border-color:black;}
.border-8 {border-width:8px;border-style:solid;border-color:black;}
.border-solid {border-style:solid}
.border-dotted {border-style:dotted}
.border-dashed {border-style:dashed}


.width-0 {width:0}
.width-full, .full-width {width:100%}
.width-half, .half-width {width:50%}

.height-0 {height:0}
.height-full {height:100%}
.height-half {width:50%}


.margin-0 {margin:0}
.margin-xxs {margin:$em-xxs}
.margin-xs {margin:$em-xs}
.margin-sm {margin:$em-sm}
.margin {margin:$em}
.margin-md {margin:$em-md}
.margin-lg {margin:$em-lg}

.margin-v-0 {margin-top:0;margin-bottom:0}
.margin-v-xxs {margin-top:$em-xxs;margin-bottom:$em-xxs}
.margin-v-xs {margin-top:$em-xs;margin-bottom:$em-xs}
.margin-v-sm {margin-top:$em-sm;margin-bottom:$em-sm}
.margin-v {margin-top:$em;margin-bottom:$em}
.margin-v-md {margin-top:$em-md;margin-bottom:$em-md}
.margin-v-lg {margin-top:$em-lg;margin-bottom:$em-lg}

.margin-h-0 {margin-left:0;margin-right:0}
.margin-h-xxs {margin-left:$em-xxs;margin-right:$em-xxs}
.margin-h-xs {margin-left:$em-xs;margin-right:$em-xs}
.margin-h-sm {margin-left:$em-sm;margin-right:$em-sm}
.margin-h {margin-left:$em;margin-right:$em}
.margin-h-md {margin-left:$em-md;margin-right:$em-md}
.margin-h-lg {margin-left:$em-lg;margin-right:$em-lg}

.margin-top-0 {margin-top:0}
.margin-top-xxs {margin-top:$em-xxs}
.margin-top-xs {margin-top:$em-xs}
.margin-top-sm {margin-top:$em-sm}
.margin-top {margin-top:$em}
.margin-top-md {margin-top:$em-md}
.margin-top-lg {margin-top:$em-lg}

.margin-bottom-0 {margin-bottom:0}
.margin-bottom-xxs {margin-bottom:$em-xxs}
.margin-bottom-xs {margin-bottom:$em-xs}
.margin-bottom-sm {margin-bottom:$em-sm}
.margin-bottom {margin-bottom:$em}
.margin-bottom-md {margin-bottom:$em-md}
.margin-bottom-lg {margin-bottom:$em-lg}

.margin-left-0 {margin-left:0}
.margin-left-xxs {margin-left:$em-xxs}
.margin-left-xs {margin-left:$em-xs}
.margin-left-sm {margin-left:$em-sm}
.margin-left {margin-left:$em}
.margin-left-md {margin-left:$em-md}
.margin-left-lg {margin-left:$em-lg}

.margin-right-0 {margin-right:0}
.margin-right-xxs {margin-right:$em-xxs}
.margin-right-xs {margin-right:$em-xs}
.margin-right-sm {margin-right:$em-sm}
.margin-right {margin-right:$em}
.margin-right-md {margin-right:$em-md}
.margin-right-lg {margin-right:$em-lg}


.pad-0 {padding:0}
.pad-xxs {padding:$em-xxs}
.pad-xs {padding:$em-xs}
.pad-sm {padding:$em-sm}
.pad {padding:$em}
.pad-md {padding:$em-md}
.pad-lg {padding:$em-lg}

.pad-v-0 {padding-top:0;padding-bottom:0}
.pad-v-xxs {padding-top:$em-xxs;padding-bottom:$em-xxs}
.pad-v-xs {padding-top:$em-xs;padding-bottom:$em-xs}
.pad-v-sm {padding-top:$em-sm;padding-bottom:$em-sm}
.pad-v {padding-top:$em;padding-bottom:$em}
.pad-v-md {padding-top:$em-md;padding-bottom:$em-md}
.pad-v-lg {padding-top:$em-lg;padding-bottom:$em-lg}

.pad-h-0 {padding-left:0;padding-right:0}
.pad-h-xxs {padding-left:$em-xxs;padding-right:$em-xxs}
.pad-h-xs {padding-left:$em-xs;padding-right:$em-xs}
.pad-h-sm {padding-left:$em-sm;padding-right:$em-sm}
.pad-h {padding-left:$em;padding-right:$em}
.pad-h-md {padding-left:$em-md;padding-right:$em-md}
.pad-h-lg {padding-left:$em-lg;padding-right:$em-lg}

.pad-top-0 {padding-top:0}
.pad-top-xxs {padding-top:$em-xxs}
.pad-top-xs {padding-top:$em-xs}
.pad-top-sm {padding-top:$em-sm}
.pad-top {padding-top:$em}
.pad-top-md {padding-top:$em-md}
.pad-top-lg {padding-top:$em-lg}

.pad-bottom-0 {padding-bottom:0}
.pad-bottom-xxs {padding-bottom:$em-xxs}
.pad-bottom-xs {padding-bottom:$em-xs}
.pad-bottom-sm {padding-bottom:$em-sm}
.pad-bottom {padding-bottom:$em}
.pad-bottom-md {padding-bottom:$em-md}
.pad-bottom-lg {padding-bottom:$em-lg}

.pad-left-0 {padding-left:0}
.pad-left-xxs {padding-left:$em-xxs}
.pad-left-xs {padding-left:$em-xs}
.pad-left-sm {padding-left:$em-sm}
.pad-left {padding-left:$em}
.pad-left-md {padding-left:$em-md}
.pad-left-lg {padding-left:$em-lg}

.pad-right-0 {padding-right:0}
.pad-right-xxs {padding-right:$em-xxs}
.pad-right-xs {padding-right:$em-xs}
.pad-right-sm {padding-right:$em-sm}
.pad-right {padding-right:$em}
.pad-right-md {padding-right:$em-md}
.pad-right-lg {padding-right:$em-lg}


.min-height {min-height:0}
.min-width {min-width:0}
.max-height {max-height:100%}
.max-width {max-width:100%}
.max-height-50 {max-height:50px}
.max-width-50 {max-width:50px}
.max-height-100 {max-height:100px}
.max-width-100 {max-width:100px}
.max-height-500 {max-height:500px}
.max-width-500 {max-width:500px}
.max-height-900 {max-height:900px}
.max-width-900 {max-width:900px}
.max-height-1000 {max-height:1000px}
.max-width-1000 {max-width:1000px}
.min-height-50 {min-height:50px}
.min-width-50 {min-width:50px}
.min-height-100 {min-height:100px}
.min-width-100 {min-width:100px}
.min-height-500 {min-height:500px}
.min-width-500 {min-width:500px}
.min-height-1000 {min-height:1000px}
.min-width-1000 {min-width:1000px}


/* TABLE PADDING CLASSES */
.table-pad-0>tbody>tr>td, .table-pad-0>tbody>tr>th, .table-pad-0>tfoot>tr>td,
.table-pad-0>tfoot>tr>th, .table-pad-0>thead>tr>td, .table-pad-0>thead>tr>th,
table>tbody>tr>td.pad-0, table>tbody>tr>th.pad-0, table>tfoot>tr>td.pad-0,
table>tfoot>tr>th.pad-0, table>thead>tr>td.pad-0, table>thead>tr>th.pad-0
{padding:0}

.table-pad-xxs>tbody>tr>td, .table-pad-xxs>tbody>tr>th, .table-pad-xxs>tfoot>tr>td,
.table-pad-xxs>tfoot>tr>th, .table-pad-xxs>thead>tr>td, .table-pad-xxs>thead>tr>th,
table>tbody>tr>td.pad-xxs, table>tbody>tr>th.pad-xxs, table>tfoot>tr>td.pad-xxs,
table>tfoot>tr>th.pad-xxs, table>thead>tr>td.pad-xxs, table>thead>tr>th.pad-xxs
{padding:$em-xxs}

.table-pad-xs>tbody>tr>td, .table-pad-xs>tbody>tr>th, .table-pad-xs>tfoot>tr>td,
.table-pad-xs>tfoot>tr>th, .table-pad-xs>thead>tr>td, .table-pad-xs>thead>tr>th,
table>tbody>tr>td.pad-xs, table>tbody>tr>th.pad-xs, table>tfoot>tr>td.pad-xs,
table>tfoot>tr>th.pad-xs, table>thead>tr>td.pad-xs, table>thead>tr>th.pad-xs
{padding:$em-xs}

.table-pad-sm>tbody>tr>td, .table-pad-sm>tbody>tr>th, .table-pad-sm>tfoot>tr>td,
.table-pad-sm>tfoot>tr>th, .table-pad-sm>thead>tr>td, .table-pad-sm>thead>tr>th,
table>tbody>tr>td.pad-sm, table>tbody>tr>th.pad-sm, table>tfoot>tr>td.pad-sm,
table>tfoot>tr>th.pad-sm, table>thead>tr>td.pad-sm, table>thead>tr>th.pad-sm
{padding:$em-sm}

.table-pad>tbody>tr>td, .table-pad>tbody>tr>th, .table-pad>tfoot>tr>td,
.table-pad>tfoot>tr>th, .table-pad>thead>tr>td, .table-pad>thead>tr>th,
table>tbody>tr>td.pad, table>tbody>tr>th.pad, table>tfoot>tr>td.pad,
table>tfoot>tr>th.pad, table>thead>tr>td.pad, table>thead>tr>th.pad
{padding:$em}

.table-pad-md>tbody>tr>td, .table-pad-md>tbody>tr>th, .table-pad-md>tfoot>tr>td,
.table-pad-md>tfoot>tr>th, .table-pad-md>thead>tr>td, .table-pad-md>thead>tr>th,
table>tbody>tr>td.pad-md, table>tbody>tr>th.pad-md, table>tfoot>tr>td.pad-md,
table>tfoot>tr>th.pad-md, table>thead>tr>td.pad-md, table>thead>tr>th.pad-md
{padding:$em-md}

.table-pad-lg>tbody>tr>td, .table-pad-lg>tbody>tr>th, .table-pad-lg>tfoot>tr>td,
.table-pad-lg>tfoot>tr>th, .table-pad-lg>thead>tr>td, .table-pad-lg>thead>tr>th,
table>tbody>tr>td.pad-lg, table>tbody>tr>th.pad-lg, table>tfoot>tr>td.pad-lg,
table>tfoot>tr>th.pad-lg, table>thead>tr>td.pad-lg, table>thead>tr>th.pad-lg
{padding:$em-lg}

.table-pad-v-0>tbody>tr>td, .table-pad-v-0>tbody>tr>th, .table-pad-v-0>tfoot>tr>td,
.table-pad-v-0>tfoot>tr>th, .table-pad-v-0>thead>tr>td, .table-pad-v-0>thead>tr>th,
table>tbody>tr>td.pad-v-0, table>tbody>tr>th.pad-v-0, table>tfoot>tr>td.pad-v-0,
table>tfoot>tr>th.pad-v-0, table>thead>tr>td.pad-v-0, table>thead>tr>th.pad-v-0
{padding-top:0;padding-bottom:0}
.table-pad-v-xxs>tbody>tr>td, .table-pad-v-xxs>tbody>tr>th, .table-pad-v-xxs>tfoot>tr>td,
.table-pad-v-xxs>tfoot>tr>th, .table-pad-v-xxs>thead>tr>td, .table-pad-v-xxs>thead>tr>th,
table>tbody>tr>td.pad-v-xxs, table>tbody>tr>th.pad-v-xxs, table>tfoot>tr>td.pad-v-xxs,
table>tfoot>tr>th.pad-v-xxs, table>thead>tr>td.pad-v-xxs, table>thead>tr>th.pad-v-xxs
{padding-top:$em-xxs;padding-bottom:$em-xxs}
.table-pad-v-xs>tbody>tr>td, .table-pad-v-xs>tbody>tr>th, .table-pad-v-xs>tfoot>tr>td,
.table-pad-v-xs>tfoot>tr>th, .table-pad-v-xs>thead>tr>td, .table-pad-v-xs>thead>tr>th,
table>tbody>tr>td.pad-v-xs, table>tbody>tr>th.pad-v-xs, table>tfoot>tr>td.pad-v-xs,
table>tfoot>tr>th.pad-v-xs, table>thead>tr>td.pad-v-xs, table>thead>tr>th.pad-v-xs
{padding-top:$em-xs;padding-bottom:$em-xs}
.table-pad-v-sm>tbody>tr>td, .table-pad-v-sm>tbody>tr>th, .table-pad-v-sm>tfoot>tr>td,
.table-pad-v-sm>tfoot>tr>th, .table-pad-v-sm>thead>tr>td, .table-pad-v-sm>thead>tr>th,
table>tbody>tr>td.pad-v-sm, table>tbody>tr>th.pad-v-sm, table>tfoot>tr>td.pad-v-sm,
table>tfoot>tr>th.pad-v-sm, table>thead>tr>td.pad-v-sm, table>thead>tr>th.pad-v-sm
{padding-top:$em-sm;padding-bottom:$em-sm}
.table-pad-v>tbody>tr>td, .table-pad-v>tbody>tr>th, .table-pad-v>tfoot>tr>td,
.table-pad-v>tfoot>tr>th, .table-pad-v>thead>tr>td, .table-pad-v>thead>tr>th,
table>tbody>tr>td.pad-v, table>tbody>tr>th.pad-v, table>tfoot>tr>td.pad-v,
table>tfoot>tr>th.pad-v, table>thead>tr>td.pad-v, table>thead>tr>th.pad-v
{padding-top:$em;padding-bottom:$em}
.table-pad-v-md>tbody>tr>td, .table-pad-v-md>tbody>tr>th, .table-pad-v-md>tfoot>tr>td,
.table-pad-v-md>tfoot>tr>th, .table-pad-v-md>thead>tr>td, .table-pad-v-md>thead>tr>th,
table>tbody>tr>td.pad-v-md, table>tbody>tr>th.pad-v-md, table>tfoot>tr>td.pad-v-md,
table>tfoot>tr>th.pad-v-md, table>thead>tr>td.pad-v-md, table>thead>tr>th.pad-v-md
{padding-top:$em-md;padding-bottom:$em-md}
.table-pad-v-lg>tbody>tr>td, .table-pad-v-lg>tbody>tr>th, .table-pad-v-lg>tfoot>tr>td,
.table-pad-v-lg>tfoot>tr>th, .table-pad-v-lg>thead>tr>td, .table-pad-v-lg>thead>tr>th,
table>tbody>tr>td.pad-v-lg, table>tbody>tr>th.pad-v-lg, table>tfoot>tr>td.pad-v-lg,
table>tfoot>tr>th.pad-v-lg, table>thead>tr>td.pad-v-lg, table>thead>tr>th.pad-v-lg
{padding-top:$em-lg;padding-bottom:$em-lg}

.table-pad-h-0>tbody>tr>td, .table-pad-h-0>tbody>tr>th, .table-pad-h-0>tfoot>tr>td,
.table-pad-h-0>tfoot>tr>th, .table-pad-h-0>thead>tr>td, .table-pad-h-0>thead>tr>th,
table>tbody>tr>td.pad-h-0, table>tbody>tr>th.pad-h-0, table>tfoot>tr>td.pad-h-0,
table>tfoot>tr>th.pad-h-0, table>thead>tr>td.pad-h-0, table>thead>tr>th.pad-h-0
{padding-left:0;padding-right:0}
.table-pad-h-xxs>tbody>tr>td, .table-pad-h-xxs>tbody>tr>th, .table-pad-h-xxs>tfoot>tr>td,
.table-pad-h-xxs>tfoot>tr>th, .table-pad-h-xxs>thead>tr>td, .table-pad-h-xxs>thead>tr>th,
table>tbody>tr>td.pad-h-xxs, table>tbody>tr>th.pad-h-xxs, table>tfoot>tr>td.pad-h-xxs,
table>tfoot>tr>th.pad-h-xxs, table>thead>tr>td.pad-h-xxs, table>thead>tr>th.pad-h-xxs
{padding-left:$em-xxs;padding-right:$em-xxs}
.table-pad-h-xs>tbody>tr>td, .table-pad-h-xs>tbody>tr>th, .table-pad-h-xs>tfoot>tr>td,
.table-pad-h-xs>tfoot>tr>th, .table-pad-h-xs>thead>tr>td, .table-pad-h-xs>thead>tr>th,
table>tbody>tr>td.pad-h-xs, table>tbody>tr>th.pad-h-xs, table>tfoot>tr>td.pad-h-xs,
table>tfoot>tr>th.pad-h-xs, table>thead>tr>td.pad-h-xs, table>thead>tr>th.pad-h-xs
{padding-left:$em-xs;padding-right:$em-xs}
.table-pad-h-sm>tbody>tr>td, .table-pad-h-sm>tbody>tr>th, .table-pad-h-sm>tfoot>tr>td,
.table-pad-h-sm>tfoot>tr>th, .table-pad-h-sm>thead>tr>td, .table-pad-h-sm>thead>tr>th,
table>tbody>tr>td.pad-h-sm, table>tbody>tr>th.pad-h-sm, table>tfoot>tr>td.pad-h-sm,
table>tfoot>tr>th.pad-h-sm, table>thead>tr>td.pad-h-sm, table>thead>tr>th.pad-h-sm
{padding-left:$em-sm;padding-right:$em-sm}
.table-pad-h>tbody>tr>td, .table-pad-h>tbody>tr>th, .table-pad-h>tfoot>tr>td,
.table-pad-h>tfoot>tr>th, .table-pad-h>thead>tr>td, .table-pad-h>thead>tr>th,
table>tbody>tr>td.pad-h, table>tbody>tr>th.pad-h, table>tfoot>tr>td.pad-h,
table>tfoot>tr>th.pad-h, table>thead>tr>td.pad-h, table>thead>tr>th.pad-h
{padding-left:$em;padding-right:$em}
.table-pad-h-md>tbody>tr>td, .table-pad-h-md>tbody>tr>th, .table-pad-h-md>tfoot>tr>td,
.table-pad-h-md>tfoot>tr>th, .table-pad-h-md>thead>tr>td, .table-pad-h-md>thead>tr>th,
table>tbody>tr>td.pad-h-md, table>tbody>tr>th.pad-h-md, table>tfoot>tr>td.pad-h-md,
table>tfoot>tr>th.pad-h-md, table>thead>tr>td.pad-h-md, table>thead>tr>th.pad-h-md
{padding-left:$em-md;padding-right:$em-md}
.table-pad-h-lg>tbody>tr>td, .table-pad-h-lg>tbody>tr>th, .table-pad-h-lg>tfoot>tr>td,
.table-pad-h-lg>tfoot>tr>th, .table-pad-h-lg>thead>tr>td, .table-pad-h-lg>thead>tr>th,
table>tbody>tr>td.pad-h-lg, table>tbody>tr>th.pad-h-lg, table>tfoot>tr>td.pad-h-lg,
table>tfoot>tr>th.pad-h-lg, table>thead>tr>td.pad-h-lg, table>thead>tr>th.pad-h-lg
{padding-left:$em-lg;padding-right:$em-lg}

.table-pad-top-0>tbody>tr>td, .table-pad-top-0>tbody>tr>th, .table-pad-top-0>tfoot>tr>td,
.table-pad-top-0>tfoot>tr>th, .table-pad-top-0>thead>tr>td, .table-pad-top-0>thead>tr>th,
table>tbody>tr>td.pad-top-0, table>tbody>tr>th.pad-top-0, table>tfoot>tr>td.pad-top-0,
table>tfoot>tr>th.pad-top-0, table>thead>tr>td.pad-top-0, table>thead>tr>th.pad-top-0
{padding-top:0}
.table-pad-top-xxs>tbody>tr>td, .table-pad-top-xxs>tbody>tr>th, .table-pad-top-xxs>tfoot>tr>td,
.table-pad-top-xxs>tfoot>tr>th, .table-pad-top-xxs>thead>tr>td, .table-pad-top-xxs>thead>tr>th,
table>tbody>tr>td.pad-top-xxs, table>tbody>tr>th.pad-top-xxs, table>tfoot>tr>td.pad-top-xxs,
table>tfoot>tr>th.pad-top-xxs, table>thead>tr>td.pad-top-xxs, table>thead>tr>th.pad-top-xxs
{padding-top:$em-xxs}
.table-pad-top-xs>tbody>tr>td, .table-pad-top-xs>tbody>tr>th, .table-pad-top-xs>tfoot>tr>td,
.table-pad-top-xs>tfoot>tr>th, .table-pad-top-xs>thead>tr>td, .table-pad-top-xs>thead>tr>th,
table>tbody>tr>td.pad-top-xs, table>tbody>tr>th.pad-top-xs, table>tfoot>tr>td.pad-top-xs,
table>tfoot>tr>th.pad-top-xs, table>thead>tr>td.pad-top-xs, table>thead>tr>th.pad-top-xs
{padding-top:$em-xs}
.table-pad-top-sm>tbody>tr>td, .table-pad-top-sm>tbody>tr>th, .table-pad-top-sm>tfoot>tr>td,
.table-pad-top-sm>tfoot>tr>th, .table-pad-top-sm>thead>tr>td, .table-pad-top-sm>thead>tr>th,
table>tbody>tr>td.pad-top-sm, table>tbody>tr>th.pad-top-sm, table>tfoot>tr>td.pad-top-sm,
table>tfoot>tr>th.pad-top-sm, table>thead>tr>td.pad-top-sm, table>thead>tr>th.pad-top-sm
{padding-top:$em-sm}
.table-pad-top>tbody>tr>td, .table-pad-top>tbody>tr>th, .table-pad-top>tfoot>tr>td,
.table-pad-top>tfoot>tr>th, .table-pad-top>thead>tr>td, .table-pad-top>thead>tr>th,
table>tbody>tr>td.pad-top, table>tbody>tr>th.pad-top, table>tfoot>tr>td.pad-top,
table>tfoot>tr>th.pad-top, table>thead>tr>td.pad-top, table>thead>tr>th.pad-top
{padding-top:$em}
.table-pad-top-md>tbody>tr>td, .table-pad-top-md>tbody>tr>th, .table-pad-top-md>tfoot>tr>td,
.table-pad-top-md>tfoot>tr>th, .table-pad-top-md>thead>tr>td, .table-pad-top-md>thead>tr>th,
table>tbody>tr>td.pad-top-md, table>tbody>tr>th.pad-top-md, table>tfoot>tr>td.pad-top-md,
table>tfoot>tr>th.pad-top-md, table>thead>tr>td.pad-top-md, table>thead>tr>th.pad-top-md
{padding-top:$em-md}
.table-pad-top-lg>tbody>tr>td, .table-pad-top-lg>tbody>tr>th, .table-pad-top-lg>tfoot>tr>td,
.table-pad-top-lg>tfoot>tr>th, .table-pad-top-lg>thead>tr>td, .table-pad-top-lg>thead>tr>th,
table>tbody>tr>td.pad-top-lg, table>tbody>tr>th.pad-top-lg, table>tfoot>tr>td.pad-top-lg,
table>tfoot>tr>th.pad-top-lg, table>thead>tr>td.pad-top-lg, table>thead>tr>th.pad-top-lg
{padding-top:$em-lg}

.table-pad-bottom-0>tbody>tr>td, .table-pad-bottom-0>tbody>tr>th, .table-pad-bottom-0>tfoot>tr>td,
.table-pad-bottom-0>tfoot>tr>th, .table-pad-bottom-0>thead>tr>td, .table-pad-bottom-0>thead>tr>th,
table>tbody>tr>td.pad-bottom-0, table>tbody>tr>th.pad-bottom-0, table>tfoot>tr>td.pad-bottom-0,
table>tfoot>tr>th.pad-bottom-0, table>thead>tr>td.pad-bottom-0, table>thead>tr>th.pad-bottom-0
{padding-bottom:0}
.table-pad-bottom-xxs>tbody>tr>td, .table-pad-bottom-xxs>tbody>tr>th, .table-pad-bottom-xxs>tfoot>tr>td,
.table-pad-bottom-xxs>tfoot>tr>th, .table-pad-bottom-xxs>thead>tr>td, .table-pad-bottom-xxs>thead>tr>th,
table>tbody>tr>td.pad-bottom-xxs, table>tbody>tr>th.pad-bottom-xxs, table>tfoot>tr>td.pad-bottom-xxs,
table>tfoot>tr>th.pad-bottom-xxs, table>thead>tr>td.pad-bottom-xxs, table>thead>tr>th.pad-bottom-xxs
{padding-bottom:$em-xxs}
.table-pad-bottom-xs>tbody>tr>td, .table-pad-bottom-xs>tbody>tr>th, .table-pad-bottom-xs>tfoot>tr>td,
.table-pad-bottom-xs>tfoot>tr>th, .table-pad-bottom-xs>thead>tr>td, .table-pad-bottom-xs>thead>tr>th,
table>tbody>tr>td.pad-bottom-xs, table>tbody>tr>th.pad-bottom-xs, table>tfoot>tr>td.pad-bottom-xs,
table>tfoot>tr>th.pad-bottom-xs, table>thead>tr>td.pad-bottom-xs, table>thead>tr>th.pad-bottom-xs
{padding-bottom:$em-xs}
.table-pad-bottom-sm>tbody>tr>td, .table-pad-bottom-sm>tbody>tr>th, .table-pad-bottom-sm>tfoot>tr>td,
.table-pad-bottom-sm>tfoot>tr>th, .table-pad-bottom-sm>thead>tr>td, .table-pad-bottom-sm>thead>tr>th,
table>tbody>tr>td.pad-bottom-sm, table>tbody>tr>th.pad-bottom-sm, table>tfoot>tr>td.pad-bottom-sm,
table>tfoot>tr>th.pad-bottom-sm, table>thead>tr>td.pad-bottom-sm, table>thead>tr>th.pad-bottom-sm
{padding-bottom:$em-sm}
table>tr>td,.pad-bottom>tbody .table-pad-bottom>tbody>tr>th, .table-pad-bottom>tfoot>tr>td,
.table-pad-bottom>tfoot>tr>th, .table-pad-bottom>thead>tr>td, .table-pad-bottom>thead>tr>th,
.table-pad-bottom>tbody>tr>td, .table-pad-bottom>tbody>tr>th, .table-pad-bottom>tfoot>tr>td,
.table-pad-bottom>tfoot>tr>th, .table-pad-bottom>thead>tr>td, .table-pad-bottom>thead>tr>th
{padding-bottom:$em}
.table-pad-bottom-md>tbody>tr>td, .table-pad-bottom-md>tbody>tr>th, .table-pad-bottom-md>tfoot>tr>td,
.table-pad-bottom-md>tfoot>tr>th, .table-pad-bottom-md>thead>tr>td, .table-pad-bottom-md>thead>tr>th,
table>tbody>tr>td.pad-bottom-md, table>tbody>tr>th.pad-bottom-md, table>tfoot>tr>td.pad-bottom-md,
table>tfoot>tr>th.pad-bottom-md, table>thead>tr>td.pad-bottom-md, table>thead>tr>th.pad-bottom-md
{padding-bottom:$em-md}
.table-pad-bottom-lg>tbody>tr>td, .table-pad-bottom-lg>tbody>tr>th, .table-pad-bottom-lg>tfoot>tr>td,
.table-pad-bottom-lg>tfoot>tr>th, .table-pad-bottom-lg>thead>tr>td, .table-pad-bottom-lg>thead>tr>th,
table>tbody>tr>td.pad-bottom-lg, table>tbody>tr>th.pad-bottom-lg, table>tfoot>tr>td.pad-bottom-lg,
table>tfoot>tr>th.pad-bottom-lg, table>thead>tr>td.pad-bottom-lg, table>thead>tr>th.pad-bottom-lg
{padding-bottom:$em-lg}

.table-pad-left-0>tbody>tr>td, .table-pad-left-0>tbody>tr>th, .table-pad-left-0>tfoot>tr>td,
.table-pad-left-0>tfoot>tr>th, .table-pad-left-0>thead>tr>td, .table-pad-left-0>thead>tr>th,
table>tbody>tr>td.pad-left-0, table>tbody>tr>th.pad-left-0, table>tfoot>tr>td.pad-left-0,
table>tfoot>tr>th.pad-left-0, table>thead>tr>td.pad-left-0, table>thead>tr>th.pad-left-0
{padding-left:0}
.table-pad-left-xxs>tbody>tr>td, .table-pad-left-xxs>tbody>tr>th, .table-pad-left-xxs>tfoot>tr>td,
.table-pad-left-xxs>tfoot>tr>th, .table-pad-left-xxs>thead>tr>td, .table-pad-left-xxs>thead>tr>th,
table>tbody>tr>td.pad-left-xxs, table>tbody>tr>th.pad-left-xxs, table>tfoot>tr>td.pad-left-xxs,
table>tfoot>tr>th.pad-left-xxs, table>thead>tr>td.pad-left-xxs, table>thead>tr>th.pad-left-xxs
{padding-left:$em-xxs}
.table-pad-left-xs>tbody>tr>td, .table-pad-left-xs>tbody>tr>th, .table-pad-left-xs>tfoot>tr>td,
.table-pad-left-xs>tfoot>tr>th, .table-pad-left-xs>thead>tr>td, .table-pad-left-xs>thead>tr>th,
table>tbody>tr>td.pad-left-xs, table>tbody>tr>th.pad-left-xs, table>tfoot>tr>td.pad-left-xs,
table>tfoot>tr>th.pad-left-xs, table>thead>tr>td.pad-left-xs, table>thead>tr>th.pad-left-xs
{padding-left:$em-xs}
.table-pad-left-sm>tbody>tr>td, .table-pad-left-sm>tbody>tr>th, .table-pad-left-sm>tfoot>tr>td,
.table-pad-left-sm>tfoot>tr>th, .table-pad-left-sm>thead>tr>td, .table-pad-left-sm>thead>tr>th,
table>tbody>tr>td.pad-left-sm, table>tbody>tr>th.pad-left-sm, table>tfoot>tr>td.pad-left-sm,
table>tfoot>tr>th.pad-left-sm, table>thead>tr>td.pad-left-sm, table>thead>tr>th.pad-left-sm
{padding-left:$em-sm}
.table-pad-left>tbody>tr>td, .table-pad-left>tbody>tr>th, .table-pad-left>tfoot>tr>td,
.table-pad-left>tfoot>tr>th, .table-pad-left>thead>tr>td, .table-pad-left>thead>tr>th,
table>tbody>tr>td.pad-left, table>tbody>tr>th.pad-left, table>tfoot>tr>td.pad-left,
table>tfoot>tr>th.pad-left, table>thead>tr>td.pad-left, table>thead>tr>th.pad-left
{padding-left:$em}
.table-pad-left-md>tbody>tr>td, .table-pad-left-md>tbody>tr>th, .table-pad-left-md>tfoot>tr>td,
.table-pad-left-md>tfoot>tr>th, .table-pad-left-md>thead>tr>td, .table-pad-left-md>thead>tr>th,
table>tbody>tr>td.pad-left-md, table>tbody>tr>th.pad-left-md, table>tfoot>tr>td.pad-left-md,
table>tfoot>tr>th.pad-left-md, table>thead>tr>td.pad-left-md, table>thead>tr>th.pad-left-md
{padding-left:$em-md}
.table-pad-left-lg>tbody>tr>td, .table-pad-left-lg>tbody>tr>th, .table-pad-left-lg>tfoot>tr>td,
.table-pad-left-lg>tfoot>tr>th, .table-pad-left-lg>thead>tr>td, .table-pad-left-lg>thead>tr>th,
table>tbody>tr>td.pad-left-lg, table>tbody>tr>th.pad-left-lg, table>tfoot>tr>td.pad-left-lg,
table>tfoot>tr>th.pad-left-lg, table>thead>tr>td.pad-left-lg, table>thead>tr>th.pad-left-lg
{padding-left:$em-lg}

.table-pad-right-0>tbody>tr>td, .table-pad-right-0>tbody>tr>th, .table-pad-right-0>tfoot>tr>td,
.table-pad-right-0>tfoot>tr>th, .table-pad-right-0>thead>tr>td, .table-pad-right-0>thead>tr>th,
table>tbody>tr>td.pad-right-0, table>tbody>tr>th.pad-right-0, table>tfoot>tr>td.pad-right-0,
table>tfoot>tr>th.pad-right-0, table>thead>tr>td.pad-right-0, table>thead>tr>th.pad-right-0
{padding-right:0}
.table-pad-right-xxs>tbody>tr>td, .table-pad-right-xxs>tbody>tr>th, .table-pad-right-xxs>tfoot>tr>td,
.table-pad-right-xxs>tfoot>tr>th, .table-pad-right-xxs>thead>tr>td, .table-pad-right-xxs>thead>tr>th,
table>tbody>tr>td.pad-right-xxs, table>tbody>tr>th.pad-right-xxs, table>tfoot>tr>td.pad-right-xxs,
table>tfoot>tr>th.pad-right-xxs, table>thead>tr>td.pad-right-xxs, table>thead>tr>th.pad-right-xxs
{padding-right:$em-xxs}
.table-pad-right-xs>tbody>tr>td, .table-pad-right-xs>tbody>tr>th, .table-pad-right-xs>tfoot>tr>td,
.table-pad-right-xs>tfoot>tr>th, .table-pad-right-xs>thead>tr>td, .table-pad-right-xs>thead>tr>th,
table>tbody>tr>td.pad-right-xs, table>tbody>tr>th.pad-right-xs, table>tfoot>tr>td.pad-right-xs,
table>tfoot>tr>th.pad-right-xs, table>thead>tr>td.pad-right-xs, table>thead>tr>th.pad-right-xs
{padding-right:$em-xs}
.table-pad-right-sm>tbody>tr>td, .table-pad-right-sm>tbody>tr>th, .table-pad-right-sm>tfoot>tr>td,
.table-pad-right-sm>tfoot>tr>th, .table-pad-right-sm>thead>tr>td, .table-pad-right-sm>thead>tr>th,
table>tbody>tr>td.pad-right-sm, table>tbody>tr>th.pad-right-sm, table>tfoot>tr>td.pad-right-sm,
table>tfoot>tr>th.pad-right-sm, table>thead>tr>td.pad-right-sm, table>thead>tr>th.pad-right-sm
{padding-right:$em-sm}
.table-pad-right>tbody>tr>td, .table-pad-right>tbody>tr>th, .table-pad-right>tfoot>tr>td,
.table-pad-right>tfoot>tr>th, .table-pad-right>thead>tr>td, .table-pad-right>thead>tr>th,
table>tbody>tr>td.pad-right, table>tbody>tr>th.pad-right, table>tfoot>tr>td.pad-right,
table>tfoot>tr>th.pad-right, table>thead>tr>td.pad-right, table>thead>tr>th.pad-right
{padding-right:$em}
.table-pad-right-md>tbody>tr>td, .table-pad-right-md>tbody>tr>th, .table-pad-right-md>tfoot>tr>td,
.table-pad-right-md>tfoot>tr>th, .table-pad-right-md>thead>tr>td, .table-pad-right-md>thead>tr>th,
table>tbody>tr>td.pad-right-md, table>tbody>tr>th.pad-right-md, table>tfoot>tr>td.pad-right-md,
table>tfoot>tr>th.pad-right-md, table>thead>tr>td.pad-right-md, table>thead>tr>th.pad-right-md
{padding-right:$em-md}
.table-pad-right-lg>tbody>tr>td, .table-pad-right-lg>tbody>tr>th, .table-pad-right-lg>tfoot>tr>td,
.table-pad-right-lg>tfoot>tr>th, .table-pad-right-lg>thead>tr>td, .table-pad-right-lg>thead>tr>th,
table>tbody>tr>td.pad-right-lg, table>tbody>tr>th.pad-right-lg, table>tfoot>tr>td.pad-right-lg,
table>tfoot>tr>th.pad-right-lg, table>thead>tr>td.pad-right-lg, table>thead>tr>th.pad-right-lg
{padding-right:$em-lg}
```


## ack-position-boot

> scss/ack-position-boot.scss

```
.valign,.valign-top,.vert-align-top {vertical-align:top}
.valign-middle,.valign-center,.vert-align-middle {vertical-align:middle}
.valign-bottom,.vert-align-bottom {vertical-align:bottom}

.pos-absolute,.pos-abs {position:absolute}
.pos-relative,.pos-rel {position:relative}
.pos-fixed,.pos-fix {position:fixed}

.z-index-1 {z-index:1}
.z-index-10 {z-index:10}
.top-0 {top:0}
.right-0 {right:0}
.bottom-0 {bottom:0}
.left-0 {left:0}


.clear,.clear-both,.clear-fix {clear:both}
.float-right, .pull-right {float:right}
.float-left, .pull-left {float:left}
```


## ack-form-boot

> scss/ack-form-boot.scss

```
.form-group.has-error label:first-child {
  color:#d43f3a;
}

.form-group.has-error input,
.form-group.has-error select,
.form-group.has-error textarea {
  border:1px solid #d43f3a;
}
```


## ack-responsive-boot

> scss/ack-responsive-boot.scss

> Screen size to size name map
- xxs > 0 && <= 438
- xs > 0 && <= 768
- smx >=576 && < 768
- sm >= 768 && < 992
- md >= 992 && < 1200
- lg >= 1200

> The following classes, allow for css width/height transistion animations
- .hide-width-
- .hide-height-
- .hide-max-width-
- .hide-max-height-

```
@media (max-width: 437px) {
  .hide-xxs, .hidden-xxs {
    display: none !important;
  }
  .hide-width-xxs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-xxs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-xxs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-xxs{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 767px) {
  .hide-xs, .hidden-xs {
    display: none !important;
  }
  .hide-width-xs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-xs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-xs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-xs{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (min-width: 576px) and (max-width: 767px) {
  .hide-smx, .hidden-smx {
    display: none !important;
  }
  .hide-width-smx{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-smx{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-smx{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-smx{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hide-sm, .hidden-sm {
    display: none !important;
  }
  .hide-width-sm{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-sm{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-sm{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-sm{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hide-md, .hidden-md {
    display: none !important;
  }
  .hide-width-md{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-md{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-md{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-md{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (min-width: 1200px) {
  .hide-lg, .hidden-lg {
    display: none !important;
  }
  .hide-width-lg{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lg{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lg{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lg{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media print {
  .hide-print, .hidden-print {
    display: none !important;
  }
}


/* HIDDEN ABOVES */
@media (min-width: 439px) {
  .hide-gt-xxs, .hide-above-xxs, .hidden-above-xxs {
    display: none !important;
  }
  .hide-width-gt-xxs, .hide-width-above-xxs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-gt-xxs, .hide-height-above-xxs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-gt-xxs, .hide-max-width-above-xxs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-gt-xxs, .hide-max-height-above-xxs{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (min-width: 769px) {
  .hide-gt-xs, .hide-above-xs, .hidden-above-xs {
    display: none !important;
  }
  .hide-width-gt-xs, .hide-width-above-xs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-gt-xs, .hide-height-above-xs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-gt-xs, .hide-max-width-above-xs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-gt-xs, .hide-max-height-above-xs{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (min-width: 577px) {
  .hide-gt-smx, .hide-above-smx, .hidden-above-smx {
    display: none !important;
  }
  .hide-width-gt-smx, .hide-width-above-smx{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-gt-smx, .hide-height-above-smx{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-gt-smx, .hide-max-width-above-smx{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-gt-smx, .hide-max-height-above-smx{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (min-width: 993px) {
  .hide-gt-sm, .hide-above-sm, .hidden-above-sm{
    display: none !important;
  }
  .hide-width-gt-sm, .hide-width-above-sm{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-gt-sm, .hide-height-above-sm{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-gt-sm, .hide-max-width-above-sm{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-gt-sm, .hide-max-height-above-sm{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (min-width: 1201px) {
  .hide-gt-md, .hide-above-md, .hidden-above-md{
    display: none !important;
  }
  .hide-width-gt-md, .hide-width-above-md{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-gt-md, .hide-height-above-md{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-gt-md, .hide-max-width-above-md{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-gt-md, .hide-max-height-above-md{
    max-height:0 !important;overflow:hidden !important;
  }
}


/* HIDDEN BELOWS */
@media (max-width: 439px) {
  .hide-lte-xxs, .hidden-lte-xxs {
    display: none !important;
  }
  .hide-width-lte-md{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lte-md{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lte-md{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lte-md{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 437px) {
  .hide-lt-xxs, .hide-below-xxs, .hidden-below-xxs, .hidden-lt-xxs {
    display: none !important;
  }
  .hide-width-lt-xxs, .hide-width-below-xxs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lt-xxs, .hide-height-below-xxs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lt-xxs, .hide-max-width-below-xxs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lt-xxs, .hide-max-height-below-xxs{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (max-width: 769px) {
  .hide-lte-xs, .hidden-lte-xs{
    display: none !important;
  }
  .hide-width-lte-xs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lte-xs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lte-xs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lte-xs{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 767px) {
  .hide-lt-xs, .hide-below-xs, .hidden-below-xs, .hidden-lt-xs {
    display: none !important;
  }
  .hide-width-lt-xs, .hide-width-below-xs{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lt-xs, .hide-height-below-xs{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lt-xs, .hide-max-width-below-xs{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lt-xs, .hide-max-height-below-xs{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (max-width: 577px) {
  .hide-lte-smx, .hidden-lte-smx{
    display: none !important;
  }
  .hide-width-lte-smx{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lte-smx{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lte-smx{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lte-smx{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 575px) {
  .hide-lt-smx, .hide-below-smx, .hidden-below-smx, .hidden-lt-smx {
    display: none !important;
  }
  .hide-width-lt-smx, .hide-width-below-smx{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lt-smx, .hide-height-below-smx{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lt-smx, .hide-max-width-below-smx{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lt-smx, .hide-max-height-below-smx{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (max-width: 993px) {
  .hide-lte-sm, .hidden-lte-sm{
    display: none !important;
  }
  .hide-width-lte-sm{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lte-sm{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lte-sm{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lte-sm{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 991px) {
  .hide-lt-sm, .hide-below-sm, .hidden-below-sm, .hidden-lt-sm{
    display: none !important;
  }
  .hide-width-lt-sm, .hide-width-below-sm{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lt-sm, .hide-height-below-sm{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lt-sm, .hide-max-width-below-sm{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lt-sm, .hide-max-height-below-sm{
    max-height:0 !important;overflow:hidden !important;
  }
}

@media (max-width: 1201px) {
  .hide-lte-md, .hidden-lte-md{
    display: none !important;
  }
  .hide-width-lte-md{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lte-md{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lte-md{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lte-md{
    max-height:0 !important;overflow:hidden !important;
  }
}
@media (max-width: 1199px) {
  .hide-lt-md, .hide-below-md, .hidden-below-md, .hidden-lt-md{
    display: none !important;
  }
  .hide-width-lt-md, .hide-width-below-md{
    width:0 !important;overflow:hidden !important;
  }
  .hide-height-lt-md, .hide-height-below-md{
    height:0 !important;overflow:hidden !important;
  }
  .hide-max-width-lt-md, .hide-max-width-below-md{
    max-width:0 !important;overflow:hidden !important;
  }
  .hide-max-height-lt-md, .hide-max-height-below-md{
    max-height:0 !important;overflow:hidden !important;
  }
}
```

> Compiled versions, .css files, can be found in ack-cssboot/dist/
