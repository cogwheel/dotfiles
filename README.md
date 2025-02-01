# Cogwheel's Dotfiles

## Prereqs

A recent (late 2024) version of GNU stow. You may have to build this yourself.
In old versions the `dot-foo` -> `.foo` renaming will fail.

## Usage

1. Clone this recursively somewhere in your `$HOME` directory (e.g. `~/.dotfiles`).
2. `cd` into that directory
3. run `stow -Sv --dotfiles -n` on each of the subdirectories to see what will be linked and check for issues
4. Remove the `-n` from the command after addressing any issues

## Tips

- If you don't use `stow` for anything else, put `alias stow='/path/to/stow --dotfiles'` in your shell rc file.

## TODO

### Starship

- [X] Bug: environment modules (ssh, etc) appear after `$character`
