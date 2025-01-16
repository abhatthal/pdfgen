# PDF Generator

Generates a PDF from HTML with embedded resources.

Installs the wkhtmltopdf engine on Rocky Linux 8 for the Expanse HPC without
requiring root access.  Provides a wrapper script `pdfgen` which is used to
convert HTML with table data, SVG images, and other external resources as a
bundled PDF for distribution.

First execute `install_wkhtmltopdf` and then `pdfgen` with the absolute path to
the directory which contains your `index.html` and its referenced resources.

## Projects using pdfgen
### [Quakeworx](https://qwx1.onescienceway.com/)
Quakeworx is a science gateway for seismic simulations. Certain Quakeworx
applications (i.e. UCERF3-ETAS) return plot results as an HTML file with links
to plot charts, CSV files, and external CSS for styling. This cannot be
rendered inside the gateway. PDF Generator is used to produce a single document
with all resources embedded inside it for easy distribution and viewing
online.

See details about how PdfGen is used on SCECpedia at
https://strike.scec.org/scecpedia/PdfGen.

