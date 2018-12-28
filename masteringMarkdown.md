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

Syntax: `![alt text](link "title")` or `[<img src="">](LINK)`

|Image|Code|
|:---:|:---|
|![Wow great pick!](http://unsplash.it/200/200?random "cool pic")|`![Wow great pick!](http://unsplash.it/200/200?random "cool pic")`|
|![Cute Pup][pup]|Using the link<br><br>`![Cute Pup][pup]`<br><br>`[pup]: http://unsplash.it/200/200?image=1012`|
|[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)|Thumbnail image<br><br>`[![]( http://unsplash.it/50/50?image=1012)]( http://unsplash.it/500/500?image=1012)`|

[pup]: http://unsplash.it/200/200?image=1012

## Lists - Ordered, Unordered, Bullets and Nesting

### Unordered list

Unordered List: `- `, `+ ` or `* `<br>
Ordered List: `1. `<br>
Nesting: `2 spaces` or `tab`


```
* item 1
* item 2
* item 3

1. first
1. second
1. third

* One
* Two
  * i
  * ii

```

* item 1
* item 2
* item 3

1. first
1. second
1. third

* One
* Two
  * i
  * ii

## Line Breaks, Horizontal Rules and Block Quotes

Line break: `<br>` or `\`<br>
Horizontal Rules: `---` or `___`<br>
Block Quotes: `>`

```
The first sentence.<br>
The second line!

---

>The quick brown fox jumped over the lazy dogs<br>
> **Mavis Beacon** 
```

The first sentence.<br>
The second line!

___

>The quick brown fox jumped over the lazy dogs<br>
> **Mavis Beacon** 



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


