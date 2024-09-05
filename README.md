# Learn-Markdown-Language

## Basic Syntax

### Headings
To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (<h3>), use three number signs (e.g., ### My Header). 

### Paragraphs
To create paragraphs, use a blank line to separate one or more lines of text.

### Line Breaks
To create a line break or new line (<br>),  
end a line with two or more spaces, and then type return.

## Emphasis

### Bold
To bold text, add **two asterisks** or __underscores__ before and after a word or phrase. To **bold the middle of a word** for emphasis, add two as**ter**isks without spaces around the letters.

### Italic
To *italicize* text, add *one asterisk* or _underscore_ before and after a word or phrase. **To italicize the middle of a word** for emphasis, add one as*ter*isk without spaces around the letters.

### Bold and Italic
To emphasize text with **bold** and *italics* at the same time, add ***three asterisks*** or **_underscores_** before and after a word or phrase. To **bold and italicize the middle of a word** for emphasis, add three as***ter***isks without spaces around the letters.

### Blockquotes
To create a blockquote, add a **>** in front of a paragraph.

> Dorothy followed her through many of the beautiful rooms in her castle.

### Blockquotes with Multiple Paragraphs
Blockquotes can contain multiple paragraphs. Add a **>** on the blank lines between the paragraphs.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with 

### Nested Blockquotes
Blockquotes can be nested. Add a **>>** in front of the paragraph you want to nest.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with

### Blockquotes with Other Elements
Blockquotes can contain other Markdown formatted elements. **Not all elements can be used** — you’ll need to experiment to see which ones work.

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Lists 

### Ordered Lists
To create an ordered list, add line items with numbers followed by periods. **The numbers don’t have to be in numerical order, but the list should start with the number one.**

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item 

### Unordered Lists
To create an unordered list, add **dashes** (-), **asterisks** (*), or **plus signs** (+) in front of line items. Indent one or more items to create a nested list.

* First item
* Second item
* Third item
* Fourth item

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item 

### Starting Unordered List Items With Numbers
If you need to start an unordered list item with a number followed by a period, you can use a *backslash* \(\) to escape the period. (1968\. is a good year.)

### Links
To create a link, enclose the link text in **brackets** (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., (https://duckduckgo.com)).

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

### Adding Titles
You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. **To add a title, enclose it in quotation marks after the URL**.

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for")

### URLs and Email Addresses
To quickly turn a URL or email address into a link, **enclose it in angle brackets.**

<https://www.markdownguide.org>
<fake@example.com>

### Formatting Links
To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

### Horizontal Rules
To create a horizontal rule, **use three or more** asterisks (***), dashes (---), or underscores (___) on a line by themselves.
***

---

_________________

### Escaping Characters
To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash \(\) in front of the character.

\* Without the backslash, this would be a bullet in an unordered list.



