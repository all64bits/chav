# chav

CHapter And Verse: A fork of Bontibon's kjv terminal viewer for the KJV bible

## Goal

View versified texts from the command line. Planned additional features:

* User selectable source text
* Support for both verse-per-line view or multi-verse lines with line break flags in the source text
* Support for footnotes

## Todo

* Change kjv references to chav
* Allow for CHAV_TEXTS path for text sources; rather than internal tsv file
* Implement alternative multi-verse per line view option
* Implement footnotes functionality

## Existing Usage

    usage: ./kjv [flags] [reference...]

      -l      list books
      -W      no line wrap
      -h      show help

      Reference types:
          <Book>
              Individual book
          <Book>:<Chapter>
              Individual chapter of a book
          <Book>:<Chapter>:<Verse>[,<Verse>]...
              Individual verse(s) of a specific chapter of a book
          <Book>:<Chapter>-<Chapter>
              Range of chapters in a book
          <Book>:<Chapter>:<Verse>-<Verse>
              Range of verses in a book chapter
          <Book>:<Chapter>:<Verse>-<Chapter>:<Verse>
              Range of chapters and verses in a book

          /<Search>
              All verses that match a pattern
          <Book>/<Search>
              All verses in a book that match a pattern
          <Book>:<Chapter>/<Search>
              All verses in a chapter of a book that match a pattern

## Current Build Instructions

Clone the repository and then run make:

    git clone https://github.com/bontibon/kjv.git
    cd kjv
    make

## License

Public domain
