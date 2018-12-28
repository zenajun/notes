# Mastering Markdown

* [Paragraphs and Text Decoraction](#paragraphs-and-text-decoration)
* [Headings](#headings)
* [Links](#links)
* [Images](#images)
* [Lists - Ordered, Unordered, Bullets and Nesting](#lists---ordered-unordered-bullets-and-nesting)
* [Line Breaks, Horizontal Rules and Block Quotes](#line-breaks-horizontal-rules-and-block-quotes)

---

## Paragragraphs and Text Decoration

|Text Decoration|Code|
|:--------------|:---|
|*Italic*| `_Italic_` or `*Italic*`|
|**Bold**|`**Bold**`|
|***Bold and Italic***|`***Bold and Italic***`|
|~~Strikethrough~~|`~~Strikethrough~~`|

## Headings

# `# Heading 1`

## `## Heading 2`

### `### Heading 3`

## Links

|Link|Code|Syntax|
|:---|:---|:-----|
|<http://zenajun.com>|`<http://zenajun.com>`|`<link>`|
|[My page](http://zenajun.com)|`[My page](http://zenajun.com)`|`[text](link)`|
|[My page](http://zenajun.com "My portfolio")|`[My page](http://zenajun.com "My portfolio")`|`[text](link "title")`|
|Check out [my][1] site.|`Check out [my][1] site`<br><br> *`[1]: http://zenajun.com`<br> |`[text][ref]`| 

**Write link references at the bottom of our code to keep your file organized and avoid having long url's in your MD.  It will also make updating links easier.*

## Images
Syntax: `![alt text](link "title")`

`![Wow great pick!](http://unsplash.it/250/250?random "cool pic")` becomes:

![Wow great pick!](http://unsplash.it/250/250?random "cool pic")


### Using the link

`![Cute Pup][pup]`<br>
`[pup]: http://unsplash.it/250/250?image=1012`<br>
becomes:

![Cute Pup][pup]

[pup]: http://unsplash.it/250/250?image=1012

### Thumbnail image

`[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)` becomes:<br>
[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)


You can also use `<img>`

`[<img src="http://unsplash.it/50/50?image=1000">](http://unsplash.it/500/500?image=1000)` which is the same thing.

## Lists - Ordered, Unordered, Bullets and Nesting

### Unordered list

Syntax: `-`, `+` or `*`

```
* item 1
* item 2
* item 3
```
becomes:

* item 1
* item 2
* item 3


### Ordered List

Sytax: `1.`
```md
1. first
1. second
1. third
```

1. first
1. second
1. third

### Nesting

Use spaces or tabs
```
* One
* Two
 * i
 * ii
```

* One
* Two
  * i
  * ii

## Line Breaks, Horizontal Rules and Block Quotes

### Line Breaks

Syntax: `<br>` or `add a space`

```md
Zena is cool.<br>
Hello
```
Zena is cool.<br>
Hello

### Horizontal rules 

Syntax: `___` or `---`

---

### Block Quotes

Syntax: `>`

```md
> You miss 100% of the shots you don't take. - Wayne Gretzky
>
> Another line here
```

> You miss 100% of the shots you don't take. - Wayne Gretzky
>
>Another line here



## Code Blocks

Syntax: ` ``` `


 ` ```html `<br>
 `<ul>`<br>
 `  <li>item x</li>`<br>
 `  <li>item y</li>`<br>
 `</ul>`<br>
 ` ``` ` 
 
 ```html
 <ul>
   <li>item x</li>
   <li>item y</li>
 </ul>
 ```

### Inline code

Syntax: ` ` `

```
Hey did you try `const x = 100`?
```

Hey did you try `const x = 100`?


### Difference

```diff
var x = 100;
-var y = 200;
+var y = 300;
```

You can write inline with ` `` `

##  Tables

Using `|`
Left align: `|:-----------|:--------|`
Centered: `|:---:|:--:|`
Right align: `|---:|---:|`

|Dog's name  |Dog's Age|
|:-----------|:--------|
|Loki|4|
|Snickers|2|


## GitHub Treats

* [x] Get Milk
* [] Get Eggs

```
* [x] Get Milk
* [] Get Eggs
```

I had the same problem in #51 

`I had the same problem in #51 `


