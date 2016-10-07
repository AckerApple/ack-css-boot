# ack-css-boot
A base set of short-hand css helper classes. Includes available classes that are commonly used for styling buttons, form inputs, and such.

Many commonly used short-hand classes, that are found in [Ionic](https://www.npmjs.com/package/ionic) and [Bootstrap](https://www.npmjs.com/package/bootstrap-css), can be found here.

### Table of Contents
- [Usage and Examples](#usage-and-examples)
- [Primary Style File](#primary-style-file)
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

> NOTE: ack-css-boot makes every attempt to avoid using the !important declaration. It is highly advised that the ack-css-boot.css file, be the LAST stylesheet file loaded in order to have short-hand css rules override other stylesheet rules.


## Primary Style File

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
.no-underline, .text-decoration-none {text-decoration:none}
.italic, .text-italic {font-style: italic}

.strong, .bold, .text-bold, .font-bold, .font-weight-bold {font-weight:bold}
.font-bolder, .font-weight-bolder {font-weight:bolder}
.font-normal, .font-weight-normal {font-weight:normal}
.font-lighter, .font-weight-lighter {font-weight:lighter}
.font-100, .font-weight-100 {font-weight:100}
.font-200, .font-weight-200 {font-weight:200}
.font-300, .font-weight-300 {font-weight:300}
.font-400, .font-weight-400 {font-weight:400}
.font-500, .font-weight-500 {font-weight:500}
.font-600, .font-weight-600 {font-weight:600}
.font-700, .font-weight-700 {font-weight:700}
.font-800, .font-weight-800 {font-weight:800}
.font-900, .font-weight-900 {font-weight:900}

.text-left {text-align:left}
.text-right {text-align:right}
.text-center {text-align:center}

.text-uppercase {text-transform: uppercase}
.text-lowercase {text-transform: lowercase}
.text-capitalize {text-transform: capitalize}


.text-9x {font-size:260%}
.text-8x {font-size:230%}
.text-7x {font-size:200%}
.text-6x {font-size:185%}
.text-5x {font-size:160%}
.text-4x {font-size:145%}
.text-lg, .text-3x {font-size:130%}
.text-md, .text-2x {font-size:115%}
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

.flex1 {flex:1 1 10em}
.flex2 {flex:2 2 20em}
.flex3 {flex:3 3 30em}
.flex4 {flex:4 4 40em}
.flex5 {flex:5 5 50em}
.flex6 {flex:6 6 60em}

.flex-grow-1,.flex-1 {flex-grow:1}
.flex-grow-2,.flex-2 {flex-grow:2}
.flex-grow-3,.flex-3 {flex-grow:3}
.flex-grow-4,.flex-4 {flex-grow:4}
.flex-grow-5,.flex-5 {flex-grow:5}
.flex-grow-6,.flex-6 {flex-grow:6}

.flex-wrap {flex-wrap:wrap;@extend .flex}

.flex-stack, .flex-stacked, .flex-column, .flex-columns, .flex-direction-column
{flex-direction: column;@extend .flex}

.flex-stack-reverse, .flex-column-reverse, .flex-columns-reverse, .flex-direction-column-reverse
{flex-direction: column-reverse;@extend .flex}

.flex-inline, .flex-row, .flex-rows, .flex-direction-row
{flex-direction: row;@extend .flex}

.flex-row-wrap, .flex-wrap-rows, .flex-wrap-inline, .flex-flow-inline
{flex-wrap:wrap;flex-direction:row;@extend .flex}

.flex-column-wrap, .flex-wrap-columns, .flex-wrap-stack, .flex-wrap-stacked, .flex-flow-stack, .flex-flow-stacked
{flex-wrap:wrap;flex-direction:column;@extend .flex}

.justify-left {justify-content:flex-start}
.flex-left {@extend .flex, .justify-left}

.justify-center {justify-content:center}
.flex-center {@extend .flex, .justify-center}

.justify-right {justify-content:flex-end}
.flex-right {@extend .flex, .justify-right}

.justify-apart, .justify-space-between {justify-content:space-between}
.flex-apart, .flex-space-between {@extend .flex, .justify-apart}

.justify-space-around {justify-content:space-around}
.flex-evenly, .flex-space-around {@extend .flex, .justify-space-around}

.flex-valign, .flex-top, .flex-valign-top {align-items:flex-start;@extend .flex}

.align-center {align-items:center}
.flex-valign-center, .flex-valign-middle {@extend .flex, .align-center}

.align-bottom,.align-end {align-items:flex-end}
.flex-valign-bottom {@extend .flex, .align-bottom}

.align-fill, .align-stretch {align-items:stretch}
.flex-fill {@extend .flex, .align-fill}

.align-baseline {align-items:baseline}
.flex-baseline {@extend .flex, .align-baseline}


.flex-stack.flex-center, .flex-stacked.flex-center, .flex-column.flex-center, .flex-columns.flex-center, .flex-direction-column.flex-center,
.flex-stack-reverse.flex-center, .flex-column-reverse.flex-center, .flex-columns-reverse.flex-center, .flex-direction-column-reverse.flex-center
{align-items:center}
.flex-stack.flex-left, .flex-stacked.flex-left, .flex-column.flex-left, .flex-columns.flex-left, .flex-direction-column.flex-left,
.flex-stack-reverse.flex-left, .flex-column-reverse.flex-left, .flex-columns-reverse.flex-left, .flex-direction-column-reverse.flex-left
{align-items:flex-start}
.flex-stack.flex-right, .flex-stacked.flex-right, .flex-column.flex-right, .flex-columns.flex-right, .flex-direction-column.flex-right,
.flex-stack-reverse.flex-right, .flex-column-reverse.flex-right, .flex-columns-reverse.flex-right, .flex-direction-column-reverse.flex-right
{align-items:flex-end}
```


## ack-color-boot

> scss/ack-color-boot.scss

```
$bg-primary:#337ab7 !default;
$bg-success:#dff0d8 !default;
$bg-info:#d9edf7 !default;
$bg-warning:#fcf8e3 !default;
$bg-danger:#f2dede !default;
$bg-grey:#777 !default;
$bg-grey-2x:#999 !default;
$bg-grey-3x:#BBB !default;
$bg-grey-4x:#CCC !default;
$bg-grey-5x:#DDD !default;
$bg-grey-6x:#EEE !default;
$bg-stable:#f8f8f8 !default;
$bg-positive:#387ef5 !default;
$bg-calm:#11c1f3 !default;
$bg-balanced:#33cd5f !default;
$bg-energized:#ffc900 !default;
$bg-assertive:#ef473a !default;
$bg-royal:#886aea !default;
$bg-dark:#444444 !default;


.text-positive {color:#0c60ee}
.text-calm {color:#0a9dc7}
.text-balanced {color:#28a54c}
.text-energized {color:#e6b500}
.text-assertive {color:#e42112}
.text-royal {color:#6b46e5}
.text-dark {color:#111111}

.text-primary {color:#337ab7}
.text-success {color:#3c763d}
.text-info {color:#31708f}
.text-warning {color:#8a6d3b}
.text-danger {color:#a94442}

.text-grey-lg, .text-muted-lg {color:#333}
.text-grey-md, .text-muted-md {color:#555}
.text-grey, .text-muted {color:#777}
.text-grey-2x, .text-grey-sm, .text-muted-sm, .text-muted-2x {color:#999}
.text-grey-3x, .text-grey-xs, .text-muted-xs, .text-muted-3x {color:#BBB}
.text-grey-4x, .text-grey-xxs, .text-muted-xxs, .text-muted-4x {color:#CCC}
.text-grey-5x {color:#DDD}
.text-grey-6x {color:#EEE}

.text-green,.font-green {color: #060}
.text-orange,.font-orange {color: #C60}
.text-red,.font-red {color:#900}
.text-blue,.font-blue {color: #009}
.text-purple,.font-purple {color: #60C}
.text-black,.font-black {color: #000}
.text-white,.font-white {color: #FFF}

.bg-white,.bg-lite {background-color:white}
.bg-black {background-color:black}
.bg-primary {background-color:$bg-primary}
.bg-success {background-color:$bg-success}
.bg-info {background-color:$bg-info}
.bg-warning {background-color:$bg-warning}
.bg-danger {background-color:$bg-danger}
.bg-grey {background-color:$bg-grey}
.bg-grey-xs,.bg-grey-2x {background-color:$bg-grey-2x}
.bg-grey-xxs,.bg-grey-3x {background-color:$bg-grey-3x}
.bg-grey-4x {background-color:$bg-grey-4x}
.bg-grey-5x {background-color:$bg-grey-5x}
.bg-grey-6x {background-color:$bg-grey-6x}
.bg-stable {background-color:$bg-stable}
.bg-positive {background-color:$bg-positive}
.bg-calm {background-color:$bg-calm}
.bg-balanced {background-color:$bg-balanced}
.bg-energized {background-color:$bg-energized}
.bg-assertive {background-color:$bg-assertive}
.bg-royal {background-color:$bg-royal}
.bg-dark {background-color:$bg-dark}

.border-grey {border-color:#666}
.border-grey-xs, .border-grey-2x {border-color:#888}
.border-grey-xxs, .border-grey-3x {border-color:#AAA}
.border-grey-4x {border-color:#BBB}
.border-grey-5x {border-color:#CCC}
.border-grey-6x {border-color:#DDD}
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
.border-stable {border-color:#e7e7e7}
.border-1-positive {border-color:#0c60ee}
.border-1-calm {border-color:#0a9dc7}
.border-1-balanced {border-color:#28a54c}
.border-1-energized {border-color:#e6b500}
.border-1-assertive {border-color:#e42112}
.border-1-royal {border-color:#6b46e5}
.border-1-dark {border-color:#111111}
.border-1-danger {border-color:#d43f3a}
.border-1-warning {border-color:#eea236}
.border-1-info {border-color:#46b8da}
.border-1-success {border-color:#4cae4c}
.border-1-primary {border-color:#2e6da4}


.hover-text-shadow-grey-blur:hover{
  text-shadow:0 0 4px #777
}
.hover-text-shadow-white-blur:hover{
  text-shadow:0 0 4px #FFF
}

.table-striped > tbody > tr:nth-of-type(odd) {background-color: #f1f1f1}
.table-striped-primary > tbody > tr:nth-of-type(odd)
{background-color:$bg-primary}
.table-striped-success > tbody > tr:nth-of-type(odd)
{background-color:$bg-success}
.table-striped-info > tbody > tr:nth-of-type(odd)
{background-color:$bg-info}
.table-striped-warning > tbody > tr:nth-of-type(odd)
{background-color:$bg-warning}
.table-striped-danger > tbody > tr:nth-of-type(odd)
{background-color:$bg-danger}
.table-striped-grey > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey}
.table-striped-grey-2x > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey-2x}
.table-striped-grey-3x > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey-3x}
.table-striped-grey-4x > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey-4x}
.table-striped-grey-5x > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey-5x}
.table-striped-grey-6x > tbody > tr:nth-of-type(odd)
{background-color:$bg-grey-6x}
.table-striped-stable > tbody > tr:nth-of-type(odd)
{background-color:$bg-stable}
.table-striped-positive > tbody > tr:nth-of-type(odd)
{background-color:$bg-positive}
.table-striped-calm > tbody > tr:nth-of-type(odd)
{background-color:$bg-calm}
.table-striped-balanced > tbody > tr:nth-of-type(odd)
{background-color:$bg-balanced}
.table-striped-energized > tbody > tr:nth-of-type(odd)
{background-color:$bg-energized}
.table-striped-assertive > tbody > tr:nth-of-type(odd)
{background-color:$bg-assertive}
.table-striped-royal > tbody > tr:nth-of-type(odd)
{background-color:$bg-royal}
.table-striped-dark > tbody > tr:nth-of-type(odd)
{background-color:$bg-dark}

table[class*="table-striped-"] > tbody > tr.bg-primary
{background-color:$bg-primary}
table[class*="table-striped-"] > tbody > tr.bg-success
{background-color:$bg-success}
table[class*="table-striped-"] > tbody > tr.bg-info
{background-color:$bg-info}
table[class*="table-striped-"] > tbody > tr.bg-warning
{background-color:$bg-warning}
table[class*="table-striped-"] > tbody > tr.bg-danger
{background-color:$bg-danger}
table[class*="table-striped-"] > tbody > tr.bg-grey
{background-color:$bg-grey}
table[class*="table-striped-"] > tbody > tr.grey-2x
{background-color:$bg-grey-2x}
table[class*="table-striped-"] > tbody > tr.grey-3x
{background-color:$bg-grey-3x}
table[class*="table-striped-"] > tbody > tr.grey-4x
{background-color:$bg-grey-4x}
table[class*="table-striped-"] > tbody > tr.grey-5x
{background-color:$bg-grey-5x}
table[class*="table-striped-"] > tbody > tr.grey-6x
{background-color:$bg-grey-6x}
[class*="table-striped-"] > tbody > tr.bg-stable
{background-color:$bg-stable}
[class*="table-striped-"] > tbody > tr.bg-positive
{background-color:$bg-positive}
[class*="table-striped-"] > tbody > tr.bg-calm
{background-color:$bg-calm}
[class*="table-striped-"] > tbody > tr.bg-balanced
{background-color:$bg-balanced}
[class*="table-striped-"] > tbody > tr.bg-energized
{background-color:$bg-energized}
[class*="table-striped-"] > tbody > tr.bg-assertive
{background-color:$bg-assertive}
[class*="table-striped-"] > tbody > tr.bg-royal
{background-color:$bg-royal}
[class*="table-striped-"] > tbody > tr.bg-dark
{background-color:$bg-dark}

.table-hover > tbody > tr:hover {background-color: #f5f5f5}
.hover-bg-primary:hover, .table-hover-primary > tbody > tr:hover,
[class*="table-striped-"].table-hover-primary > tbody > tr:hover
{background-color:$bg-primary}
.hover-bg-success:hover, .table-hover-success > tbody > tr:hover,
[class*="table-striped-"].table-hover-success > tbody > tr:hover
{background-color:$bg-success}
.hover-bg-info:hover, .table-hover-info > tbody > tr:hover,
[class*="table-striped-"].table-hover-info > tbody > tr:hover
{background-color:$bg-info}
.hover-bg-warning:hover, .table-hover-warning > tbody > tr:hover,
[class*="table-striped-"].table-hover-warning > tbody > tr:hover
{background-color:$bg-warning}
.hover-bg-danger:hover, .table-hover-danger > tbody > tr:hover,
[class*="table-striped-"].table-hover-danger > tbody > tr:hover
{background-color:$bg-danger}
.hover-bg-grey:hover, .table-hover-grey > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey > tbody > tr:hover
{background-color:$bg-grey}
.hover-bg-grey-2x:hover, .table-hover-grey-2x > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey-2x > tbody > tr:hover
{background-color:$bg-grey-2x}
.hover-bg-grey-3x:hover, .table-hover-grey-3x > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey-3x > tbody > tr:hover
{background-color:$bg-grey-3x}
.hover-bg-grey-4x:hover, .table-hover-grey-4x > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey-4x > tbody > tr:hover
{background-color:$bg-grey-4x}
.hover-bg-grey-5x:hover, .table-hover-grey-5x > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey-5x > tbody > tr:hover
{background-color:$bg-grey-5x}
.hover-bg-grey-6x:hover, .table-hover-grey-6x > tbody > tr:hover,
[class*="table-striped-"].table-hover-grey-6x > tbody > tr:hover
{background-color:$bg-grey-6x}
.hover-bg-stable:hover, .table-hover-stable > tbody > tr:hover,
[class*="table-striped-"].table-hover-stable > tbody > tr:hover
{background-color:$bg-stable}
.hover-bg-positive:hover, .table-hover-positive > tbody > tr:hover,
[class*="table-striped-"].table-hover-positive > tbody > tr:hover
{background-color:$bg-positive}
.hover-bg-calm:hover, .table-hover-calm > tbody > tr:hover,
[class*="table-striped-"].table-hover-calm > tbody > tr:hover
{background-color:$bg-calm}
.hover-bg-balanced:hover, .table-hover-balanced > tbody > tr:hover,
[class*="table-striped-"].table-hover-balanced > tbody > tr:hover
{background-color:$bg-balanced}
.hover-bg-energized:hover, .table-hover-energized > tbody > tr:hover,
[class*="table-striped-"].table-hover-energized > tbody > tr:hover
{background-color:$bg-energized}
.hover-bg-assertive:hover, .table-hover-assertive > tbody > tr:hover,
[class*="table-striped-"].table-hover-assertive > tbody > tr:hover
{background-color:$bg-assertive}
.hover-bg-royal:hover, .table-hover-royal > tbody > tr:hover,
[class*="table-striped-"].table-hover-royal > tbody > tr:hover
{background-color:$bg-royal}
.hover-bg-dark:hover, .table-hover-dark > tbody > tr:hover,
[class*="table-striped-"].table-hover-dark > tbody > tr:hover
{background-color:$bg-dark}


.table-lines-primary {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-primary}}}
  > thead > tr > th {@extend .border-primary}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-primary}}}
  > tbody + tbody {@extend .border-primary}
}
.table-lines-success {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-success}}}
  > thead > tr > th {@extend .border-success}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-success}}}
  > tbody + tbody {@extend .border-success}
}
.table-lines-info {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-info}}}
  > thead > tr > th {@extend .border-info}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-info}}}
  > tbody + tbody {@extend .border-info}
}
.table-lines-warning {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-warning}}}
  > thead > tr > th {@extend .border-warning}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-warning}}}
  > tbody + tbody {@extend .border-warning}
}
.table-lines-danger {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-danger}}}
  > thead > tr > th {@extend .border-danger}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-danger}}}
  > tbody + tbody {@extend .border-danger}
}
.table-lines-grey {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey}}}
  > thead > tr > th {@extend .border-grey}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey}}}
  > tbody + tbody {@extend .border-grey}
}
.table-lines-grey-2x {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey-2x}}}
  > thead > tr > th {@extend .border-grey-2x}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey-2x}}}
  > tbody + tbody {@extend .border-grey-2x}
}
.table-lines-grey-3x {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey-3x}}}
  > thead > tr > th {@extend .border-grey-3x}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey-3x}}}
  > tbody + tbody {@extend .border-grey-3x}
}
.table-lines-grey-4x {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey-4x}}}
  > thead > tr > th {@extend .border-grey-4x}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey-4x}}}
  > tbody + tbody {@extend .border-grey-4x}
}
.table-lines-grey-5x {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey-5x}}}
  > thead > tr > th {@extend .border-grey-5x}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey-5x}}}
  > tbody + tbody {@extend .border-grey-5x}
}
.table-lines-grey-6x {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-grey-6x}}}
  > thead > tr > th {@extend .border-grey-6x}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-grey-6x}}}
  > tbody + tbody {@extend .border-grey-6x}
}
.table-lines-stable {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-stable}}}
  > thead > tr > th {@extend .border-stable}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-stable}}}
  > tbody + tbody {@extend .border-stable}
}
.table-lines-positive {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-positive}}}
  > thead > tr > th {@extend .border-positive}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-positive}}}
  > tbody + tbody {@extend .border-positive}
}
.table-lines-calm {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-calm}}}
  > thead > tr > th {@extend .border-calm}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-calm}}}
  > tbody + tbody {@extend .border-calm}
}
.table-lines-balanced {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-balanced}}}
  > thead > tr > th {@extend .border-balanced}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-balanced}}}
  > tbody + tbody {@extend .border-balanced}
}
.table-lines-energized {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-energized}}}
  > thead > tr > th {@extend .border-energized}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-energized}}}
  > tbody + tbody {@extend .border-energized}
}
.table-lines-assertive {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-assertive}}}
  > thead > tr > th {@extend .border-assertive}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-assertive}}}
  > tbody + tbody {@extend .border-assertive}
}
.table-lines-royal {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-royal}}}
  > thead > tr > th {@extend .border-royal}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-royal}}}
  > tbody + tbody {@extend .border-royal}
}
.table-lines-dark {
  > thead,> tbody,> tfoot {> tr {> th, > td {@extend .border-dark}}}
  > thead > tr > th {@extend .border-dark}
  > caption + thead,> colgroup + thead,> thead:first-child {> tr:first-child {> th, > td {@extend .border-dark}}}
  > tbody + tbody {@extend .border-dark}
}
```


## ack-block-boot

> scss/ack-block-boot.scss

```
$em-xxs: 0.2em !default;
$em-xs: 0.4em !default;
$em-sm: 0.6em !default;
$em: 0.8em !default;
$em-md: 1em !default;
$em-lg: 1.5em !default;
$em-4x: 2em !default;

