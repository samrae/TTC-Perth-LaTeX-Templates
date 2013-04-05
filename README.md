# TTC Perth LaTeX Templates

This is a set of template files for creating assignments for **Trinity Theological College**, Perth, Australia using [LaTeX](http://www.latex-project.org) and, optionally, [Scrivener](http://www.literatureandlatte.com/scrivener.php).

## Requirements
These instructions assume that you already know how to typeset a file in LaTeX and are set up for it.

XeLaTeX is used to typeset the document, so you will need that installed and configured for the LaTeX app (or command line) you use. [TeXShop](http://pages.uoregon.edu/koch/texshop/) works well for me.

You will, of course, have to make sure that all the packages used in `ttc-header` are installed.

### Fonts
The template by default uses the following fonts:

- Standard text: Times New Roman (as required by Trinity)
- Hebrew: [SBL Hebrew](http://www.sbl-site.org/educational/BiblicalFonts_SBLHebrew.aspx)
- Greek: [Linux Libertine O](http://www.linuxlibertine.org/index.php?id=1&L=1)

For über-typesetting, I recommend buying the offical [Times New Roman® Std Regular MT](http://www.fontshop.com/fonts/downloads/monotype/times_new_roman_std_regular/) font from Monotype. It will give you:

- small caps
- old-style numerals
- ligatures
- proper superscripts
- better appearance all-round

It costs around $28.


## Installation for Mac
### LaTeX
Move the **ttc-assignments** directory into `~/Library/texmf/tex/latex/`, or alternatively any directory in LaTeX's path.

Move the **Trinity.bst** BibTeX style file into `~/Library/texmf/bibtex/bst/`.

### Scrivener
Move the *contents* of the **Compile settings** directory into `~/Library/Application Support/Scrivener/CompileSettings/`

Move the *contents* of the **Project templates** directory into `~/Library/Application Support/Scrivener/ProjectTemplates/`

## Installation for everything else
The LaTeX files should work on any platform that can run LaTeX. The Scrivener files should work on Windows, but we haven't tested it.

## Usage

### With Scrivener
1. Create a new project with the TTC Assignment template. The template has a fair bit of documentation on how to use various LaTeX commands in Scrivener.
2. **Compile** the project with **Format As:** College Essay — LaTeX.
3. Open the resulting `.tex` file and typeset it.

### LaTeX without Scrivener
Put these lines at the top of your file:

	\input{ttc-header}
	\input{ttc-start}

And this line at the end:

	\input{ttc-end}

The header and end files are very short because of the way Scrivener uses LaTeX includes. You might want to use only `ttc-header`—that's where all the goodies are.
