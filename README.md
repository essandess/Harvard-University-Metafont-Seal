# Harvard University Metafont Seal
Harvard's seal in Metafont

![Harvard University Metafont Seal](https://github.com/essandess/Harvard-University-Metafont-Seal/blob/master/Harvard%20Seal%20metafont.png)

## Use

This Metafont code may be used to include the Harvard seal within TeX and LaTeX documents.

## Examples

### Metafont proof

The Metafont proof above was created using the TeXLive commands:

```
mktextfm gray ; mktextfm black
mf '\mode:=proof; mag:=360/2602; input harvard64.mf'
gftodvi harvard64.360gf
dvipdf harvard64.dvi
```

### TeX document

This TeX file produces the seal.

hlogo.tex
```
\nopagenumbers

\font\hseal=harvard64
\hbox{\hseal H}\bye
```

### Other documents

One [example](http://arxiv.org/pdf/1305.1886v1).
