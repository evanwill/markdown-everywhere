---
title: Markdown
nav: Intro
---

[Markdown](https://daringfireball.net/projects/markdown/){:target="_blank" rel="noopener"} is a quick and simple standard to create formatted documents in plaintext.

Originally developed in 2004 by John Gruber with Aaron Swartz based on how people intuitively write emails, it focuses on being human readable, yet designed to easily convert into HTML for the web.

Markdown files are plaintext, usually with the extension `.md`, and can be edited by any text editor.
Think of it as source code for your content, that can be easily read and understood, but also compiled to generate outputs such as HTML, .docx, or PDF.
Because of it's simplicity and flexibility, a growing number of websites, note taking apps, publishing systems, and code notebooks use Markdown to format content, making it a powerful, cross-platform option for academic and tech writing. 

## Flavors

It is important to keep in mind that Markdown isn't a formal standard, but comes in "flavors" from various specifications or implementations that add additional features. 
Some common flavors:

- [CommonMark](https://commonmark.org/){:target="_blank" rel="noopener"} (attempt to standardize, led by John MacFarlane of Pandoc)
- [GitHub Flavored Markdown (GFM)](https://github.github.com/gfm/){:target="_blank" rel="noopener"} (popular style that can be used any where on GitHub)
- [Pandoc Markdown](https://pandoc.org/MANUAL.html#pandocs-markdown){:target="_blank" rel="noopener"} (document-centric extensions)
- [kramdown](https://kramdown.gettalong.org/syntax.html){:target="_blank" rel="noopener"} (the Ruby markdown parser)
- [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/){:target="_blank" rel="noopener"} (PHP)
- [MultiMarkdown](https://fletcherpenney.net/multimarkdown/){:target="_blank" rel="noopener"}
- [R Markdown](https://rmarkdown.rstudio.com/){:target="_blank" rel="noopener"}

One of the benefits of these various Markdown parsers is that they usually allow a mix of other types of markup inside an `.md` file, including LaTeX style math, HTML elements, and code blocks making it a flexible base to write content in an efficient manner.

## Lightweight Markup languages

Lightweight markup languages seek to be easy to write and read, while providing expressive semantic markup that can be used to transform the marked up content into different formats.
Some popular examples (other than Markdown) include:

- [Wikitext](https://en.wikipedia.org/wiki/Help:Wikitext){:target="_blank" rel="noopener"}
- [AsciiDoc](http://asciidoc.org/){:target="_blank" rel="noopener"}
- [reStructuredText](http://docutils.sourceforge.net/docs/ref/rst/introduction.html){:target="_blank" rel="noopener"}
- [Org-Mode](https://orgmode.org/){:target="_blank" rel="noopener"}

Opportunities:

- Simple(ish) to learn
- [Plaintext](https://en.wikipedia.org/wiki/Plain_text){:target="_blank" rel="noopener"} and open standards -based
    - shareable and useable by any device with no special software or license needed
    - preservable / sustainable - easy digital preservation and human readable
    - version controllable - you can use the full power of Git or other version control systems
- Separation of content/semantics and presentation
    - spend less time formatting, more time writing - don't waste time in complex and frustrating formatting in Word that will be deleted by publishers anyway!
    - structure content as data = powerful, more useful, more accessible
- Flexible outputs - ready for web, ebooks, blogs, not just PDFs.

Example: 
Karthik Ram, "Git can facilitate greater reproducibility and increased transparency in science", *Source Code Biol Med* 8, 7 (2013), https://doi.org/10.1186/1751-0473-8-7. Available at <https://github.com/karthik/smb_git>