.no-a-style {color:inherit;text-decoration:inherit}

.cursor-pointer {cursor:pointer}

.overflow-hidden {overflow:hidden}
.overflow, .overflow-auto {overflow:auto}
.overflow-y-auto {overflow-y:auto}
.overflow-y-hidden {overflow-y:hidden}
.overflow-x-auto {overflow-x:auto}
.overflow-x-hidden {overflow-x:hidden}


.hide,.hidden,.display-none {display:none}
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
.opacity-0 {opacity: 0}

.radius-0, .border-radius-0 {border-radius:0}
.radius-3, .border-radius-3 {border-radius:3px}
.radius-4, .border-radius-4 {border-radius:4px}
.radius-5, .border-radius-5 {border-radius:5px}
.radius-6, .border-radius-6 {border-radius:6px}
.radius-7, .border-radius-7 {border-radius:7px}
.radius-8, .border-radius-8 {border-radius:8px}
.radius-9, .border-radius-9 {border-radius:9px}
.radius-10, .border-radius-10 {border-radius:10px}
.radius-15, .border-radius-15 {border-radius:15px}
.radius-20, .border-radius-20 {border-radius:20px}
.radius-25, .border-radius-25 {border-radius:25px}
.radius-third, .border-radius-third {border-radius:33.3%}
.radius-quarter, .border-radius-quarter {border-radius:25%}
.radius-half, .border-radius-half {border-radius:50%}
.radius-left-0 {border-top-left-radius:0;border-bottom-left-radius:0}
.radius-right-0 {border-top-right-radius:0;border-bottom-right-radius:0}
.radius-top-0 {border-top-left-radius:0;border-top-right-radius:0}
.radius-bottom-0 {border-bottom-right-radius:0;border-bottom-left-radius:0}

