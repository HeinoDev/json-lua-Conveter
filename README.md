# json-lua-tool

a desktop converter that flips between json and lua table syntax. built for fivem devs who get tired of rewriting locale files and config tables by hand.

## what it does

- **json → lua** - turn json objects into properly formatted lua tables
- **lua → json** - parse lua tables back to json (useful for apis, config exports)
- handles nested structures, arrays, booleans, strings, numbers
- respects lua keywords and valid identifiers
- strips out lua comments and `return` statements automatically

## how to use

**windows only** - double click `convert.hta` and it opens as a desktop window. paste your json or lua in the left box, hit convert, copy the result from the right.

swap between modes with the buttons at the top. switch languages with the dropdown (english/dansk).

## limits

- only converts data structures, not code - no functions, commands, or logic
- if a lua table mixes array items and named keys at the same time, it becomes a json object not an array (rare edge case)

## files

- `convert.hta` - the app, ready to run
- `README.md` - you're reading it
