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

## Package Listing

### Automatically loaded packages in `start/`

| Package                 | Description                                       |
|-------------------------|---------------------------------------------------|
| ZoomWin                 | Toggle fullscreen for the current window          |
| org.vim                 | Edit org-mode files                               |
| vim-colorpack           | Select from modern colorschemes                   |
| vim-commentary          | Toggle code comments                              |
| vim-dispatch            | Run programs asynchronously in your terminal      |
| vim-endwise             | Automatically end code blocks                     |
| vim-fugitive            | Interface with Git                                |
| vim-helm                | Edit Helm templates                               |
| vim-jq                  | Edit jq scripts                                   |
| vim-lion                | Align text by some character                      |
| vim-markdown            | Edit markdown documentation                       |
| vim-matchit             | Jump between more begin/end tokens with `%`       |
| vim-mustache-handlebars | Edit Mustache and Handlebars templates            |
| vim-ragtag              | Conveniently edit `<tag>` structures in code      |
| vim-repeat              | Repeat more commands with `.`                     |
| vim-surround            | Work with text objects defined by surroundings    |
| vim-terraform           | Edit and run Terraform                            |
| vim-toml                | Edit TOML config files                            |
| vim-unimpaired          | Perform clunky/common operations with ease        |

### Manually loaded packages in `opt/`

| Package                 | Description                                       |
|-------------------------|---------------------------------------------------|
| aspnetide.vim           | Edit and run ASP.NET code                         |
| nerdtree                | Explore a filesystem tree in a sidebar            |
| syntastic               | Run code linters                                  |
| taboo.vim               | Easily format and rename tabs                     |
| tagbar                  | Navigate ctags in a sidebar                       |
| vbnet.vim               | Edit VB.NET code                                  |
| vim-abolish             | Work with variations in casing and congugation    |
| vim-bookmarks           | Bookmark and annotate lines of files              |
| vim-characterize        | View extended character representations with `ga` |
| vim-flagship            | Display a global status/tag line                  |
| vim-obsession           | Automatically save and load sessions              |
| vim-sleuth              | Automatically set `shiftwidth` and `expandtab`    |
| vim-speeddating         | Conveniently work with timestamps                 |
| vim-table-mode          | Insert and edit tables                            |
