---
title: Markdown Basics
nav: Write
---

Academic documents are usually organized using Headers and Paragraphs, which correspond to semantic structure elements even though it is mostly intuitive.


## Headings 

Headings range from level one to six, with one being the most important concepts.
They should generally move up in order without skipping a level.

Be sure to include a blank line above and below a heading.

{% capture atxtext %}
<div class="row">
<div class="col-md-6" markdown="1">
```
# Heading One

## Heading Two

### Heading Three
```
</div>
<div class="col-md-6 md-demo" markdown="1">
# Heading One

## Heading Two

### Heading Three
</div>
</div>
{% endcapture %}
{% include card.html text=atxtext %}

## Paragraphs 

Paragraphs don't require any special markup.
Just leave an empty line between your paragraphs and any other block element.
For example:

{% capture par %}
```
Any text with no empty lines between will be joined into a paragraph.
Leave an empty line between headings and paragraphs.

Since there is an empty line above, 
this will start a new paragraph.
This gives you the option to write a paragraph all on one line 
(like a word processor),
or to put each sentence on its own line.
Splitting the sentences can make editing and version control easier. 
```

----------------

Any text with no empty lines between will be joined into a paragraph.
Leave an empty line between headings and paragraphs.

Since there is an empty line above, 
this will start a new paragraph.
This gives you the option to write a paragraph all on one line 
(like a word processor),
or to put each sentence on its own line.
Splitting the sentences can make editing and version control easier. 
{% endcapture %}
{% include card.html text=par %}

## Lists

A bullet list (i.e. **unordered list**) is created using `-` followed by a space (alternatively can use `*` or `+`).
Put each list item on a new line.
A numbered list (i.e. **ordered list**) is created using a number + `.` followed by a space.
The items will be automatically renumbered correctly in outputs. 
Both kinds of lists can be nested by tabbing in a level.

{% capture lists %}
<div class="row">
<div class="col-md-6" markdown="1">
```
- dog
- cat
- muffin
```
</div>
<div class="col-md-6  md-demo" markdown="1">
- dog
- cat
- muffin
</div>
</div>
<hr>
<div class="row">
<div class="col-md-6" markdown="1">
```
1. dog
2. cat
6. muffin
1. other thing
```
</div>
<div class="col-md-6 md-demo" markdown="1">
1. dog
2. cat
6. muffin
1. other thing
</div>
</div>
<hr>
<div class="row">
<div class="col-md-6" markdown="1">
```
1. dog
    - bark
    - wag
2. cat
    - meow
6. muffin
    - yum
```
</div>
<div class="col-md-6 md-demo" markdown="1">
1. dog
    - bark
    - wag
2. cat
    - meow
6. muffin
    - yum
</div>
</div>
{% endcapture %}
{% include card.html text=lists %}

{% include alert.html text="Although Markdown is simple, it is important to remember that white space, blank lines, and tabs matter. If you are getting unexpected results when rendering, check your white space. For example, leaving two spaces at the end of a line will insert a `<br>` break." color="warning" %}

## Inline Elements

{:.table .table-bordered}
| Markdown | HTML |
| --- | --- |
| `*Emphasis*` or `_emphasis_` | *Emphasis* or _emphasis_ |
| `**Strong**` or `__strong__` | **Strong** or __strong__ |
| `inline [hyperlink](https://www.google.com)` | inline [hyperlink](https://www.google.com) |
| `image ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png)` | image ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png) |
| `footnote.[^1]` | footnote.[^1] |

`[^1]: example footnote definition.`

[^1]: example footnote definition.

## Code 

{% capture code %}

    Code can be highlighted inline with `backticks`.

    {% raw %}```{% endraw %}
    Or make a code block 
    open with three backticks alone on a line 
    and close with three more on a line. 
    {% raw %}```{% endraw %}

    This makes it possible to copy unformatted code/text from your writing.

----------------

Code can be highlighted inline with `backticks`.

```
Or make a code block 
open with three backticks alone on a line 
and close with three more on a line. 
```

This makes it possible to copy unformatted code/text from your writing.

{% endcapture %}
{% include card.html text=code %}

## Tables 

Tables aren't supported by all Markdown converters, but can be useful for some quick structure.

{% capture table %}

```
| column1 | column2 | column3 |
| --- | --- | --- |
| value | value | value |
| value | value | value |

```

-----------

{:.table .table-bordered}
| column1 | column2 | column3 |
| --- | --- | --- |
| value | value | value |
| value | value | value |

{% endcapture %}
{% include card.html text=table %}

## Block Elements

Here are some more things to try:

```

Horizontal rule is three or more dashes on a line:

-------------

> Block quote.
> Continuing the quote.

```
