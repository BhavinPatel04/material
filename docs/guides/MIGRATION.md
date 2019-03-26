# Migration to Angular Material and the Angular CDK

## Key Concepts

// TODO

## Directives
Most directives changed to components. These make for straight forward conversions, for instance
`<md-card>` changed to `<mat-card>`.

Some element directives changed to attribute directives, for instance `<md-subheader>` changed to
`matSubheader`.

| Directive          | Old Docs     | New Docs     | Notes                                                  |
|--------------------|--------------|--------------|--------------------------------------------------------|
| autocomplete       |   [Docs][41] |   [Docs][24] |                                                        |
| autofocus          |   [Docs][69] |   N/A        |                                                        |
| button             |   [Docs][43] |   [Docs][1]  |                                                        |
| calendar           |   [Docs][70] |   N/A        |                                                        |
| card               |   [Docs][44] |   [Docs][2]  |                                                        |
| checkbox           |   [Docs][45] |   [Docs][3]  |                                                        |
| chip               |   [Docs][71] |   [Docs][26] |                                                        |
| chip-remove        |   [Docs][72] |   [Docs][26] | `matChipRemove`                                        |
| chips              |   [Docs][46] |   [Docs][26] |                                                        |
| colors             |   [Docs][73] |   N/A        | [`mat-color` mixin][74] supports static theme color lookups. No support for dynamic theming.|
| contact-chips      |   [Docs][75] |   N/A        |                                                        |
| content            |   [Docs][76] |   [Docs][77] | `cdkScrollable`                                        |
| datepicker         |   [Docs][47] |   [Docs][25] |                                                        |
| divider            |   [Docs][49] |   [Docs][35] |                                                        |
| fab-speed-dial     |   [Docs][78] |   N/A        |                                                        |
| fab-toolbar        |   [Docs][79] |   N/A        |                                                        |
| grid-list          |   [Docs][50] |   [Docs][9]  |                                                        |
| highlight-text     |   [Docs][80] |   N/A        |                                                        |
| icon               |   [Docs][51] |   [Docs][10] |                                                        |
| ink-ripple         |   [Docs][81] |   [Docs][19] | `matRipple`                                            |
| input              |   [Docs][52] |   [Docs][5]  | `matInput`                                             |
| input-container    |   [Docs][82] |   [Docs][83] | `mat-form-field`                                       |
| list               |   [Docs][53] |   [Docs][8]  |                                                        |
| menu               |   [Docs][54] |   [Docs][17] |                                                        |
| menu-bar           |   [Docs][84] |   N/A        |                                                        |
| nav-bar            |   [Docs][85] |   [Docs][86] | `mat-tab-nav-bar`                                      |
| nav-item           |   [Docs][87] |   [Docs][88] | `mat-tab-link`                                         |
| optgroup           |   [Docs][89] |   [Docs][90] |                                                        |
| option             |   [Docs][91] |   [Docs][23] |                                                        |
| progress-linear    |   [Docs][55] |   [Docs][12] | `mat-progress-bar`                                    |
| progress-circular  |   [Docs][56] |   [Docs][11] | `mat-progress-spinner`                                 |
| radio-button       |   [Docs][57] |   [Docs][4]  |                                                        |
| radio-group        |   [Docs][92] |   [Docs][93] |                                                        |
| select             |   [Docs][59] |   [Docs][23] |                                                        |
| select-on-focus    |   [Docs][94] |   N/A        |                                                        |
| sidenav            |   [Docs][60] |   [Docs][6]  |                                                        |
| sidenav-focus      |   [Docs][95] |   N/A        | [autofocus][96] only supports focusing the first focusable element.|
| switch             |   [Docs][61] |   [Docs][14] | `mat-slide-toggle`                                     |
| slider             |   [Docs][62] |   [Docs][16] |                                                        |
| slider-container   |   [Docs][97] |   N/A        |                                                        |
| subheader          |   [Docs][98] |   [Docs][99] | `matSubheader`                                         |
| swipe              |   [Docs][100]|   N/A        | See [HammerJS setup][101] and [Hammer.Swipe][102]      |
| tabs               |   [Docs][64] |   [Docs][13] |                                                        |
| textarea           |   [Docs][65] |   [Docs][5]  |                                                        |
| toolbar            |   [Docs][66] |   [Docs][7]  |                                                        |
| tooltip            |   [Docs][67] |   [Docs][18] |                                                        |
| truncate           |   [Docs][103]|   N/A        |                                                        |
| virtual-repeat     |   [Docs][68] |   [Docs][40] | `cdk-virtual-scroll-viewport` and `*cdkVirtualFor`     |
| whiteframe         |   [Docs][104]|  [Guide][105]| Based on classes and mixins                            |

## Services

| Service          | Old Docs     | New Docs     | Notes                                                  |
|------------------|--------------|--------------|--------------------------------------------------------|
| $mdBottomSheet   |   [Docs][42] |   [Docs][38] | `MatBottomSheet`                                       |
| $mdDialog        |   [Docs][48] |   [Docs][22] | `MatDialog`                                            |
| $mdInkRipple     |   [Docs][58] |   [Docs][19] | `matRippleTrigger`                                     |
| $mdPanel         |   [Docs][109]|   [Docs][110]| `Overlay`                                              |
| $mdToast         |   [Docs][63] |   [Docs][21] | `MatSnackBar`                                          |