.border-spacing-0 {border-spacing:0}
.border-collapse {border-collapse:collapse}
.border-separate, .border-collapse-seperate {border-collapse:separate}
.border,.border-1 {border-width:1px;border-style:solid;border-color:black}
.border-top, .border-top-1 {border-top-width:1px;border-top-style:solid;border-color:black}
.border-right, .border-right-1 {border-right-width:1px;border-right-style:solid;border-color:black}
.border-left, .border-left-1 {border-left-width:1px;border-left-style:solid;border-color:black}
.border-bottom, .border-bottom-1 {border-bottom-width:1px;border-bottom-style:solid;border-color:black}
.border-2 {border-width:2px;border-style:solid;border-color:black}
.border-3 {border-width:3px;border-style:solid;border-color:black}
.border-4 {border-width:4px;border-style:solid;border-color:black}
.border-5 {border-width:5px;border-style:solid;border-color:black}
.border-6 {border-width:6px;border-style:solid;border-color:black}
.border-7 {border-width:7px;border-style:solid;border-color:black}
.border-8 {border-width:8px;border-style:solid;border-color:black}
.border-top-2 {border-top-width:2px;border-top-style:solid;border-color:black}
.border-top-3 {border-top-width:3px;border-top-style:solid;border-color:black}
.border-top-4 {border-top-width:4px;border-top-style:solid;border-color:black}
.border-top-5 {border-top-width:5px;border-top-style:solid;border-color:black}
.border-top-6 {border-top-width:6px;border-top-style:solid;border-color:black}
.border-top-7 {border-top-width:7px;border-top-style:solid;border-color:black}
.border-top-8 {border-top-width:8px;border-top-style:solid;border-color:black}
.border-right-2 {border-right-width:2px;border-right-style:solid;border-color:black}
.border-right-3 {border-right-width:3px;border-right-style:solid;border-color:black}
.border-right-4 {border-right-width:4px;border-right-style:solid;border-color:black}
.border-right-5 {border-right-width:5px;border-right-style:solid;border-color:black}
.border-right-6 {border-right-width:6px;border-right-style:solid;border-color:black}
.border-right-7 {border-right-width:7px;border-right-style:solid;border-color:black}
.border-right-8 {border-right-width:8px;border-right-style:solid;border-color:black}
.border-bottom-2 {border-bottom-width:2px;border-bottom-style:solid;border-color:black}
.border-bottom-3 {border-bottom-width:3px;border-bottom-style:solid;border-color:black}
.border-bottom-4 {border-bottom-width:4px;border-bottom-style:solid;border-color:black}
.border-bottom-5 {border-bottom-width:5px;border-bottom-style:solid;border-color:black}
.border-bottom-6 {border-bottom-width:6px;border-bottom-style:solid;border-color:black}
.border-bottom-7 {border-bottom-width:7px;border-bottom-style:solid;border-color:black}
.border-bottom-8 {border-bottom-width:8px;border-bottom-style:solid;border-color:black}
.border-left-2 {border-left-width:2px;border-left-style:solid;border-color:black}
.border-left-3 {border-left-width:3px;border-left-style:solid;border-color:black}
.border-left-4 {border-left-width:4px;border-left-style:solid;border-color:black}
.border-left-5 {border-left-width:5px;border-left-style:solid;border-color:black}
.border-left-6 {border-left-width:6px;border-left-style:solid;border-color:black}
.border-left-7 {border-left-width:7px;border-left-style:solid;border-color:black}
.border-left-8 {border-left-width:8px;border-left-style:solid;border-color:black}


