# Vim Packages

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
