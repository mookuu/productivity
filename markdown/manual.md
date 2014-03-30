Manual for markdown
===================

#### M1: block

> Block1.
>
> Block2.

#### M2: list-unorder

* List1

* List2

+ List3

+ List4

- List5

- List6

#### M3: list-ordered

1. List1

2. List2

#### M4: emphasis

* Use two asterisks for **strong emphasis**.

* Use two underscores for __strong emphasis__.

#### M5_1: linkage

* [Google](https://www.google.com)

* [github](https://github.com/Takechiyocn "Title: Github")

#### M5_2: linkage-->reference

* [Google][reference1]

* [github][reference2]

[reference1]: https://github.com/Takechiyocn "Github"
[reference2]: https://www.google.com "Google"

#### M6: picture

![Picture](img.jpg "Title: Picture")

![Picture][p_id]

[p_id]: img.jpg "Title: Picture"

#### M7: code block-->&、< and >

`Code with codeblock quotation: <blink>`

Code without codeblock quotation: <blink>

`Code with codeblock quotation: &mdash`

Code without codeblock quotation: &mdash

`Code with codeblock quotation: &#8212`

Code without codeblock quotation &mdash

#### M8: XHTML backwoard compatility

If you want your page to validate under XHTML 1.0 Strict,
you've got to put paragraph tags in your blockquotes:

<blockquote>
<p>For example.</p>
</blockquote>

