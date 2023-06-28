# Smoke Tests

This repository contains the current state of the app! All contents must be considered UNTESTED. It should not be used by students for learning!!

## URL
- [https://mathebuddy.github.io/smoke/](https://mathebuddy.github.io/smoke/)
- note that the test instance shows solutions and all individual levels on the start page for debugging purposes.

## Known bugs / limitations / design issues
- permanent headers (top bar + level navigation bar) may consume too much vertical space on small screens
- leaving the current unit vanishes all progress
- keyboard: non-numeric chars/strings must be separated by a space (e.g. "isqrt(" -> "i sqrt(")
- "-1-2-3" on keyboard is rendered as "1 + -2 + -3"
- missing navigation button to (default) next level (at the end of the current level)
- CAS is still limited/buggy (in some "circumstances": decimal representation instead of symbolic terms, e.g. "1.57..." instead of "pi/2"; or "1/2+1" instead of "3/2"); known bugs are marked by "work-in-progess"-texts
- the context-sensitive keyboard for answers is too restricted in some cases; especially polar form input is currently not yet available; known bugs are marked by "work-in-progess"-texts
- the TeX-engine is inaccurate in spacing. E.g. "\left{1,2,3\right}" is really ugly...
- scoring is not persisted

## Fixed (only items since announcement on 27 June 20:00)
- level oberview: icons should be arranged in 4 columns max
- level overview graph does not show edges