.border-1-positive,
.border-1-calm,
.border-1-balanced,
.border-1-energized,
.border-1-assertive,
.border-1-royal,
.border-1-dark,
.border-1-danger,
.border-1-warning,
.border-1-info,
.border-1-success,
.border-1-primary {border-width:1px;border-style:solid}

.border-solid {border-style:solid}
.border-dotted {border-style:dotted}
.border-dashed {border-style:dashed}

.border-top-solid {border-top-style:solid}
.border-top-dotted {border-top-style:dotted}
.border-top-dashed {border-top-style:dashed}

.border-right-solid {border-right-style:solid}
.border-right-dotted {border-right-style:dotted}
.border-right-dashed {border-right-style:dashed}

.border-bottom-solid {border-bottom-style:solid}
.border-bottom-dotted {border-bottom-style:dotted}
.border-bottom-dashed {border-bottom-style:dashed}

.border-left-solid {border-left-style:solid}
.border-left-dotted {border-left-style:dotted}
.border-left-dashed {border-left-style:dashed}

.border-0 {border:0}
.border-top-0 {border-top:0}
.border-right-0 {border-right:0}
.border-left-0 {border-left:0}
.border-bottom-0 {border-bottom:0}


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
.margin-2x, .margin-md {margin:$em-md}
.margin-3x, .margin-lg {margin:$em-lg}
.margin-4x {margin:$em-4x}

