# Pandoc-heig

This repository is made to be used whenever you want to generate nice PDFs from a Markdown or a Latex file. Its first intended use is to execute the scripts directly in your terminal but as the scripts are written in bash you will need a UNIX operating system, or a WSL distribution.

Feel free to tweak the scripts and the other options present in the script.

The custom template that is used for pandoc is the excellent [Eisvogel][eisvogel-gh].

# How to use it ?
## Local
You will need pandoc and TeXLive installed for that as well as a custom pandoc template. The advantages of this method is that you have to install it only once and then you can just execute the scripts.

### Installation
- You can go to [Eisvogel - Installation][eisvogel-install] and follow the installation procedure.
- Take a look at [Eisvogel - LaTeX Packages][eisvogel-latex] before beginning the installation.
- Once the template is copied in the pandoc templates folder you are good to go

### Usage
To generate a PDF you have 2 options:
1) Execute the script `generate-pdf` with the following options :
   - `-f` to specify the Markdown filename [default: _README.md_]
   - `-o` to specify the pdf output name (do not put the extension here, only the name) [default: _Rapport_]
   - `-t` to specify which templates you want to use ([listing][eisvogel-listings] or [highlights][pandoc-highlights], see) [default: none]
2) Execute the script `pandoc-generate-styles` ...

## Docker image
To be continued...

[eisvogel-gh]: https://github.com/Wandmalfarbe/pandoc-latex-template
[eisvogel-install]: https://github.com/Wandmalfarbe/pandoc-latex-template#installation
[eisvogel-latex]: https://github.com/Wandmalfarbe/pandoc-latex-template#required-latex-packages
[eisvogel-listings]: https://github.com/Wandmalfarbe/pandoc-latex-template#syntax-highlighting-with-listings
[pandoc-highlights]: https://pandoc.org/MANUAL.html#syntax-highlighting