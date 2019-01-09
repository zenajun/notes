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

Match a range of characters with `-`

`/[a-e]/ig` matches any character between a and 3, including the a and e.

`/[0-5]/g` matches any number between 0 and 5, including the 0 and 5.

Combine a range of letters and numbers in a single character set, `/[a-e][2-6]/ig`

To create a negated character set, you place `^` after the opening bracket and before the characters you do not want to match.

`/[^aeiou]/gi` matches all character that are not vowels.

Match Characters that Occur One or More Times with `+`

`'bass.match(/s/ig)'`  returns **'s,s'**

`'bass.match(/s+/ig)'` returns **'ss'**

Match Characters that Occur Zero or More Times with `*`

`'gooooooooal!'.match(/go*/);` returns **'goooooooo'**

`'gut feeling'.match(/go*/);` returns **'g'**

`'over the moon'.match(/go*/)` returns **null**
