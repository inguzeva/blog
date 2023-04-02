---
title: Markdown
subtitle: This post is about how to write on Markdown

# Summary for listings and search engines
summary: This post is about how to write on Markdown

# Link this post with a project
projects: []

# Date published
date: '2023-04-02T00:00:00Z'

# Date updated
lastmod: '2023-04-02T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.

authors:
  - Irina

tags:
  - Markdown

categories:
  - study
---

```python
import libr
print('hello')
```

## About the Markdown

Markdown is a readable markup language that is transparently converted to HTML. You can open and edit it in any text editor. It is widely used for writing documentation and README files.


## Syntax. Paragraph

A paragraph is one or more consecutive lines of text separated by one or more empty lines. If a string contains only spaces or tabs, it is still considered empty.

Consecutive lines will be glued into one, if you do not add a hard transfer. There are several ways to do this:

add two (or more) spaces at the end of < >< >;
add a backslash at the end of the line \;
add an HTML line wrap tag <br>.


## Headings

Markdown offers two styles of writing headings: through lattices (#) and through underscores (====). You can use up to six levels of headings, but underscores only allow you to create the first two (<h1> and <h2>).

🤓
In English-language sources, the terms Atx-style (for lattices) and Setext-style (for underscores) are used to indicate the styles of writing headings.


## Grilles

Grilles (Atx-style) Copy the link to the section "Lattices (Atx-style)"
In order to select the title, you need to put from 1 to 6 bars (#) and a space at the very beginning of the line. The level of the header depends only on the number of lattices.


## Underscores (Setext-style)

"Underlining" a paragraph with equal signs (=) or hyphens (-) makes it the title of the first or second level, respectively. The level of the header depends only on the type of "dashes", their number does not matter.

There should be no empty lines between the text and the underline.


## Lists. Marked

To create bulleted (unnumbered) lists, you need to put a minus (-), plus (+) or an asterisk (*) before each item. The marker and the text of the paragraph must be separated by a space. If there are different markers in front of the items in a row, then after the conversion we will get different lists.

## Ordered

If we use numbers with a dot at the end (1., 2., etc.) as markers, we will get an ordered (numbered) list. The item numbers in the final markup will go in order (1, 2, 3), even if markdown will be 1., 4., 9.. This feature allows us to use "lazy numbering", when the same number is placed before each item. The number before the first item shows where to start numbering the list items, so if you put 99., 22. in Markdown, then in the final markup the items will be under the numbers 99, 100, 101. 1.

## Nesting 

Any lists can be nested within each other, for this you need to put a tab or several spaces in front of the marker.
The number of spaces you need to use to nest one list within another can vary. It depends on the number of characters in the parent marker (L):

+ — 1 character (L = 1)
1. — 2 characters (L = 2)
99. — 3 characters (L = 3)
Before the nested list, you need to put from L + 1 to L + 4 spaces.


## Quotes

If you put a triangular bracket (>) at > the line, Markdown will turn the text after it into a quote. Inside can be any blocks: paragraphs, headlines or even other quotes.


## Source code

Markdown allows you to mark up the source code in a special way, all characters inside will be automatically escaped. There are 3 ways how this can be done:

Wrap the code with one or two pairs of backsticks (`код`)
Wrap the code with three or more pairs of backsticks (```код```)
Put a tab or 4 spaces before each line of code


## One or two pairs of backsticks 

This method allows you to insert the source code as a lowercase element. Even if we actually have a few lines of code wrapped in backsticks, we will still get one line after converting to HTML.

## Three or more pairs of backsticks 

If we wrap one line of code with three or more pairs of backsticks, we get a lowercase element, and if there are several lines, then a block element. The second option allows you to specify the programming language that we use, for this we need to write it immediately after the opening backsticks.

After designating the programming language, nothing will change visually, but this will allow additional plug-ins and scripts to highlight the code inside the block.


## Indentation 

Another way to highlight the code is to put a tab or 4 spaces in front of it. The source code must be separated by an empty line from the previous block.


## Select text 

If you wrap text with asterisks (*) or underscores (_), it becomes bold or italic. Both characters work the same way, the selection style depends only on their number:

one pair * or _ will make the text *italic*;
two * or _ will make the text **bold**;
three * or _ will apply both styles***.

To escape markdown service characters, you need to put a backslash before each of them (\*, \_, \*\*).


## Standardization 

Markdown has an original specification from one of the language's creators, John Gruber. Unfortunately, it doesn't always unambiguously describe the syntax, which is why many Markdown converters work differently. To remedy this situation, a group of "Markdown fans" created CommonMark, a specification that describes many special cases, and a reference implementation of the Markdown parser on JS.




## Resource

https://doka.guide/tools/markdown/
