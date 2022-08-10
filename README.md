# Vim Packages

## Usage

Recursively clone this repo to `~/.vim/pack/foo`, where `foo` is literally any
name. The following commands should do that for you:

``` sh
mkdir -p ~/.vim/pack
cd ~/.vim/pack
git clone --recurse-submodules git@github.com:eeowaa/vim-plugins.git
```

Packages that live in `start/` are automatically loaded. Packages that live in
`opt/` must be loaded with `:packadd packagename`.

Reference: <https://shapeshed.com/vim-packages/>.

## Package Maintenance

The `.bin` directory contains two interactive shell scripts (neither one
accepts command-line arguments):

- `add`: Add a vim package as a submodule
- `update`: Update git submodules for vim packages

If you have `direnv` installed, the `.bin` directory will automatically be
added to your `$PATH` when the current working directory is within this git
repository, so you can directly execute the `add` or `update` commands.
