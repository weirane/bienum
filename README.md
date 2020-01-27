# `bienum`: a double column sub-enumerate environment
Usage:

```tex
% In preamble:
% \input{bienum.tex}

\begin{enumerate}
  \item blah blah
    \begin{bienum}[<left-move length>]
      \itemxx{item}{item}
      \itemx{single line item}
      \itemxx{item}{item}
    \end{bienum}
\end{enumerate}
```

which will render:

```text
1. blah blah
   (1) item                    (2) item
   (3) single line item
   (4) item                    (5) item
```

the optional argument is the length for which the right column moves left.
