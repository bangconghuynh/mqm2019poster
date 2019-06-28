# mqm2019poster
Poster title: *Exploiting Multiple Symmetry-Broken SCF Solutions to Describe Ground and Excited States of Transition-Metal Complexes*

Poster presented at MQM 2019 in Heidelberg, Germany.

## Compilation
The required packages and libraries should be obvious from the preamble. But in particular:
  * `lualatex` with `-shell-escape` and ` PGFPLOTS 1.16` are required to compile the main TeX document and the `TikZ` and `PGFPLOTS` figures, especially since the very new `luamath` library is used to perform some axis scaling;
  * `biber` is required to compile the References (not that there are a lot of complicated references in this poster, but it's nice to use something that offers a bit more control and better handling of any potential complicated stuff).
 
`texlive 2019` as-is should contain all of the required packages and libraries. The latest packages updated via `MiKTeX` by June 2019 should do the job too.

Note that `tikzexternalize` is used in this document to generate the aforementioned figures. All figures have thus been precompiled, so if one wants to avoid recompiling them, please make sure that the boolean `\tikzex` is set to `false`, i.e., comment `\tikzextrue` and uncomment `\tikzexfalse` in the preamble:
```
%\tikzextrue
\tikzexfalse
```

## Acknowledgement
The theme used in this poster is based on the Gemini theme which can be found [here](https://github.com/anishathalye/gemini).
