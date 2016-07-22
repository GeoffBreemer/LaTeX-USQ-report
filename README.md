# LaTeX-USQ-report
LaTeX template for USQ reports. Uses BiBLaTeX for referencing.

# Using biber instead of BibTex as the backend
The line below instructs TeXShop to use biber as the back-end, it MUST appear in the first 20 lines of code in the document to a) work and b) avoid weird errors. The `%` is required, it does NOT mean the line is commented out.

`% !BIB TS-program = biber`

# Start here: initial setup
- rename `USQ Report template.tex` to something more useful
- update `personal-settings.tex`
- update `other/toc-figures-tables.tex' to include/exclude the table of figures, tables etc.

# While writing the report
- create/edit chapter and appendix .tex files and store them in the `content` and `appendices` subfolder respectively
- store images in the `images` subfolder
- add/delete reference to/from `references/bibliography-references.bib`
- add/delete chapters, appendices and other report parts to/from `USQ Report template.tex`

# Typically done during the final stages
- update `content/conclusion.tex` (optional)
- update `content/introduction.tex` (optional)
- update `content/recommendations.tex` (optional)
- update `other/abstract.tex` (optional)
- update `other/acknowledgments` (optional)
- update `other/glossary-abbreviations` (optional)
- update `other/letter-of-transmittal.text` (optional)

# To generate the .PDF using TeXShop
- run LaTeX
- run BibTex (which will actually run BibLaTeX using biber as the backend)
- run LaTeX
- run LaTeX again

# Subfolders used by this document
- `appendices`: all appendices
- `content`: regularly edited text, e.g. introduction, chapters, conclusion and recommendations
- `images`: all image files
- `misc`: code style definitions
- `other`: all "one-off" text, e.g. title page, letter of transmittal, abstract
- `references`: bibliography/references, the .bib file
- `settings`: containing bibliography and page settings

# Word count
Run texcount:

`texcount -v -inc -nobib "name of main tex file.tex"`