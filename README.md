# An Introduction to Financial Derivatives — Open Lecture Notes

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23849183.svg)](https://doi.org/10.5281/zenodo.23849183)

Matthew Lorig, Department of Applied Mathematics, University of Washington

**[Download the PDF](https://github.com/mattlorig/intro-financial-derivatives/releases/latest)** from the latest release.

Open-source lecture notes on financial derivatives, originally developed for CFRM 504 at the University of Washington. Topics include forwards and futures, no-arbitrage bounds, the binomial model, the fundamental theorems of asset pricing, Brownian motion and Itô calculus, Black–Scholes, the Greeks, stochastic and local volatility, the Heston model, and barrier options. Each chapter ends with exercises; solutions are in the appendix.

## Building the PDF

The notes are a single LaTeX file with no external figures or bibliography files. All figures are drawn with TikZ/pgfplots.

```
pdflatex Lecture-Notes-CFRM-504-3.58.tex
pdflatex Lecture-Notes-CFRM-504-3.58.tex
```

Run it twice so cross-references resolve. Any recent TeX Live or MiKTeX distribution should work.

## Contributing

Corrections and additions are welcome.

- **Found an error?** Open an issue with the chapter, page or line number, and what you think it should say.
- **Want to add or improve something?** Fork the repository, make your change in the `.tex` file, check that it compiles, and open a pull request.

Contributors whose changes are accepted are listed in the preface.

## License

© 2026 Matthew Lorig. The notes are licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). You may share and adapt them for any purpose, provided you credit the original author, indicate what you changed, and release your version under the same license. Code listings in the notes are additionally released under the MIT License.

## Citation

M. Lorig, *An Introduction to Financial Derivatives: Open Lecture Notes*, version 3.58, 2026. https://doi.org/10.5281/zenodo.23849183
