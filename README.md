# LaTeX-USQ-report
LaTeX template for USQ reports.

# Using biber instead of BibTex as the backend
The line below instructs TeXShop to use biber as the back-end, it MUST appear in the first 20 lines of code in the document to a) work and b) avoid weird errors. The % is required, it does NOT mean the line is commented out.

% !BIB TS-program = biber

# To generate the .PDF
- optional: update references/bibliography-references.bib
- Run LaTeX
- run BibTeX/biber
- run LaTeX
- run LaTeX again

# Subfolders used by this document
- appendices: all appendices
- content: regularly edited text, e.g. introduction, chapters, conclusion and recommendations
- images: all image files
- other: all "one-off" text, e.g. title page, letter of transmittal, abstract
- references: bibliography/references, the .bib file
- settings: containing bibliography and page settings
