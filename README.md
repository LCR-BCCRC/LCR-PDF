# PrettyPDF

Quarto extension for a template to generate a PDF with LCR branding. This extension now allows you to style PDFs LaTeX. Simply use `LCR_PDF-pdf` as the format in the document yaml header.

## Installation and use

To install the Quarto extension, create a directory, and use the template file:

``` bash
quarto use template LCR-BCCRC/LCR-PDF
```

To use the extension in an existing project without installing the template file:

``` bash
quarto install extension LCR-BCCRC/LCR-PDF
```
Note that you will need to update the output format to `format: LCR_PDF-pdf` to enable use of the extension. For book projects, add:

```
project:
  type: LCR_PDF
```
to the `_quarto.yml` file.

## Adjusting LaTeX Styling

If you want to update the LaTeX version of this template to use a different colour or logo, open up the `_extensions/LCR_PDF/LCR-PDF.tex` file after you have installed the extension.

### Logo

Either replace the `logo.png` file with a new file of your choosing, or change the file path on line 28 to point to a different logo file. Note that the file path is relative to your .qmd file.

### Colours

Lines 14-16 in `_extensions/LCR_PDF/LCR-PDF.tex` define three colours used in the template: `light`, `dark`, and `highlight`. Change the hex colours in these lines to update the colours. The `_extensions/LCR_PDF/LCR-PDF.tex` and `_extensions/LCR_PDF/_extension.yml` files indicate how these colours are used throughout the documents, as headers, highlighting, link colours, etc.

## Blog

Read more about this extension from its original author at [nrennie.rbind.io/blog/making-pretty-pdf-quarto](https://nrennie.rbind.io/blog/making-pretty-pdf-quarto/).





