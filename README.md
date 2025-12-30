# listingsextra.sty

Additional language definitions for the LaTeX [listings](https://ctan.org/pkg/listings) package.

## Overview

This package extends the `listings` package with language definitions that are not included in the standard distribution. It provides proper syntax highlighting for modern programming languages.

## Supported Languages

- **js** - JavaScript with ES6+ keywords, built-in objects, and literals
- **fundamental** - Empty language definition for plain text

## Installation

Copy `listingsextra.sty` to your LaTeX project directory, or install it in your local texmf tree:

```
~/texmf/tex/latex/listingsextra/listingsextra.sty
```

Then run `texhash` if installed system-wide.

## Usage

```latex
\documentclass{article}
\usepackage{listings}
\usepackage{listingsextra}

\begin{document}

\begin{lstlisting}[language=js]
const greeting = async (name) => {
  return `Hello, ${name}!`;
};
\end{lstlisting}

\end{document}
```

## Requirements

- LaTeX2e
- listings package

## License

GPL-3.0. See [LICENSE](LICENSE) for details.
