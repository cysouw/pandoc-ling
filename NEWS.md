# pandoc-ling 1.8 (upcoming)

# pandoc-ling 1.7

## changes

- allow for no space between number and suffix in latex export
- bugfix latex-linguex (thx speechchemistry)

# pandoc-ling 1.6

## changes

- adding option `samePage` to determine whether examples are kept together on a page in Latex typesetting (#pr14, thanks to CLRafaelR)

## bugs

- allow for one-letter elements in glossing (#pr13, thanks to CLRafaelR)

# pandoc-ling 1.5

## changes

- removing the colon from the internal ID to harmonize the cross-document referencing

## bugs

- handling of `header-includes` improved: additional user-provided statements are just passed through.
- various internal changes to match the updated functioning of lua inside pandoc 2.12 and newer.

# pandoc-ling 1.4

## changes

- adding option to use bullet lists for example entry. Will still be transformed into labelled list.

## bugs

- fixed gb4e error prevented by adding `\noautomath` to preamble
- fixed gb4e error with cross-referencing because of wrong placement of `\label` statement
- fixed latex error when using special symbols in judgements (closes #4, thx @CLRafaelR)

# pandoc-ling 1.3.1

## bugs

- fixed bug with not-appearing header of interlinear in HTML output
- fixed bug with judgements in single-line examples (closes #3, thx @CLRafaelR)

# pandoc-ling 1.3

## changes

- changed the ID system to "#ex:" for easier cross-document linking to examples
- change @next and @last to lowercase for easier typing
- added 'samepage' enclosures in latex so that examples do not break across pages

## bugs

- resolved clash with pandoc-crossref
- corrected wrong counting with unnumbered headings
- fixed counter reset and \exewidth with gb4e
- fixed bugs with linguex export

# pandoc-ling 1.2

## changes

- adding experimental beamer as possible export. It uses the same routines as basic latex export. needs more testing.

## bugs

- fixed problem with parsing local options

# pandoc-ling 1.1

## changes

- adding experimental noFormat option to simply use the raw content of the example as a complete div to a single table cell and set number to vertically centred. For latex export, all lines are simply squashed together. needs more testing.

# pandoc-ling 1.0

First complete working version
