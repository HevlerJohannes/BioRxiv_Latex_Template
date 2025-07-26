# LaTeX code to produce BioRxiv style preprint using VS Code

## Acknowledgements

This LaTeX template is based on the [zHenriquesLab-StyleBioRxiv.cls]([https://github.com/HenriquesLab/LaTeX-template-bioRxiv](https://www.overleaf.com/latex/templates/henriqueslab-biorxiv-template/nyprsybwffws)) originally developed by Ricardo Henriques.  

It has been slightly modified to suit my personal preferences.

All original credit goes to the author.

## Why running LaTeX locally
Latex needs to be installed locally, as online resources just like Overleaf cannot compile the full thesis (a thesis with ~ 300 pages takes about 2 min to compile (depending your machine of course), while Overleaf (with the University account) crashes after ~ 1 min).

## Requirements
* VS Code e.g. via the Software Center
* LaTeX; use TeX Live and install as described in [Requirements](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install#requirements).
* Optional: Git; install as described in [Getting Started with Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). With this you can keep track of the changes over time and easily revert back if something is broken.

## VS Code Installation of LaTeX and other helpful addons
Open the folder containing the LaTeX code in VScode as follows:
* File --> Open Folder --> Choose the correct folder.
* When opening the folder for the first time, VScode will give you recommendations what to install via a pop-up window in the lowe right corner. If this is not the case, you can find the needed packages in [.vscode/extensions.json](.vscode/extensions.json).

## Compile pdf
Compile in terminal by running the following:

```bash
pdflatex Article.tex
```
If bibliography is not correctly compiled run the following:

```bash
pdflatex Article.tex
bibtex Article
pdflatex Article.tex
pdflatex Article.tex
```
