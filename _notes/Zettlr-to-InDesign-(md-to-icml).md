---
title: Zettlr to InDesign
---

## Problem
Zettlr does not provide direct export to InCopy `.icml` (yet), but we want to export all references and the bibliography properly without using `.docx` which cannot automatically update.

## Solution
1. Export `.md` from **zettlr** to `.tex` 
2. convert the `.tex` to `.icml` using **pandoc** in the command line: `$ pandoc -s -f latex -t icml -o master-text.icml master-text.tex`
3. place the _InCopy_ file in a text frame in InDesign.

### Corrections 
Correct spelling mistakes, line breaks, double spaces etc. in the `master-text.md`. Then, repeat steps one and two and refresh the `.icml` in the InDesign _links_ pane to update.


## Automation
`input.md` → `output.icml` 

### Prerequisite
`bibliography` (BibTeX-json file) and `csl` (= citation style specification file) paths are set in the YAML header of your `input.md`, like this:
```JSON
---
bibliography: path/to/mybib.json
csl: path/to/chicago-autor-date.csl
---
# markdown h1
your file's content ...
```
### Script

Run this script in your working directory to automate the file conversions.

```bash
pandoc input.md -f markdown -t latex --citeproc -s --pdf-engine=xelatex --mathjax -o workingfile.tex
echo "md to latex done ..."
pandoc -s -f latex -t icml -o output.icml workingfile.tex
echo "... latex to icml done"
pause
```

Now the content can be updated in InDesign:

![](media/2021-05-11-00-22-23.png)

### Run on Windows

Open a text editor, paste the script and save it as `md-icml-script.bat` - you can run it by opening the file or by navigating to the directory in the command line and typing `& ".\md-icml-script.bat"`.


