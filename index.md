---
layout: page
title: hipsteR
tagline: re-educating people who learned R before it was cool.
---

I was an early adopter of [R](http://www.r-project.org), having first
learned S (yay!) and then S-plus (yuck!). But at times my knowledge of
R seems stuck in 2001. I keep finding out about &ldquo;new&rdquo; R
functions (like `replicate`, which was new in _2002_).

This is a tutorial for people like me.

### Step 1: switch to knitr

If you use [Sweave](http://leisch.userweb.mwn.de/Sweave/), it's time
you switched to [knitr](http://yihui.name/knitr/). You'll find that
the transition is easy.

A number of Sweave annoyances have been eliminated, but most
importantly you can use knitr
[with R Markdown](http://kbroman.github.io/knitr_knutshell/pages/Rmarkdown.html)
or
[with AsciiDoc](http://kbroman.github.io/knitr_knutshell/pages/asciidoc.html)
for writing simple reports. The markup is much simpler than LaTeX, and
you don't have to worry about page breaks.

### Step 2: Learn [Hadley Wickham](http://had.co.nz/)'s packages

Start with [dplyr](https://github.com/hadley/dplyr),
[reshape2](https://github.com/hadley/reshape), and
[ggplot2](http://ggplot2.org/).

Also [devtools](https://github.com/hadley/devtools),
[roxygen2](https://github.com/klutometis/roxygen), and
[testthat](https://github.com/hadley/testthat).

Also [lubridate](https://github.com/hadley/lubridate) and
[stringr](https://github.com/hadley/stringr).

Also, read his [Advanced R programming](http://adv-r.had.co.nz/) book.


### Step 3: You _can_ put underscores in names

It used to be that `_` was a shortcut for `<-`. (That was always a bad
idea. And it led me to use dots in function names, like
[`calc.genoprob`](https://github.com/kbroman/qtl/blob/master/R/calc.genoprob.R),
which has been problematic due to the S3 class system.)

Then they started allowing `=` in place of `<-`.

And then they got rid of `_` as a shortcut for `<-`.  Good idea, and
now we can have functions named like `calc_genoprob`.


---

The source for this tutorial is
[on github](http://github.com/kbroman/hipsteR).

I would be glad for suggestions, corrections, or additions.

Also see my
[git/github guide](http://kbroman.github.io/github_tutorial),
[knitr in a knutshell tutorial](http://kbroman.github.io/knitr_knutshell),
and [minimal make tutorial](http://kbroman.github.io/minimal_make).