// TODO flesh out the rest of the services


## Features
// TODO break down the differences in each

| Feature          | Old Docs     | New Docs     | Notes                                                  |
|------------------|--------------|--------------|--------------------------------------------------------|
| theming          |  [Guide][106]|  [Guide][20] |                                                        |
| typography       |  [Docs][107] |  [Guide][27] |                                                        |
| layout           |  [Guide][108]|  [Wiki][0]   |                     See [@angular/flex-layout][lay_rp] |
| cdk              |  N/A         |   [Docs][34] |                                                        |

## New Components
These are new components found in Angular Material that do not exist in AngularJS Material.

| Directive        |     Docs     |
|------------------|--------------|
| badge            |   [Docs][37] |
| button-toggle    |   [Docs][15] |
| data-table       |   [Docs][28] |
| drag-drop        |   [Docs][39] |
| expansion-panel  |   [Docs][32] |
| paginator        |   [Docs][29] |
| sort-header      |   [Docs][30] |
| stepper          |   [Docs][33] |
| tree             |   [Docs][36] |


 [0]: https://github.com/angular/flex-layout/wiki
 [1]: https://material.angular.io/components/button/overview
 [2]: https://material.angular.io/components/card/overview
 [3]: https://material.angular.io/components/checkbox/overview
 [4]: https://material.angular.io/components/radio/overview
 [5]: https://material.angular.io/components/input/overview
 [6]: https://material.angular.io/components/sidenav/overview
 [7]: https://material.angular.io/components/toolbar/overview
 [8]: https://material.angular.io/components/list/overview
 [9]: https://material.angular.io/components/grid-list/overview
