TORINO, A PRETTY THEME FOR LATEX-BEAMER
=======================================

## Authors
Marco Barisione <marco@barisione.org>
Bozhidar Batsov
Stefan Fochler

## Abstract
Beamer (http://latex-beamer.sourceforge.net/) is a LaTeX class that
allows you to create presentations.  Beamer contains several
full-featured (but a bit ugly) themes, so Marco wrote this pretty theme
(but with some missing features) called Torino.

## Installation
First of all, you have to install Beamer, directly from source or
using an already made package for your distro.  Then install the
theme, on a Unix system just type in a terminal:

```bash
$ sudo cp -r themes /usr/share/texmf/tex/latex/beamer/
$ sudo texhash
```

### Mac
On a mac with the MacTeX package, copy the files to the regarding folders in
`~/Library/texmf/tex/latex/beamer/themes` and don't forget to run `texhash`
afterwards.

## Usage
Now you are ready to use the theme, for documentation read the example
files: chameleon.tex nouvelle.tex and freewilly.tex.  Compiling them
you get some slides with documentation:

```bash
$ pdflatex chameleon.tex
$ pdflatex nouvelle.tex
$ pdflatex freewilly.tex
```

### Additional Features
#### Navigation
You can enable a simple navigation bar with the `navigation=true` flag (just
like `titleline=true` or `alternativetitlepage=true`). Navigation can be turned
off by `\navigationoff` and back on again with `\navigationon`. This is usefull
for e.g. the title page. Note, that this only works when navigation is enabled
via `navigation=true` in the `\usetheme` command!