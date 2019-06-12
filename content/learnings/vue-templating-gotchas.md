---
title: Vue templating gotchas
tags:  ["Vue.js"]
goal:  Front-End Engineering
date:  2019-05-19
draft: false

---
Don’t mix `v-for` & `v-if` on the same el; v-for has unexpectedly higher precedence. Instead, move the if to a parent el, and move filters to a computed property (function) for more performant, dependably logical flow

Keep complicated logic out of HTML templates and in computed functions. Keep templates declarative!
