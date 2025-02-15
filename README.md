# devdocs

Document generation and templates.

# Capabilities

- Generate a LaTeX PDF with JDF

## JDF

Generate a PDF document from LaTeX that uses the Joyner Document Format (JDF).
```
make
```

The unnecessary files can be removed with `make clean`.
All generated files can be removed (including the document) with `make clean doc=true`.

# LaTeX

Templates that are `.tex` files require installing LaTeX.
This includes XeLaTeX for font handling and latexmk for the Makefile.

This tool is developed with macOS, where LaTeX can be installed using Homebrew.
Information about Homebrew, as well as the installation instructions are available
through [Homebrew documentation](https://brew.sh). To install LaTeX, open the terminal
and use the following command:
```
brew install --cask mactex
```

After the installation, restart the terminal and check for the LaTeX installation.
This is performed with the following code in the terminal:
```
latex --version
```