[10]: https://material.angular.io/components/icon/overview
[11]: https://material.angular.io/components/progress-spinner/overview
[12]: https://material.angular.io/components/progress-bar/overview
[13]: https://material.angular.io/components/tabs/overview
[14]: https://material.angular.io/components/slide-toggle/overview
[15]: https://material.angular.io/components/button-toggle/overview
[16]: https://material.angular.io/components/slider/overview
[17]: https://material.angular.io/components/menu/overview
[18]: https://material.angular.io/components/tooltip/overview
[19]: https://material.angular.io/components/ripple/overview
[20]: https://material.angular.io/guide/theming
[21]: https://material.angular.io/components/snack-bar/overview
[22]: https://material.angular.io/components/dialog/overview
[23]: https://material.angular.io/components/select/overview
[24]: https://material.angular.io/components/autocomplete/overview
[25]: https://material.angular.io/components/datepicker/overview
[26]: https://material.angular.io/components/chips/overview
[27]: https://material.angular.io/guide/typography
[28]: https://material.angular.io/components/table/overview
[29]: https://material.angular.io/components/paginator/overview
[30]: https://material.angular.io/components/sort/overview
[31]: https://tina-material-tree.firebaseapp.com/simple-tree
[32]: https://material.angular.io/components/expansion/overview
[33]: https://material.angular.io/components/stepper/overview
[34]: https://material.angular.io/cdk/categories
[35]: https://material.angular.io/components/divider/overview
[36]: https://material.angular.io/components/tree/overview
[37]: https://material.angular.io/components/badge/overview
[38]: https://material.angular.io/components/bottom-sheet/overview
[39]: https://material.angular.io/cdk/drag-drop/overview
[40]: https://material.angular.io/cdk/scrolling/overview#virtual-scrolling
[41]: https://material.angularjs.org/latest/api/directive/mdAutocomplete
[42]: https://material.angularjs.org/latest/api/service/$mdBottomSheet
[43]: https://material.angularjs.org/latest/api/directive/mdButton
[44]: https://material.angularjs.org/latest/api/directive/mdCard
[45]: https://material.angularjs.org/latest/api/directive/mdCheckbox
[46]: https://material.angularjs.org/latest/api/directive/mdChips
[47]: https://material.angularjs.org/latest/api/directive/mdDatepicker
[48]: https://material.angularjs.org/latest/api/service/$mdDialog
[49]: https://material.angularjs.org/latest/api/directive/mdDivider
[50]: https://material.angularjs.org/latest/api/directive/mdGridList
[51]: https://material.angularjs.org/latest/api/directive/mdIcon
[52]: https://material.angularjs.org/latest/api/directive/mdInput
[53]: https://material.angularjs.org/latest/api/directive/mdList
[54]: https://material.angularjs.org/latest/api/directive/mdMenu
[55]: https://material.angularjs.org/latest/api/directive/mdProgressLinear
[56]: https://material.angularjs.org/latest/api/directive/mdProgressCircular
[57]: https://material.angularjs.org/latest/api/directive/mdRadioButton
[58]: https://material.angularjs.org/latest/api/service/$mdInkRipple
[59]: https://material.angularjs.org/latest/api/directive/mdSelect
[60]: https://material.angularjs.org/latest/api/directive/mdSidenav
[61]: https://material.angularjs.org/latest/api/directive/mdSwitch
[62]: https://material.angularjs.org/latest/api/directive/mdSlider
[63]: https://material.angularjs.org/latest/api/service/$mdToast
[64]: https://material.angularjs.org/latest/api/directive/mdTabs
[65]: https://material.angularjs.org/latest/api/directive/mdInput
[66]: https://material.angularjs.org/latest/api/directive/mdToolbar
[67]: https://material.angularjs.org/latest/api/directive/mdTooltip
[68]: https://material.angularjs.org/latest/api/directive/mdVirtualRepeat
[69]: https://material.angularjs.org/latest/api/directive/mdAutofocus
[70]: https://material.angularjs.org/latest/api/directive/mdCalendar
[71]: https://material.angularjs.org/latest/api/directive/mdChip
[72]: https://material.angularjs.org/latest/api/directive/mdChipRemove
[73]: https://material.angularjs.org/latest/api/directive/mdColors
[74]: https://material.angular.io/guide/theming-your-components#note-using-the-code-mat-color-code-function-to-extract-colors-from-a-palette
[75]: https://material.angularjs.org/latest/api/directive/mdContactChips
[76]: https://material.angularjs.org/latest/api/directive/mdContent
[77]: https://material.angular.io/cdk/scrolling/overview#cdkscrollable-and-scrolldispatcher
[78]: https://material.angularjs.org/latest/api/directive/mdFabSpeedDial
[79]: https://material.angularjs.org/latest/api/directive/mdFabToolbar
[80]: https://material.angularjs.org/latest/api/directive/mdHighlightText
[81]: https://material.angularjs.org/latest/api/directive/mdInkRipple
[82]: https://material.angularjs.org/latest/api/directive/mdInputContainer
[83]: https://material.angular.io/components/form-field/overview
[84]: https://material.angularjs.org/latest/api/directive/mdMenuBar
[85]: https://material.angularjs.org/latest/api/directive/mdNavBar
[86]: https://material.angular.io/components/tabs/overview#tabs-and-navigation
[87]: https://material.angularjs.org/latest/api/directive/mdNavItem
[88]: https://material.angular.io/components/tabs/api#MatTabLink
[89]: https://material.angularjs.org/latest/api/directive/mdOptgroup
[90]: https://material.angular.io/components/select/overview#creating-groups-of-options
[91]: https://material.angularjs.org/latest/api/directive/mdOption
[92]: https://material.angularjs.org/latest/api/directive/mdRadioGroup
[93]: https://material.angular.io/components/radio/overview#radio-groups
[94]: https://material.angularjs.org/latest/api/directive/mdSelectOnFocus
[95]: https://material.angularjs.org/latest/api/directive/mdSidenavFocus
[96]: https://material.angular.io/components/sidenav/api#MatSidenav
[97]: https://material.angularjs.org/latest/api/directive/mdSliderContainer
[98]: https://material.angularjs.org/latest/api/directive/mdSubheader
[99]: https://material.angular.io/components/list/overview#lists-with-multiple-sections
[100]: https://material.angularjs.org/latest/api/directive/mdSwipeDown
[101]: https://material.angular.io/guide/getting-started#step-5-gesture-support
[102]: http://hammerjs.github.io/recognizer-swipe/
[103]: https://material.angularjs.org/latest/api/directive/mdTruncate
[104]: https://material.angularjs.org/latest/api/directive/mdWhiteframe
[105]: https://material.angular.io/guide/elevation
[106]: https://material.angularjs.org/latest/Theming/01_introduction
[107]: https://material.angularjs.org/latest/CSS/typography
[108]: https://material.angularjs.org/latest/layout/introduction
[109]: https://material.angularjs.org/latest/api/service/$mdPanel
[110]: https://material.angular.io/cdk/overlay/overview 

[0107]: https://github.com/angular/material2/issues/107
[0119]: https://github.com/angular/material2/issues/119
[0108]: https://github.com/angular/material2/issues/108
[0114]: https://github.com/angular/material2/issues/114
[0115]: https://github.com/angular/material2/issues/115
[0118]: https://github.com/angular/material2/issues/118
[0546]: https://github.com/angular/material2/issues/546
[0117]: https://github.com/angular/material2/issues/117
[0120]: https://github.com/angular/material2/issues/120
[0123]: https://github.com/angular/material2/issues/123
[0205]: https://github.com/angular/material2/issues/205
[0860]: https://github.com/angular/material2/issues/860
[0408]: https://github.com/angular/material2/issues/408
[0508]: https://github.com/angular/material2/issues/508
[0823]: https://github.com/angular/material2/issues/823
[0581]: https://github.com/angular/material2/issues/581
[4191]: https://github.com/angular/material2/pull/4191
[0995]: https://github.com/angular/material2/pull/995
[0474]: https://github.com/angular/material2/pull/474

[aio]: https://material.angular.io
[getting-started]: https://material.angular.io/guide/getting-started
[lay_rp]:  https://github.com/angular/flex-layout
