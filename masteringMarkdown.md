# Mastering Markdown

* [Paragraphs and Text Decoraction](#paragraphs-and-text-decoration)
* [Headings](#headings)
* [Links](#links)
* [Images](#images)

---

## Paragragraphs and Text Decoration

|Text Decoration|Code|
|:--------------|:---|
|**Bold**|`**Bold**`|
|_Italic_| `_Italic_` or `*Italic*`|
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

`![Wow great pick!](http://unsplash.it/500/500?random "cool pic")` becomes:

![Wow great pick!](http://unsplash.it/500/500?random "cool pic")


`![Cute Pup][pup]`<br>
`[pup]: http://unsplash.it/500/500?image=1012`<br>
becomes:

Using the link

![Cute Pup][pup]
[pup]: http://unsplash.it/500/500?image=1012

Thumbnail image

`[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)` becomes
[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)




## Lists - Ordered, unordered, Bullets and Nesting

### Groceries:
- item 1, or
* item 2, or
+ item 3

`- item 1, or`

`* item 2, or`

`+ item 3`

### Todo:
1. first
1. second
1. third

```txt
1. first
1. second
1. third
```

## Line Breaks, Horizontal Rules and BlockQuotes

Zena is cool.<br>
Hello

Or add a space

Horizontal rules `===` or `---`

===

> You miss 100% of the shots you don't take. - Wayne Gretzky
>
>Another line here

`> You miss 100% of the shots you don't take. - Wayne Gretzky`
`>`
`>Another line here`

## Code Blocks

```html
<ul>
  <li>item</li>
  <li>item</li>
</ul>
```

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


