# RegEx

`/string/`


Search for multiple patterns with the OR operator `|`

`/yes|no|maybe/`

Ignore case `i`

`/a/i` will look for **A** or **a**

`.match()` to extract the actual match

`string.match(Regex)`

Find more than the first match with `g`

`/string/g`

Wildcard character `.`

`/abc./` will search for all strings that contain 'abc' within them

Character classes `[]` - define a group of characters you wish to match

`/b[aiu]g/`

```javascript
  let bigStr = "big";
  let bagStr = "bag";
  let bugStr = "bug";
  let bogStr = "bog";
  let bgRegex = /b[aiu]g/;
  bigStr.match(bgRegex); // Returns ["big"]
  bagStr.match(bgRegex); // Returns ["bag"]
  bugStr.match(bgRegex); // Returns ["bug"]
  bogStr.match(bgRegex); // Returns null
```
