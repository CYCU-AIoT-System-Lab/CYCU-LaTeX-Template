# CYCU-LaTeX-Template

## Description

| Directory                            | Description                                           |
| ---------                            | -----------                                           |
| [./figure](./figure)                 | Figure embedded in template.                          |
| [./latex-template](./latex-template) | Template Minimal Working Example (MWE) with examples. |
| [./script](./script)                 | Program embedded in template.                         |

## Entry Point

[./latex-template](./latex-template) follows the same pipeline. The main PDF file `main.pdf` is created with the main entry point `main.tex`. In order to add book spine on the cover page, the second entry point `main2.tex` is used to generate `main2.pdf`. However, the `main2.pdf` does not have any of the hyperlink originally presented in `main.pdf` with this approach.

## Environment and Compilation

No matter which distribution or platform, you need to make sure there is the option "XeLaTeX" available for this template to compile.

1. **Windows**: use [MikTeX](https://miktex.org/) which not only prepare the executables and also maintain/update various packages.
2. **Linux**: try [TeX Live](https://www.tug.org/texlive/).
3. **MacTeX**: try [MacTeX](https://www.tug.org/mactex/mainpage2024.html).
4. **Online**: try [Overleaf](https://www.overleaf.com/).

If these options does not work, try finding your suitable option on [The LaTeX Project](https://www.latex-project.org/get/).

Note that this template is only tested with **MikTeX** and are tested with the following commands from [belongtothenight/powershell_scripts/process_tex](https://github.com/belongtothenight/powershell_scripts/tree/main/process_tex): (XeLaTeX must be used to compile)

```
process_tex -fn .\main.tex && process_tex -fn .\main2.tex
```
