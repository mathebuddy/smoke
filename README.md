# Smoke Tests

This repository contains the current state of the app! All contents must be considered UNTESTED. It should not be used by students for learning!!

## URL
- [https://mathebuddy.github.io/smoke/](https://mathebuddy.github.io/smoke/)
- note that the test instance shows solutions and all individual levels on the start page for debugging purposes.

## Known bugs / limitations / design issues
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
- buttons may not be understood well. TODO:   a) Exercises: remove border around "check-OK" after successful evaluation to indicate that this is not a clickable button   b) Add backward/forward buttons at the end of a level-page
- keep scores when repeating an exercise!
- remove icons in exercises, definitions, .. (since page icons are present anyway...)
- option to enable special keyboards for certain exercises (e.g. if "^" is needed).
- leaving the current unit vanishes all progress
- bullet points in itemize lists are rendered vertically too high

## Fixed (only items since announcement on 27 June 20:00) - NEWEST FIRST

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

