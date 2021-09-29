# ack-css-boot - Change Log
All notable changes to this project will be documented here.


## [3.0.2] - 2021-09-02
- Moved active classes lower than hover classes to ensure they fire
- updated dev dependencies
- New width height vw/vh classes
- Removed .font-color use .text-color or .color-color (ex: .text-red .color-red)
- Added .color-name and simple text colors as .red, .blue, and so on... (added yellow)

## [2.1.1] - 2021-08-24
- added xxxs

## [2.1.0] - 2021-5-27
- Added mousedown aka :active classes

## [2.0.0] - 2021-5-5
- border-v and border-h treatments swapped
  - border-v used to add border to top and bottom
    - border-v stands for border-verticals
    - The borders now run vertically be specifying left and right borders
  - border-h used to add border to sides
    - border-h stands for border-horizontals
    - The borders now run horizontally be specifying top and bottom borders

## [1.2.63] - 2019-06-23
- added .underline-no-skip
- added .underline-under
- added width-2 height-2
- added width height docs
- added .rotate-45
- added .rotate-90
- added .rotate-135
- added .rotate-180

## [1.2.59] - 2019-05-14
- added .hyphens

## [1.2.58] - 2019-05-14
- added .text-justify

## [1.2.57] - 2019-04-26
- Added `.no-scroll-bars` definition of `scrollbar-width: none` for firefox

## [1.2.56] - 2019-04-12
- new .print-no-bg
- moved block, inline-block and such above flex classes to give flex priority
- added child-pad-smx
- added child-margin-smx
- added .touch-scroll
- All overflow auto classes has touch scroll to them

## [1.2.55] - 2018-12-03
- removed scroll bard for Edge

## [1.2.54] - 2018-11-01
- added .valign-text-top
- added .flex1-5 and child-flex1-5

## [1.2.52] - 2018-08-16
- added letter-spacing
  - .letter-spacing-xxs
  - .letter-spacing-smx
  - .letter-spacing-sm
  - .letter-spacing-2x
  - .letter-spacing-3x
  - .letter-spacing-4x

## [1.2.51] - 2018-08-16
- added stroke
  - .stroke
  - .stroke-1
  - .stroke-2
  - .stroke-3
  - .stroke-4
  - .stroke-5

## [1.2.49] - 2018-08-01
- Added
  - bg-grey-7x
  - more line-height values above 100
  - .bold-100 through .bold-900
  - .strong-100 through .strong-900
  - .child-pad-right-xxs
  - .child-flex1
  - .child-flex-1
  - .child-flex2
  - .child-flex-2

## [1.2.48] - 2018-04-12
- .child-last-block
- .child-last-height-full

## [1.2.47] - 2018-03-29
- Added 150 as a width height
- added child-width-* child-height-* classes
- code sample pre tag default no margin
- added more child-margin-* classes
- Added .hover-strong (.hover-bold already existed)

## [1.2.46] - 2018-01-29
- Added border-h classes
- Added border-v classes

## [1.2.42] - 2017-07-26
- added .flex-reverse

## [1.2.40] - 2017-06-11
### Added
- .child-radius classes

## [1.2.37] - 2017-05-24
### Added
- hover-border classes
- improved examples
- more child classes

## [1.2.34] - 2017-04-14
### Added
- child class docs
- added .child-first classes

## [1.2.31] - 2017-03-31
### Added
- .no-scroll-bars-ever
- .code-sample always has .no-scroll-bars

## [1.2.30] - 2017-03-31
### Added
- easier to read examples
- .no-scroll-bars

## [1.2.28] - 2017-02-21
### Added
- .no-a-style has been enhanced to effect child a-tags of .no-a-style
- .code-sample
- updated dev dependencies

## [1.2.25] - 2016-12-14
### Changed
- README.md is more condensed and now uses links to offer better jumping around
### Added
- more radius classes like .radius-left-5

## [1.2.24] - 2016-12-6
### Added
- more child classes
- .form-group-label class
### Changed
- form-group label assumptions

## [1.2.23] - 2016-10-08
### Added
- .child-margin .child-pad .child-hover-bg classes

## [1.2.19] - 2016-10-07
### Added
- .radius shorthand of border-radius
- .a-no-style

## [1.2.18] - 2016-09-20
- Added .no-unserline and .text-decoration-none

## [1.2.17] - 2016-09-15
- Added flex-stack reverse classes

## [1.2.10] - 2016-09-09
- Added back more forcebale .flex# classes (.flex1, .flex2)
- Added .opacity-0

## [1.2.9] - 2016-08-23
- .flex is implied into .flex- classes
- sass variables are in a default like mode

## [1.2.7] - 2016-08-22
### Added
- bg hover classes
- table color striping

## [1.2.6] - 2016-08-17
### Breaking Change
- .flex-wrap had unneccessary "flex-flow:row" definition (not changing minor vnum due to minor number change only yesterday)
### Added
- .margin-4x classes
- .pad-4x classes
- .flex-inline
- .flex-stacked
- .flex-row-wrap
- .flex-column-wrap

## [1.2.1] - 2016-08-16
### Altered
- Docs now pad and margin with 2x 3x classes instead of md and lg
### Added
- More max-width, max-height, min-width, min-height classes
- margin and pad 2x 3x classes

## [1.2.0] - 2016-08-16
### Added
- .text-6x, .text-7x, .text-8x, .text-9x
### Breaking Change
- .text-5, .text-4, .text-3x, and .text-2x have been reduced in size

## [1.1.9] - 2016-08-15
### Added
- more greys
- deprecated muted
- border classes

## [1.1.0] - 2016-08-12
### Breaking Change
- How flex-# classes adjust

## [1.0.29] - 2016-08-12
### Added
- table classes

## [1.0.19] - 2016-08-04
### Added
- responsive hide width/height/max-width/max-height classes

## [1.0.13] - 2016-08-04
### Added
- responsive below classes

## [1.0.12] - 2016-08-04
### Added
- ack-responsive-boot

## [1.0.7] - 2016-08-03
### Added
- File organization structure
- .overflow- classes

## [1.0.4] - 2016-07-29
### Created CHANGELOG