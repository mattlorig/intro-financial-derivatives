# Contributing

Thank you for helping improve these notes. Contributions of every size are welcome, from a one-character typo fix to a new chapter. Accepted contributors are listed in the preface.

## Ways to contribute

### Report an error

Open an [issue](https://github.com/mattlorig/intro-financial-derivatives/issues/new). Include:

- where the error is (chapter, page number in the PDF, or equation/exercise number),
- what it says now, and
- what you think it should say.

You do not need to know Git or LaTeX to do this.

### Fix a small error yourself

You can do this entirely in your browser:

1. Open the `.tex` file on GitHub and click the pencil icon (**Edit this file**).
2. GitHub will ask you to fork the repository. Accept.
3. Make your change, then click **Commit changes** and **Propose changes**.
4. On the next page, click **Create pull request** and briefly describe the fix.

### Add new material

New exercises, solutions, figures, examples, sections or chapters are all welcome. For anything larger than a few paragraphs, please open an issue first describing what you plan to add, so we can agree on where it fits before you put in the work.

1. Fork the repository and clone your fork.
2. Make your changes to the `.tex` file.
3. Compile with `pdflatex` (run it twice) and check that there are no errors and that your material looks right in the PDF.
4. Open a pull request with a short description of what you added.

Issues labeled [good first issue](https://github.com/mattlorig/intro-financial-derivatives/labels/good%20first%20issue) are a good place to start.

## Conventions

Please follow the conventions already used in the notes so that the source stays consistent.

**The file must compile on its own.** No external image files, `.bib` files or custom packages. In particular:

- Draw figures with TikZ or pgfplots inside the `.tex` file. Do not use `\includegraphics`.
- Add references to the `thebibliography` environment at the end of the file, using natbib author-year keys, e.g. `\bibitem[Heston(1993)]{heston1993}`.

**Use the existing macros.** For example:

| Write | Not |
| --- | --- |
| `\Eb`, `\Ebt` | `\mathbb{E}`, `\widetilde{\mathbb{E}}` |
| `\Pb`, `\Qb`, `\Rb` | `\mathbb{P}`, `\mathbb{Q}`, `\mathbb{R}` |
| `\dd t`, `\dd W_t` | `dt`, `dW_t` |
| `\ee^{x}` | `e^{x}` |
| `\sig`, `\lam`, `\Del`, `\gam` | `\sigma`, `\lambda`, `\Delta`, `\gamma` |

The full list of macros is in the preamble.

**Exercises and solutions.** Exercises go in the `Exercises` section at the end of each chapter:

```latex
\begin{exercise}
\label{exer:5-10}
Statement of the exercise.
\end{exercise}
```

If you add a solution, put it in the `Solutions to Exercises` chapter in the matching place:

```latex
\subsection*{Solution to Exercise \ref{exer:5-10}}
Solution.
```

An exercise without a solution is still a useful contribution.

**Labels.** Use descriptive, unique labels with a prefix: `eq:`, `thm:`, `def:`, `ex:`, `exer:`, `sec:`, `fig:`. Refer to equations with `\eqref`.

**Code.** Python code goes in a `lstlisting` environment with a caption giving the file name. Code should run as written with only NumPy, SciPy and Matplotlib.

**Spelling.** Use US spelling.

**Version number.** Please do not change the version number or file name. The maintainer does this when a new release is made.

## Original material only

Please contribute only material you wrote yourself, or material that is in the public domain or under a compatible open license (with attribution). Do not copy exercises, examples, text or figures from textbooks or papers. Mathematical ideas cannot be owned, so you are free to cover any standard result, but write the explanation, the exercise and the figure in your own words and your own way. If you adapted an idea from a specific source, cite it.

## License

By contributing, you agree that your contributions are licensed under the same terms as the rest of the notes: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) for text and figures, and additionally the MIT License for code listings. You keep the copyright to your contributions.

## Using the notes in your own course

Instructors are encouraged to fork the repository and adapt the notes for their own courses: cut chapters, add material, change notation. Under CC BY-SA, your version must credit the original, state that you changed it, and be released under the same license. If you make improvements that would help everyone, please consider sending them back as a pull request.
