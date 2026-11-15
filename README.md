# CV

I've lost my CV 3 times. I've uploaded again to avoid starting from scratch again. Its based on the template [Medium Length Professional CV](https://www.latextemplates.com/template/medium-length-professional-cv)

## Files

| Source    | Output      | Language    |
|-----------|-------------|-------------|
| `cv.tex`  | `cv.pdf`    | English     |
| `cv-es.tex` | `cv-es.pdf` | Castellano  |

Both documents share the layout in `resume.cls`. The content is duplicated on purpose, so any change to a section has to be applied to both files.

## Build

```sh
latexmk -pdf cv.tex cv-es.tex
```

`cv-es.tex` uses `babel` with Spanish hyphenation patterns when `spanish.ldf` is installed; otherwise it disables hyphenation so Spanish words are not split following English rules.
