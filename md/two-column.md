---
title: This is a title
author: Author's information 
date: YYYY-MM-DD
header-includes: |
    \usepackage{fancyhdr}
    \pagestyle{fancy}
    \fancyhead[CO,CE]{This is a header}
    \fancyfoot[CO,CE]{\textit{This is a footer}}
    \fancyfoot[LE,RO]{\thepage}
# Disable this option for a single column layout.
classoption:
  - twocolumn
papersize: a4
fontsize: 12pt
colorlinks: true
geometry: margin=2.5cm
output: pdf_document
---

## Markdown Two Column (or One) Paper Template

Use `pandoc` to transpile to `PDF`:

```sh
#!/bin/sh
pandoc paper.md --pdf-engine=pdflatex     \
                --highlight-style=haddock \
                -o exp.pdf
```
