
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

### Journal-specific options

Each of these should be placed under the `journal:` name.

For example,

```yaml
journal:
  name: "Journal of Example Studies"
```

- `title`: The name of the journal to use
- `doi`: The DOI or "DOI HERE" as a placeholder
- `copyright-year`: The year of copyright, e.g. 2025
- `publication-year`: The year of publication, e.g. 2019
- `advance-access`: The date to include, in `"Day Month Year"` format.
- `paper-type`: The subject section, typically a subtype of article.
- `first-page`: For submission, should typically be `1`.
- `received-date`: The date the article was received, formatted in 3 parts:
  - `year`: The year the article was received, e.g. 2024
  - `month`: The month the article was received, e.g. 01
  - `day`: The day the article was received, e.g. 15
- `revised-date`: The date the article was revised, formatted in 3 parts:
  - `year`: The year the article was revised, e.g. 2024
  - `month`: The month the article was revised, e.g. 02
  - `day`: The day the article was revised, e.g. 20
- `accepted-date`: The date the article was accepted, formatted in 3 parts:
  - `year`: The year the article was accepted, e.g. 2024
  - `month`: The month the article was accepted, e.g. 03
  - `day`: The day the article was accepted, e.g. 01

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf',pages = 1)  -->
![[template.qmd](template.qmd)](template_1.png)

## License

This project is a derivative of [OUP General Template](https://www.overleaf.com/latex/templates/oup-general-template/ybpypwncdxyb), licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) by Oxford University Press.  
All changes and additions in this repository are also licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/) by Christopher T. Kenny.

