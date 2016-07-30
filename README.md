# ack-css-boot
A base set of short-hand css helper classes. Includes available classes that are commonly used for styling buttons, form inputs, and such.

Many commonly used short-hand classes, that are found in [Ionic](https://www.npmjs.com/package/ionic) and [Bootstrap](https://www.npmjs.com/package/bootstrap-css), can be found here.

> scss/ack-css-boot.scss

```
.font-arial {font-family:Arial}
.font-times {font-family:Times New Roman}
.font-helvetica {font-family:Helvetica}

.text-overflow {text-overflow:ellipsis;white-space:nowrap;overflow:hidden}

.valign,.valign-top,.vert-align-top {vertical-align:top}
.valign-middle,.valign-center,.vert-align-middle {vertical-align:middle}
.valign-bottom,.vert-align-bottom {vertical-align:bottom}

.nowrap {white-space:nowrap}

a,.cursor-pointer {cursor:pointer}

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

.clear,.clear-both,.clear-fix {clear:both}

.pos-absolute,.pos-abs {position:absolute}
.pos-relative,.pos-rel {position:relative}
.pos-fixed,.pos-fix {position:fixed}

.z-index-1 {z-index:1}
.z-index-10 {z-index:10}
.top-0 {top:0}
.right-0 {right:0}
.bottom-0 {bottom:0}
.left-0 {left:0}

.inline-block, .display-inline-block {display:inline-block}
.block, .display-block {display:block}

.flex, .display-flex {display:flex}
.flex-1 {flex:1 1 10em}
.flex-2 {flex:2 2 20em}
.flex-3 {flex:3 3 45em}
.flex-4 {flex:4 4 60em}
.flex-5 {flex:5 5 75em}
.flex-6 {flex:6 6 90em}
.flex-flow-inline, .flex-wrap {
  flex-flow:row wrap;
  flex-wrap:wrap;flex-direction:row;/*required for safari*/
}

.justify-left {justify-content:flex-start}
.justify-center {justify-content:center}
.justify-evenly, .justify-space-between {justify-content:space-between}
.justify-center-evenly, .justify-space-around {justify-content:space-around}
.justify-right {justify-content:flex-end}

.align-center {align-items:center}
.align-bottom,.align-end {align-items:flex-end}
.align-fill,.align-stretch {align-items:stretch}
.align-baseline {align-items:baseline}


.opacity-90 {opacity: 0.9}
.opacity-80 {opacity: 0.8}
.opacity-75 {opacity: 0.75}
.opacity-70 {opacity: 0.7}
.opacity-60 {opacity: 0.6}
.opacity-50,.opacity-half {opacity: 0.5}
.opacity-40 {opacity: 0.4}
.opacity-30 {opacity: 0.3}
.opacity-25,.opacity-third {opacity: 0.25}
.opacity-20 {opacity: 0.2}
.opacity-10 {opacity: 0.1}

.width-full,.full-width {width:100%}
.width-half,.half-width {width:50%}

.height-full {height:100%}
.height-half {width:50%}

.margin-0 {margin:0}
.margin-xxs {margin:0.2em}
.margin-xs {margin:0.4em}
.margin-sm {margin:0.6em}
.margin {margin:0.8em}
.margin-md {margin:1em}
.margin-lg {margin:1.5em}

.margin-v-0 {margin-top:0;margin-bottom:0}
.margin-v-xxs {margin-top:0.2em;margin-bottom:0.2em}
.margin-v-xs {margin-top:0.4em;margin-bottom:0.4em}
.margin-v-sm {margin-top:0.6em;margin-bottom:0.6em}
.margin-v {margin-top:0.8em;margin-bottom:0.8em}
.margin-v-md {margin-top:1em;margin-bottom:1em}
.margin-v-lg {margin-top:1.5em;margin-bottom:1.5em}

.margin-h-0 {margin-left:0;margin-right:0}
.margin-h-xxs {margin-left:0.2em;margin-right:0.2em}
.margin-h-xs {margin-left:0.4em;margin-right:0.4em}
.margin-h-sm {margin-left:0.6em;margin-right:0.6em}
.margin-h {margin-left:0.8em;margin-right:0.8em}
.margin-h-md {margin-left:1em;margin-right:1em}
.margin-h-lg {margin-left:1.5em;margin-right:1.5em}

.margin-top-0 {margin-top:0}
.margin-top-xxs {margin-top:0.2em}
.margin-top-xs {margin-top:0.4em}
.margin-top-sm {margin-top:0.6em}
.margin-top {margin-top:0.8em}
.margin-top-md {margin-top:1em}
.margin-top-lg {margin-top:1.5em}

.margin-bottom-0 {margin-bottom:0}
.margin-bottom-xxs {margin-bottom:0.2em}
.margin-bottom-xs {margin-bottom:0.4em}
.margin-bottom-sm {margin-bottom:0.6em}
.margin-bottom {margin-bottom:0.8em}
.margin-bottom-md {margin-bottom:1em}
.margin-bottom-lg {margin-bottom:1.5em}

.margin-left-0 {margin-left:0}
.margin-left-xxs {margin-left:0.2em}
.margin-left-xs {margin-left:0.4em}
.margin-left-sm {margin-left:0.6em}
.margin-left {margin-left:0.8em}
.margin-left-md {margin-left:1em}
.margin-left-lg {margin-left:1.5em}

.margin-right-0 {margin-right:0}
.margin-right-xxs {margin-right:0.2em}
.margin-right-xs {margin-right:0.4em}
.margin-right-sm {margin-right:0.6em}
.margin-right {margin-right:0.8em}
.margin-right-md {margin-right:1em}
.margin-right-lg {margin-right:1.5em}

.pad-0 {padding:0}
.pad-xxs {padding:0.2em}
.pad-xs {padding:0.4em}
.pad-sm {padding:0.6em}
.pad {padding:0.8em}
.pad-md {padding:1em}
.pad-lg {padding:1.5em}

.pad-v-0 {padding-top:0;padding-bottom:0}
.pad-v-xxs {padding-top:0.2em;padding-bottom:0.2em}
.pad-v-xs {padding-top:0.4em;padding-bottom:0.4em}
.pad-v-sm {padding-top:0.6em;padding-bottom:0.6em}
.pad-v {padding-top:0.8em;padding-bottom:0.8em}
.pad-v-md {padding-top:1em;padding-bottom:1em}
.pad-v-lg {padding-top:1.5em;padding-bottom:1.5em}

.pad-h-0 {padding-left:0;padding-right:0}
.pad-h-xxs {padding-left:0.2em;padding-right:0.2em}
.pad-h-xs {padding-left:0.4em;padding-right:0.4em}
.pad-h-sm {padding-left:0.6em;padding-right:0.6em}
.pad-h {padding-left:0.8em;padding-right:0.8em}
.pad-h-md {padding-left:1em;padding-right:1em}
.pad-h-lg {padding-left:1.5em;padding-right:1.5em}

.pad-top-0 {padding-top:0}
.pad-top-xxs {padding-top:0.2em}
.pad-top-xs {padding-top:0.4em}
.pad-top-sm {padding-top:0.6em}
.pad-top {padding-top:0.8em}
.pad-top-md {padding-top:1em}
.pad-top-lg {padding-top:1.5em}

.pad-bottom-0 {padding-bottom:0}
.pad-bottom-xxs {padding-bottom:0.2em}
.pad-bottom-xs {padding-bottom:0.4em}
.pad-bottom-sm {padding-bottom:0.6em}
.pad-bottom {padding-bottom:0.8em}
.pad-bottom-md {padding-bottom:1em}
.pad-bottom-lg {padding-bottom:1.5em}

.pad-left-0 {padding-left:0}
.pad-left-xxs {padding-left:0.2em}
.pad-left-xs {padding-left:0.4em}
.pad-left-sm {padding-left:0.6em}
.pad-left {padding-left:0.8em}
.pad-left-md {padding-left:1em}
.pad-left-lg {padding-left:1.5em}

.pad-right-0 {padding-right:0}
.pad-right-xxs {padding-right:0.2em}
.pad-right-xs {padding-right:0.4em}
.pad-right-sm {padding-right:0.6em}
.pad-right {padding-right:0.8em}
.pad-right-md {padding-right:1em}
.pad-right-lg {padding-right:1.5em}


.bg-royal {background-color:#ab57ff}
.bg-primary {background-color:#337ab7}
.bg-success {background-color:#dff0d8}
.bg-info {background-color:#d9edf7}
.bg-warning {background-color:#fcf8e3}
.bg-danger {background-color:#f2dede}
.bg-white {background-color:white}
.bg-black {background-color:black}
.bg-grey {background-color:#777}
.bg-grey-xs {background-color:#999}
.bg-grey-xxs {background-color:#BBB}

.float-right, .pull-right {float:right}
.float-left, .pull-left {float:left}

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

.border-radius-0 {border-radius:0}
.border-radius-half {border-radius:50%}

.line-height-0 {line-height:0}
.line-height-half {line-height:50%}
.line-height-third {line-height:33.3%}
.line-height-quarter {line-height:25%}
.line-height-2x {line-height:150%}
.line-height-3x {line-height:200%}


.form-group.has-error label:first-child {
  color:#d43f3a;
}

.form-group.has-error input,
.form-group.has-error select,
.form-group.has-error textarea {
  border:1px solid #d43f3a;
}
```