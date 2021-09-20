# vim colemak-DHm
 
This **fork of a fork** is kind of *usable*. It works as intended, it just needs more remaps to do. But anyways, remaps are **not** included in the plugin and have to be written in config as `g:colemak_dhm_mappings` (see below).

## Simple setup

Define this in the vimrc runtime stream prior to plugin loading (plugins run after vimrc by default)
```vim
" Need to define prior to plugin load or include in plugin
" Defined here first so can get mappings for downstream vimrc
let g:colemak_dhm_mappings = {
\        'left': {'dhm': 'm', 'original': 'h'},
\        'right': {'dhm': 'i', 'original': 'l'},
\        'down': {'dhm': 'n', 'original': 'j'},
\        'up': {'dhm': 'e', 'original': 'k'},
\        'insert': {'dhm': 'u', 'original': 'i'},
\        'undo': {'dhm': 'l', 'original': 'u'},
\        'next': {'dhm': 'k', 'original': 'n'},
\        'previous': {'dhm': 'K', 'original': 'N'},
\        'mark': {'dhm': 'm', 'original': 'm'},
\        'top_screen': {'dhm': 'M', 'original': 'H'},
\        'join': {'dhm': 'N', 'original': 'J'},
\        'shift_i': {'dhm': 'I', 'original': '<nop>'},
\}
```

# Install


1. Use [vim-plug](https://github.com/manning390/vim-plug).
2. Add to `.vimrc`: `Plug 'fiplox/vim-colemak-DHm'`
3. Run `vim +PlugInstall`
4. You probably want to load vim-colemak last.

# Licence

Distributed under the same terms as Vim itself. See `:help license`.
