# Blizzard.j Fix

Putting on my plumber hat to fix leaks and shiet

Source: original files + paths

Licence: I don't watch TV but must pay for it.

...Whatever license I decide upon later (if I need to) shall retroactively
apply to my earlier changes (patches) here.

## Explanation

> In Jass you must set local variables that hold agents (or any child type) to `null`
at the end of functions to avoid reference counter leaks.

Further reading:

1. <https://github.com/lep/jassdoc/pull/108>
2. <https://www.hiveworkshop.com/threads/jass-contest-how-would-you-avoid-local-variable-leaks.374040/>

## Ignored files

```
./scripts/h06_green.ai:    local player kill     = null
./scripts/reforged_u05_navy.ai:    local unit target = null
./scripts/reforged_u08_blue.ai:    local unit target = null
./scripts/reforged_u08_red.ai:    local unit target = null
./scripts/reforged_u08_teal.ai:    local unit target = null
./scripts/u05_mint.ai:    local unit target = null
```
