# README

Having taken Tiago Forte's course on knowledge management (called [Building a
Second Brain]) I've started highlighting interesting parts of the books
I'm reading.

Rather than leave these highlights languishing within my ebook reader, I then
import the highlights into a note taking app (e.g. Notion) where I can easily
skim through them, highlight key points, etc.

While Notion are apparently working on an API, it's not yet as easy as it could
be to automatically load this kind of data into it. So while I wait for an API
and a bunch of IFTTT recipes to present themselves, I'm using some little
utilities to help me get by.

So far, the list of supported ebook platforms is short!

## Book highlights from O'Reilly Learning site

O'Reilly provide a CSV file containing all the highlights you've made to
any of the books that you read on https://learning.oreilly.com.

The `oreilly-book` script generates a Markdown file containing the
highlights from a specific book, that can then be imported into a note-taking
app. It was written to get highlights into Notion, but it's just generating
Markdown, so will work with any app that can import Markdown.

Run it like this:

    $ ./oreilly-book "Book Title" < safari-annotations-export.csv > book.md

The "Book Title" string must match the first column in the CSV file for
the book you're extracting highlights for.

[Building a Second Brain]: https://www.buildingasecondbrain.com
