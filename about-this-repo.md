# About this repository

I write my resume in Markdown so it's easy to edit, serve on GitHub (which
automatically renders it as HTML), and convert to PDF.  The files in this repo are:

* README.md: The simplest version of my resume
  - Served at <https://github.com/jeffs/resume/>
  - Also available on GitHub pages at <https://jeffs.github.io/resume/>
* about-this-repo.md: This file
* jeff-schwab.pdf: My resume, rendered as a PDF
* pdf.css: Styles for generating jeff-schwab.pdf
* pdf.md: Stylized Markdown for generating the PDF

Updates to the resume are performed thus:

1. Edit README.md by hand
2. Copy updated content from README.md to pdf.md
3. Convert pdf.md to HTML
    ```sh
    markdown pdf.md > pdf.md.html
    ```
4. Serve the HTML version locally, and tweak the styles as needed
    ```sh
    miniserve .
    open http://localhost:8080/pdf.md.html
    ```
5. Save as jeff-schwab.pdf
