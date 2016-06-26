---
layout: post
title: sample markdown post
header_keywords_abstract : false
one_sentence: 学好markdown，走遍天下都不怕
header_image: kramdown.png
keywords:
- my first keywords
- my second keywords
- my third keywords
anchors:
- a1
- a2
- a3
---

Hello        {#a1}
-----

> note one line
> note same line

> note different line

# heading 1

## heading 2

`a = 2; import scikit`


First level header
==================

Second level header
------

   Other first level header
=


This is a normal
paragraph.






This is some text.[^1]. Other text.[^footnote].




And A Header
------------
And a paragraph

> This is a blockquote.

And A Header
------------


> This is a blockquote.
>     on multiple lines
that may be lazy.
>
> This is the second paragraph.


# Hello      {#a2}




> This is a paragraph.
>
> > A nested blockquote.
>
> ## Headers work
>
> * lists too
>
> and all other block-level elements



code blocks: five spaces or one space and one tab

>     import xxx

>     import xxx



> This is a paragraph inside
a blockquote.
>
> > This is a nested paragraph
that continues here
> and here
> > and here


Here comes some code

    This text belongs to the same code block.


    Here comes some code
^
    This one is separate.



~~~~~~~~
import xxx
a = s
	dsf
~~~~~~~~


~~~
def what?
  42
end
~~~
{: .language-ruby}


* kram
+ down
- now

1. kram
2. down
3. now


* This is the first line. Since the first non-space characters appears in
  column 3, all other indented lines have to be indented 2 spaces.
However, one could be lazy and not indent a line but this is not
recommended.
*       This is the another item of the list. It uses a different number
   of spaces for indentation which is okay but should generally be avoided.
   * The list item marker is indented 3 spaces which is allowed but should
     also be avoided and starts the third list item. Note that the lazy
     line in the second list item may make you believe that this is a
     sub-list which it isn't! So avoid being lazy!




*   Using a tab to indent this line, the tab only counts as three spaces
    and therefore the overall indentation is four spaces.

   1.   The tab after the marker counts here as three spaces. Since the
        indentation of the marker is three spaces and the marker itself
        takes two characters, the overall indentation needed for the
        following lines is eight spaces or tw


* kram

* down
* now        



*   First item

    A second paragraph

    * nested list

    > blockquote

*   Second item


|---+---+---|
+ :-: |:------| ---:|
| :-: :- -: -
:-: | :-



|-----------------+------------+-----------------+----------------|
| Default aligned |Left aligned| Center aligned  | Right aligned  |
|-----------------|:-----------|:---------------:|---------------:|
| First body part |Second cell | Third cell      | fourth cell    |
| Second line     |foo         | **strong**      | baz            |
| Third line      |quux        | baz             | bar            |
|-----------------+------------+-----------------+----------------|
| Second body     |            |                 |                |
| 2 line          |            |                 |                |
|=================+============+=================+================|
| Footer row      |            |                 |                |
|-----------------+------------+-----------------+----------------|


$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$


The following is a math block:

$$ 5 + 5 $$

But next comes a paragraph with an inline math statement:

\$$ 5 + 5 $$


\$\$ 5 + 5 $$


script style math option textarea pre code kbd samp var

<div markdown="1">This is the first part of a para,
which is continued here.
</div>


This is a para.
<!-- a *comment* -->
<? a processing `instruction`
   spanning multiple lines
?> First part of para,
continues here.



This is [a link](http://rubyforge.org) to a page.
A [link](../test "local URI") can also have a title.
And [spaces](link with spaces.html)!

This is a [link](http://example.com){:hreflang="de"}
Reference Links

This *is*{:.underline} some `code`{:#id}{:.class}.
A [link](test.html){:rel='something'} and some **tools**{:.tools}.

# Hello #    {#a3}

This is a [reference style link][linkid] to a page. And [this]
[linkid] is also a link. As is [this][] and [THIS].

The next paragraph contains a link and some text.

[Room 100]\: There you should find everything you need!

[Room 100]: link_to_room_100.html

*some text*
_some text_
**some text**
__some text__


This is un*believe*able! This d_oe_s not work!


This is a * literal asterisk.
These are ** two literal asterisk.
As \*are\* these!


Use `<html>` tags for this.


Here is a literal `` ` `` backtick.
And here is ``  `some`  `` text (note the two spaces so that one is left
in the output!).

This is a Ruby code fragment `x = Class.new`{:.language-ruby}






[^1]: Some *crazy* footnote definition.

[^footnote]:
    > Blockquotes can be in a footnote.

        as well as code blocks

    or, naturally, simple paragraphs.

[^other-note]:       no code block here (spaces are stripped away)

[^codeblock-note]:
        this is now a code block (8 spaces indentation)





This is some text not written in HTML but in another language!

*[another language]: It's called Markdown

*[HTML]: HyperTextMarkupLanguage
{:.mega-big}


--- will become an em-dash (like this —)




[linkid]: http://www.example.com/ "Optional Title"