.margin-v-0 {margin-top:0;margin-bottom:0}
.margin-v-xxs {margin-top:$em-xxs;margin-bottom:$em-xxs}
.margin-v-xs {margin-top:$em-xs;margin-bottom:$em-xs}
.margin-v-sm {margin-top:$em-sm;margin-bottom:$em-sm}
.margin-v {margin-top:$em;margin-bottom:$em}
.margin-v-2x, .margin-v-md {margin-top:$em-md;margin-bottom:$em-md}
.margin-v-3x, .margin-v-lg {margin-top:$em-lg;margin-bottom:$em-lg}
.margin-v-4x {margin-top:$em-4x;margin-bottom:$em-4x}

.margin-h-0 {margin-left:0;margin-right:0}
.margin-h-xxs {margin-left:$em-xxs;margin-right:$em-xxs}
.margin-h-xs {margin-left:$em-xs;margin-right:$em-xs}
.margin-h-sm {margin-left:$em-sm;margin-right:$em-sm}
.margin-h {margin-left:$em;margin-right:$em}
.margin-h-2x, .margin-h-md {margin-left:$em-md;margin-right:$em-md}
.margin-h-3x, .margin-h-lg {margin-left:$em-lg;margin-right:$em-lg}
.margin-h-4x {margin-left:$em-4x;margin-right:$em-4x}

