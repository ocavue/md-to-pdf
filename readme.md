# Markdown to PDF

Simple tool to convert a markdown file to pdf. Uses [marked](https://www.npmjs.com/package/marked) to convert `markdown` to `html` and [html-pdf](https://www.npmjs.com/package/html-pdf) to convert `html` to `pdf`.

## Installation

Clone repo, then install the package with `npm`:

```plain
cd md-to-pdf
npm install -g
```

After that `md-to-pdf` (or alias `md2pdf`) is globally available from anywhere in your command line/terminal.

## Usage

The first argument is `path/to/file.md` and the second one optionally specifies the `path/to/output.pdf`. If you omit the second argument, it will derive the pdf name from the markdown file name and save it into the directory that contains the markdown file.

```sh
md-to-pdf readme.md
md2pdf readme.md ~/readme.pdf
```

**Page Break:** Place an element with class `page-break` to force a page break at a certain point of the document, e. g.:

```md
<div class="page-break"></div>
```

## Customization

If you don't like the style, just change `markdown.css` to your liking. The paper format and borders can be changed in `index.js`.
