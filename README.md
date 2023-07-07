# Smoke Tests

This repository contains the current state of the app! All contents must be considered UNTESTED. It should not be used by students for learning!!

## URL

- [https://mathebuddy.github.io/smoke/](https://mathebuddy.github.io/smoke/)
- note that the test instance shows solutions and all individual levels on the start page for debugging purposes.

## Android App

- **CAUTION:** This is a test build, without an identified developer ID. Test is at your own risk! You may reduce your system security settings (as requested while installing).
- Click on one of the links below (that is appropriate to your device) and then select "view raw" to download the APK file
  - [android/app-arm64-v8a-release.apk](android/app-arm64-v8a-release.apk)
  - [android/app-armeabi-v7a-release.apk](android/app-armeabi-v7a-release.apk)

## Known bugs / limitations / design issues

- level overview icons are still too small (max 3 columns or horizontal scrolling?)
- larger exercises should be split up, with possiblity to evaluate parts of it
- SMPL code "let phi = randZ(-1,1)*pi/rand({2,3,6});" is generated to TeX (e.g.) "\frac{-pi}{3}" instead of "-\frac{pi}{3}"
- SMPL code should allow to include the students answer for evaluation
- keyboards should open automatically, if there is only one exercise in the current view
- automatically move to the next input field after pressing the "enter" key
- repeat-exercise button must draw instances that are distinct to prior ones
- keyboard input field: if the input is longer than the field, things become strange..
- "-1-2-3" on keyboard is rendered as "1 + -2 + -3"
- missing navigation button to (default) next level (at the end of the current level)
- CAS is still limited/buggy (in some "circumstances": decimal representation instead of symbolic terms, e.g. "1.57..." instead of "pi/2"; or "1/2+1" instead of "3/2"); known bugs are marked by "work-in-progess"-texts
- the context-sensitive keyboard for answers is too restricted in some cases; especially polar form input is currently not yet available; known bugs are marked by "work-in-progess"-texts
- the TeX-engine is inaccurate in spacing. E.g. "\left{1,2,3\right}" is really ugly...
- scoring is not persisted
- chatbot (that asks randomized questions) is not yet present
- "events" are not yet gamified

## Implemented, but not yet online - NEWEST FIRST

(list is currently empty)

## Fixed (only items since announcement on 27 June 20:00) - NEWEST FIRST

2023-07-07

- refactored complete app code
- "Navigator" is now used to push/pop app pages

2023-06-30

- pressing on "DEBUG" (or "RELEAE") in the title bar switches between debug and release mode.
- some buttons have confused testers.
  (a) The exercise passed/OK check now has no border and thus does not seem to be a clickable button any longer
  (b) Added backward/forward buttons at the end of a level-page
- repeating an exercise that has been passed, does not longer vanish scores.
- the level progress is now indicated by a linear progress bar on the top
- icons in exercises, definitions have been removed
- added MBL syntax to force special keyboards (e.g. with "`^(`"-key).
- leaving the current unit does not vanish all progress anymore
- vertical alignment of bullet points in itemize lists has been improved

2023-06-29

- level overview: a lock symbol for non-accessible levels is shown. Currently, at least 50 % must be reached to pass a level. NOTE: Since the progress can not be persisted yet, also locked levels can be opened.
- LL-parsing of unary-minus wrongly used an unary expression as operand, instead of a multiply-expression (e.g. "-x/y" war wrongly parsed to "(-x)/y" instead of "-(x/y)")

2023-06-28

- added a tutorial template
- added button to repeat randomized exercises
- progress within level is now shown
- progress in level overview is now shown
- keyboard: non-numeric chars/strings are now separated by "*" (e.g. "isqrt(" -> "i * sqrt(")
- invalid term inputs are now marked by a border at top and bottom of the input field
- permanent headers (top bar + level navigation bar) consumed too much vertical space on small screens
- level oberview: icons are rearranged to fill 4 columns max
- level overview graph now shows edges
