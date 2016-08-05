---
title: "The last Word"
categories: opinions
excerpt: "We seemed to have been stuck with _Word_ forever. Except for things do not stay in one place."
excerpt_separator: "<!--more-->" 
---

John Gruber with the help of Aaron Shwarz relieved the pain of writing awkward
html to writing straightforward
[Markdown](http://daringfireball.net/projects/markdown/).  Yes, yes, yes and
yes! Was it difficult? - I cannot know.  Was it needed? - Yes!

<!-- more -->

From:

```html
<div class="entry-content"><p>John Gruber with the help of Aaron Shwarz
relieved the pain of writing awkward html to writing straightforward
<a href="http://daringfireball.net/projects/markdown/">Markdown</a>. 
Yes, yes, yes and yes! Was it difficult? &ndash; I cannot know. 
Was it needed? &ndash; Yes!</p>
```

we've got:

```markdown
John Gruber with the help of Aaron Shwarz relieved the pain of writing awkward
html to writing straightforward
[Markdown](http://daringfireball.net/projects/markdown/).  Yes, yes, yes and
yes! Was it difficult? - I cannot know.  Was it needed? - Yes! 
```

In the following I will argue that before long _Markdown_ will kill _Word_.  I
am talking about _MS Word_. _Markdown_ with all its
seemingly superficial simplicity has the power to throw such an
blow.

## Prelude

We seemed to have been stuck with _Word_ forever.

Except for things do not stay in one place. In the last decade a number of
species of text manipulation and formatting tools have become dramatically
better and fitter, though working with plain text (code) for computer programs.
_Word_ seems to remain much the same and we seem to have become resigned to its
interface and behavior.

When I say dramatically better, I am looking into the direction of the modern
text and code editors and IDEs, tools that software developers and designers
use. Just look at _Sublime Text_ and catching up _Atom_ or _Coda2_ -- sleek,
extensible, fast.[^2]  _Sublime Text_, for instance, has taken the best of what
is out there in code manipulation and put it into an appealing interface. Any
software developer or web designer who cares about her tools has a well-tuned
IDE or editor of choice.


[^2]: [Sublime Text](http://www.sublimetext.com) and [Coda2](http://panic.com/coda/) are not free, [Atom by Github](https://atom.io) is

Other alternatives to _Word_ have been around since early Cenozoic times:
powerful text editors like _Vim_ or _Emacs_ are around for decades.  Whereas
_LaTeX_ -- a typesetting system for formatting sophisticated articles -- is
extensively used in scientific community since 1980s.[^3]

[^3]: Forgot to mention -- these are free. [Here's one example of what _LaTeX_ can produce](http://tug.ctan.org/tex-archive/macros/latex/contrib/elsarticle/doc/els2.pdf)

## The effort

After working with _Markdown_ documents for long enough, I
realized that Markdown-style text editing is a great middle point between
WYSYWIG and markup-based text processing. (I am aware of pro and contra
decoupling text manipulation from styling.)  However, only now __the effort of
working with markup-based solution is less than an effort of editing in WYSYWIG
mode__.  To me, this is a new spiral in a slow evolution of text manipulation
-- a tipping point for adoption of Markdown-style text editing by general
users. 

And it's already there.  _Markdown_ kinds spread over the Web and are now
almost everywhere: Wikipedia, StackOverflow, Github, blogs (including this one)
to name a few. New stylish editors for Markdown appear:
[Mou](http://mouapp.com), [Ulysses III](http://ulyssesapp.com).

Why? Because _Markdown_ is simple and adequate. You can type it in a _Notepad_
or on your phone and get a result of a _Word_ value.[^4]

[^4]: More details about _Markdown_ and tools for OSX on [Tuts+](http://computers.tutsplus.com/tutorials/introducing-markdown-on-os-x--cms-20764)

## Separation of concerns: content, structure and style

<!-- This one is not new. No one needs to invent a wheel here. -->

_Markdown_ allows you to focus on Content and Structure, and only on them.[^5]
Then you focus on Style, independently. Style is external to the content and it
can be flexibly adjusted.  Have you even written a postcard? Didn't you try out
wording on a scratch paper first?

[^5]: You can separate them in _Word_ as well, but only in the first edit. Once you've formatted your text in Word, all consecutive edits will require adjustment of Content, Structure and Style altogether.

There is still something we need to work on: __How do we add style?__

Of course style can be in _CSS_ -- that is how we have it in the Internet --  
`Markdown -> HTML` + `CSS` = `Happy`.  Except for _CSS_ is not convenient to
learn or use by general users. There must be some visual editor that would help
them to tweak and adjust styling in a intuitive way. Ideally, tweaking should
humbly live in the _Markdown_ editor and spit out _SASS_ or _CSS_ if asked.

Visual _CSS_ editors start to appear. For instance,
[Stylizer](http://www.skybound.ca) is tuned for intuitive style editing with
immediate feedback, though still not an option for anyone who does not know
_CSS_.

[Deckset](http://decksetapp.com) approaches _Markdown_ styling from another
angle -- it takes care of the style and generates styled presentations. You
focus on the content and the app provides you with predefined trendy styles
(that you can't change, yet).

The solutions are out there to be put together. We don't need _Word_ anymore. We
are changing the way we think about text editing.


P.S.: Now that _Word_ is sorted out, how do we go about _Excel_?

