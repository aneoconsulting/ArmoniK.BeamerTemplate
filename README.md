# LaTeX Beamer template for ArmoniK presentations

This repository contains a beamer template with a custom ANEO inspired theme.

## Requirements

- LaTeX distribution (e.g.; TeX Live)
- lualatex to be able to use the Poppins and Lexend Deca fonts
- `latexmk` for smarter compilation

## Usage

The example directory provides a sample presentation using the custom theme. The directoy contains two files: the  `.tex` file defining the slides itself and a `.latexmkrc` with the configuration so `latexmk` is able to compile it. The `.latexmkrc` file prepends the two
environment variables:

 - `TEXINPUTS` with the path of our custom beamer theme.
 - `OSFONTDIR` with the path of the fonts used by the theme.

If you wish to start a new presentation a copy of the example directory is a good startingpoint, you may create it in at the same level as the example directory, in which case the copied `.latexmkrc` file should have the correct settings for `latexmk` to compile your presentation. If you choose to create a new presentation in a different arbitrary location, you will need t
adapt the value of `$theme_dir;` to point to the location of the custom theme.