.margin-top-0 {margin-top:0}
.margin-top-xxs {margin-top:$em-xxs}
.margin-top-xs {margin-top:$em-xs}
.margin-top-sm {margin-top:$em-sm}
.margin-top {margin-top:$em}
.margin-top-2x, .margin-top-md {margin-top:$em-md}
.margin-top-3x, .margin-top-lg {margin-top:$em-lg}
.margin-top-4x, .margin-top-lg {margin-top:$em-4x}

.margin-bottom-0 {margin-bottom:0}
.margin-bottom-xxs {margin-bottom:$em-xxs}
.margin-bottom-xs {margin-bottom:$em-xs}
.margin-bottom-sm {margin-bottom:$em-sm}
.margin-bottom {margin-bottom:$em}
.margin-bottom-2x, .margin-bottom-md {margin-bottom:$em-md}
.margin-bottom-3x, .margin-bottom-lg {margin-bottom:$em-lg}
.margin-bottom-4x {margin-bottom:$em-4x}

.margin-left-0 {margin-left:0}
.margin-left-xxs {margin-left:$em-xxs}
.margin-left-xs {margin-left:$em-xs}
.margin-left-sm {margin-left:$em-sm}
.margin-left {margin-left:$em}
.margin-left-2x, .margin-left-md {margin-left:$em-md}
.margin-left-3x, .margin-left-lg {margin-left:$em-lg}
.margin-left-4x {margin-left:$em-4x}

