# PDF Generator

Generates a PDF from HTML with embedded resources.

Installs the wkhtmltopdf engine on Rocky Linux 8 for the Expanse HPC without
requiring root access.  Provides a wrapper script `pdfgen` which is used to
convert HTML with table data, SVG images, and other external resources as a
bundled PDF for distribution.

First execute `install_wkhtmltopdf` and then `pdfgen` with the absolute path to
the directory which contains your `index.html` and its referenced resources.

