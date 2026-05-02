# Report Build Guide

This folder contains the LaTeX source for the Computer Vision report.

## Project Structure

- `main.tex`: entry point of the report.
- `preamble.tex`: shared packages and page setup.
- `conver_page.tex`: cover page.
- `thankyou.tex`: acknowledgment page.
- `abstract.tex`: abstract page.
- `chapters/`: chapter sources and appendix.
- `images/`: figures used by the report.
- `thesis.bib`: bibliography database.

## How to Build

### Option 1: If `latexmk` is available on PATH

Run this inside the `report` folder:

```powershell
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

### Option 2: Use MiKTeX directly on Windows

If `latexmk` or `pdflatex` is not on PATH, run the executable directly:

```powershell
& "C:\Users\caoha\AppData\Local\Programs\MiKTeX\miktex\bin\x64\pdflatex.exe" -interaction=nonstopmode -halt-on-error main.tex
```

If the bibliography contains citations, run these commands in order:

```powershell
& "C:\Users\caoha\AppData\Local\Programs\MiKTeX\miktex\bin\x64\pdflatex.exe" -interaction=nonstopmode -halt-on-error main.tex
& "C:\Users\caoha\AppData\Local\Programs\MiKTeX\miktex\bin\x64\biber.exe" main
& "C:\Users\caoha\AppData\Local\Programs\MiKTeX\miktex\bin\x64\pdflatex.exe" -interaction=nonstopmode -halt-on-error main.tex
& "C:\Users\caoha\AppData\Local\Programs\MiKTeX\miktex\bin\x64\pdflatex.exe" -interaction=nonstopmode -halt-on-error main.tex
```

## Output

The compiled PDF will be generated as `main.pdf` in this folder.

## Cleaning Build Files

To remove temporary LaTeX files, delete the generated files such as:

- `main.aux`
- `main.bbl`
- `main.bcf`
- `main.lof`
- `main.log`
- `main.lot`
- `main.out`
- `main.run.xml`
- `main.toc`
- `main.pdf`