.margin-right-0 {margin-right:0}
.margin-right-xxs {margin-right:$em-xxs}
.margin-right-xs {margin-right:$em-xs}
.margin-right-sm {margin-right:$em-sm}
.margin-right {margin-right:$em}
.margin-right-2x, .margin-right-md {margin-right:$em-md}
.margin-right-3x, .margin-right-lg {margin-right:$em-lg}
.margin-right-4x {margin-right:$em-4x}


.pad-0 {padding:0}
.pad-xxs {padding:$em-xxs}
.pad-xs {padding:$em-xs}
.pad-sm {padding:$em-sm}
.pad {padding:$em}
.pad-2x, .pad-md {padding:$em-md}
.pad-3x, .pad-lg {padding:$em-lg}
.pad-4x {padding:$em-4x}

.pad-v-0 {padding-top:0;padding-bottom:0}
.pad-v-xxs {padding-top:$em-xxs;padding-bottom:$em-xxs}
.pad-v-xs {padding-top:$em-xs;padding-bottom:$em-xs}
.pad-v-sm {padding-top:$em-sm;padding-bottom:$em-sm}
.pad-v {padding-top:$em;padding-bottom:$em}
.pad-v-2x, .pad-v-md {padding-top:$em-md;padding-bottom:$em-md}
.pad-v-3x, .pad-v-lg {padding-top:$em-lg;padding-bottom:$em-lg}
.pad-v-4x {padding-top:$em-4x;padding-bottom:$em-4x}

.pad-h-0 {padding-left:0;padding-right:0}
.pad-h-xxs {padding-left:$em-xxs;padding-right:$em-xxs}
.pad-h-xs {padding-left:$em-xs;padding-right:$em-xs}
.pad-h-sm {padding-left:$em-sm;padding-right:$em-sm}
.pad-h {padding-left:$em;padding-right:$em}
.pad-h-2x, .pad-h-md {padding-left:$em-md;padding-right:$em-md}
.pad-h-3x, .pad-h-lg {padding-left:$em-lg;padding-right:$em-lg}
.pad-h-4x {padding-left:$em-4x;padding-right:$em-4x}

.pad-top-0 {padding-top:0}
.pad-top-xxs {padding-top:$em-xxs}
.pad-top-xs {padding-top:$em-xs}
.pad-top-sm {padding-top:$em-sm}
.pad-top {padding-top:$em}
.pad-top-2x, .pad-top-md {padding-top:$em-md}
.pad-top-3x, .pad-top-lg {padding-top:$em-lg}
.pad-top-4x {padding-top:$em-4x}

.pad-bottom-0 {padding-bottom:0}
.pad-bottom-xxs {padding-bottom:$em-xxs}
.pad-bottom-xs {padding-bottom:$em-xs}
.pad-bottom-sm {padding-bottom:$em-sm}
.pad-bottom {padding-bottom:$em}
.pad-bottom-2x, .pad-bottom-md {padding-bottom:$em-md}
.pad-bottom-3x, .pad-bottom-lg {padding-bottom:$em-lg}
.pad-bottom-4x {padding-bottom:$em-4x}

.pad-left-0 {padding-left:0}
.pad-left-xxs {padding-left:$em-xxs}
.pad-left-xs {padding-left:$em-xs}
.pad-left-sm {padding-left:$em-sm}
.pad-left {padding-left:$em}
.pad-left-2x, .pad-left-md {padding-left:$em-md}
.pad-left-3x, .pad-left-lg {padding-left:$em-lg}
.pad-left-4x {padding-left:$em-4x}

.pad-right-0 {padding-right:0}
.pad-right-xxs {padding-right:$em-xxs}
.pad-right-xs {padding-right:$em-xs}
.pad-right-sm {padding-right:$em-sm}
.pad-right {padding-right:$em}
.pad-right-2x, .pad-right-md {padding-right:$em-md}
.pad-right-3x, .pad-right-lg {padding-right:$em-lg}
.pad-right-4x {padding-right:$em-4x}

