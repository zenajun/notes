# RegEx

`/string/`

`.test()` will return **true** or **false**

`Regex.test(string);`

`.match()` to extract the actual match

`string.match(Regex);`

## Search for multiple patterns with the OR operator `|`

`/yes|no|maybe/`

## Ignore case `i`

`/a/i` will look for **A** or **a**

## Find more than the first match with `g`

`/string/g`

## Wildcard character `.`

`/abc./` will search for all strings that contain 'abc' within them

## Character classes 

`[]` - define a group of characters you wish to match

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

### Match a range of characters with `-`

`/[a-e]/ig` matches any character between a and 3, including the a and e.

`/[0-5]/g` matches any number between 0 and 5, including the 0 and 5.

Combine a range of letters and numbers in a single character set, `/[a-e][2-6]/ig`

### Match all letters and numbers

`/[A-Za-z0-9_]/` - matches upper and lowercase letters plus numbers including _.

The shorthand for `/[A-Za-z0-9_]/` is `/\w/`

### Match everything but letters and numbers

Longhand: `[^A-Za-z0-9_]`

Shorthand: `\W`

### Match all numbers

Longhand: `[0-9]`

Shorthand: `\d`

### Match all non-numbers

Longhand: `[^0-9]`

Shorthand: `\D`

### Match Whitespace

`\s` matches **whitespace** including **carriage return**, **tab**, **form feed** and **new line** characters.

### Match Non-Whitespace
`\S`


### To create a negated character set, you place `^` after the opening bracket and before the characters you do not want to match.

`/[^aeiou]/gi` matches all character that are not vowels.

 Outside of a character set, the `^` is used to search for patterns at the beginning of strings.
 
 `/*Cat/` will only search the beginning of the string
 
`/^Cat/.test('Cat');` returns **true**

`/^Cat/.test('Black Cat');` returns **false**

## Match Characters that Occur One or More Times with `+`

`'bass.match(/s/ig)'`  returns **'s,s'**

`'bass.match(/s+/ig)'` returns **'ss'**

## Match Characters that Occur Zero or More Times with `*`

`'gooooooooal!'.match(/go*/);` returns **'goooooooo'**

`'gut feeling'.match(/go*/);` returns **'g'**

`'over the moon'.match(/go*/)` returns **null**

## Lazy matching

`?`Finds the smallest possible part of the string that satisfies the regex pattern.

Regex is by default greedy (finds the longest possible match)

`'titanic'.match(/t[a-z]i/ig);` returns **titani**

`'titanic'.match(/t[a-z]*i?/ig);` returns **ti**


## Match Ending String Patterns with `$`

`/story$/.test('This is a never ending story)` returns **true**

`/story$/.test('Sometimes a story will have to end)` returns **false**

## Quantify Specifiers

`{}` - Specify the upper and lower number of matches

```js
let A4 = "aaaah";
let A2 = "aah";
let multipleA = /a{3,5}h/;
multipleA.test(A4); // Returns true
multipleA.test(A2); // Returns false
```

