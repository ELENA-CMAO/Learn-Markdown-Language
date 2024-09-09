# Learn-Markdown-Language

## Basic Syntax

### Headings
To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (< h3 >), use three number signs (e.g., ### My Header). 

### Paragraphs
To create paragraphs, use a blank line to separate one or more lines of text.

### Line Breaks
To create a line break or new line (< br >),  
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
If you need to start an unordered list item with a number followed by a period, you can use a *backslash* ( \ ) to escape the period. (1968\. is a good year.)

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

I love supporting the **`[EFF](https://eff.org)`**.
This is the *`[Markdown Guide](https://www.markdownguide.org)`*.
See the section on `[code]``(#code)`.

### Reference-style Links

> Reference-style links are a special kind of link that make URLs easier to display and read in Markdown. **Reference-style links are constructed in two parts:** the part you **keep inline with your text** and the part you **store somewhere else in the file** to keep the text easy to read. 

#### Formatting the First Part of the Link

> The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.
>
> Although not required, you can include a space between the first and second set of brackets. The label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.
>
> This means the following example formats are roughly equivalent for the first part of the link:
>
>    `[hobbit-hole][1]`
>    `[hobbit-hole] [1]`

#### Formatting the Second Part of the Link

> The second part of a reference-style link is formatted with the following attributes:
>
>    The label, in brackets, followed immediately by a colon and at least one space (e.g., `[label]:` ).
>    The URL for the link, which you can optionally enclose in angle brackets.
>    The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

This means the following example formats are all roughly equivalent for the second part of the link:

```
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)
```

**Example of putting both parts together:**

> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a `[hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles")`, and that means comfort.

Though it may point to interesting additional information, the URL as displayed really doesn’t add much to the existing raw text other than making it harder to read. To fix that, you could format the URL like this instead:

> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a `[hobbit-hole][1]`, and that means comfort. 
>
> `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`

In both instances above, the rendered output would be identical:

> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort. [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

*** 



### Horizontal Rules
To create a horizontal rule, **use three or more** asterisks (***), dashes (---), or underscores (___) on a line by themselves.
***

---

_________________

### Escaping Characters
To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash ( \ ) in front of the character.

\* Without the backslash, this would be a bullet in an unordered list.


### Images
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    `![Tux, the Linux mascot](/assets/images/tux.png)`

3. Close the file.

The rendered output looks like this:

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.

#### link images

* To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

`[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)`

[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

*** 

## More about MD ↓

[Extended Syntax - tables/aligment/formatting...](https://www.markdownguide.org/extended-syntax/)


