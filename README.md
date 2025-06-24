
# Oxford University Press Article Template

## Creating a New Article

To create a new article using this format:

```bash
quarto use template christopherkenny/oup
```

This will create a new directory with an example document that uses this format.

## Using with an Existing Document

To add this format to an existing document:

```bash
quarto add christopherkenny/oup
```

Then, add the format to your document options:

```yaml
format:
  oup-pdf: default
```    

## Options

- `layout`: One of `contemporary`, `modern`, or `traditional`. This controls the style of the document. Defaults to `contemporary`.
- `papersize`: One of `large`, `medium`, or `small`. This controls the paper size of the document. Defaults to `large`.
- `namedate`: Default `false` for regular numbered reference style. Change to `true` for `authoryear`-style references.
- `lineno`: Default `false`. Change to `true` to enable line numbers in the document.
- `running-title`: Short title for the running header. Defaults to the title without subtitle.
- `running-author`: Short author name for the running header.

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf',pages = 1) 
![[template.qmd](template.qmd)](template_1.png) -->

## License

This project is a derivative of [OUP General Template](https://www.overleaf.com/latex/templates/oup-general-template/ybpypwncdxyb), licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) by Oxford University Press.  
All changes and additions in this repository are also licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/) by Christopher T. Kenny.