.height-5 {height:5px}
.width-5 {width:5px}
.height-10 {height:10px}
.width-10 {width:10px}
.height-15 {height:15px}
.width-15 {width:15px}
.height-20 {height:20px}
.width-20 {width:20px}
.height-30 {height:30px}
.width-30 {width:30px}
.height-40 {height:40px}
.width-40 {width:40px}
.height-50 {height:50px}
.width-50 {width:50px}
.height-60 {height:60px}
.width-60 {width:60px}
.height-70 {height:70px}
.width-70 {width:70px}
.height-80 {height:80px}
.width-80 {width:80px}
.height-90 {height:90px}
.width-90 {width:90px}
.height-100 {height:100px}
.width-100 {width:100px}
.height-200 {height:200px}
.width-200 {width:200px}
.height-300 {height:300px}
.width-300 {width:300px}
.height-400 {height:400px}
.width-400 {width:400px}
.height-500 {height:500px}
.width-500 {width:500px}
.height-600 {height:600px}
.width-600 {width:600px}
.height-700 {height:700px}
.width-700 {width:700px}
.height-800 {height:800px}
.width-800 {width:800px}
.height-900 {height:900px}
.width-900 {width:900px}
.height-1000 {height:1000px}
.width-1000 {width:1000px}

.max-height {max-height:100%}
.max-width {max-width:100%}
.max-height-50 {max-height:50px}
.max-width-50 {max-width:50px}
.max-height-60 {max-height:60px}
.max-width-60 {max-width:60px}
.max-height-70 {max-height:70px}
.max-width-70 {max-width:70px}
.max-height-80 {max-height:80px}
.max-width-80 {max-width:80px}
.max-height-90 {max-height:90px}
.max-width-90 {max-width:90px}
.max-height-100 {max-height:100px}
.max-width-100 {max-width:100px}
.max-height-200 {max-height:200px}
.max-width-200 {max-width:200px}
.max-height-300 {max-height:300px}
.max-width-300 {max-width:300px}
.max-height-400 {max-height:400px}
.max-width-400 {max-width:400px}
.max-height-500 {max-height:500px}
.max-width-500 {max-width:500px}
.max-height-600 {max-height:600px}
.max-width-600 {max-width:600px}
.max-height-700 {max-height:700px}
.max-width-700 {max-width:700px}
.max-height-800 {max-height:800px}
.max-width-800 {max-width:800px}
.max-height-900 {max-height:900px}
.max-width-900 {max-width:900px}
.max-height-1000 {max-height:1000px}
.max-width-1000 {max-width:1000px}

.min-height {min-height:0}
.min-width {min-width:0}
.min-height-5 {min-height:5px}
.min-width-5 {min-width:5px}
.min-height-10 {min-height:10px}
.min-width-10 {min-width:10px}
.min-height-20 {min-height:20px}
.min-width-20 {min-width:20px}
.min-height-30 {min-height:30px}
.min-width-30 {min-width:30px}
.min-height-40 {min-height:40px}
.min-width-40 {min-width:40px}
.min-height-50 {min-height:50px}
.min-width-50 {min-width:50px}
.min-height-60 {min-height:60px}
.min-width-60 {min-width:60px}
.min-height-70 {min-height:70px}
.min-width-70 {min-width:70px}
.min-height-80 {min-height:80px}
.min-width-80 {min-width:80px}
.min-height-90 {min-height:90px}
.min-width-90 {min-width:90px}
.min-height-100 {min-height:100px}
.min-width-100 {min-width:100px}
.min-height-200 {min-height:200px}
.min-width-200 {min-width:200px}
.min-height-300 {min-height:300px}
.min-width-300 {min-width:300px}
.min-height-400 {min-height:400px}
.min-width-400 {min-width:400px}
.min-height-500 {min-height:500px}
.min-width-500 {min-width:500px}
.min-height-600 {min-height:600px}
.min-width-600 {min-width:600px}
.min-height-700 {min-height:700px}
.min-width-700 {min-width:700px}
.min-height-800 {min-height:800px}
.min-width-800 {min-width:800px}
.min-height-900 {min-height:900px}
.min-width-900 {min-width:900px}
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

.table-lines {
  > thead,
  > tbody,
  > tfoot {
    > tr {
      > th, > td {@extend .border-bottom;border-color:#DDD;}
    }
  }
  > thead > tr > th {@extend .border-bottom-2;border-color:#DDD;}
  > caption + thead,
  > colgroup + thead,
  > thead:first-child {
    > tr:first-child {
      > th, > td {@extend .border-top-0;border-color:#DDD;}
    }
  }
  > tbody + tbody {@extend .border-top-2;border-color:#DDD;}
}
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

## ack-overrides

> scss/ack-overrides.scss
```
a, button {cursor:pointer}
```

> Compiled versions, .css files, can be found in ack-cssboot/dist/
