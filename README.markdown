[vim colemak DHm](vim-colemak-DHm)
===========

=======
# This is a **work in progress** fork of a fork, check back later. When this text is removed, it is ready for use.

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
\        'next': {'dhm': 'h', 'original': 'n'},
\        'previous': {'dhm': 'H', 'original': 'N'},
\        'mark': {'dhm': 'k', 'original': 'm'},
\        'top_screen': {'dhm': 'K', 'original': 'H'},
\        'join': {'dhm': 'N', 'original': 'J'},
\        'shift_i': {'dhm': 'I', 'original': '<nop>'}
\}

Install
-------

1. Use [vim-plug](https://github.com/manning390/vim-plug).
2. Add to `.vimrc`: `Plug 'manning390/vim-colemak-DHm'`
3. Run `vim +PlugInstall`
4. You probably want to load vim-colemak last. Reload the plugin at the bottom of your Vim configuration.

    ```
    " Reload vim-colemak to remap any overridden keys
    silent! source "$HOME/.vim/bundle/vim-colemak/plugin/colemak-dhm.vim"
    ```

    *Note: You might be using `~/.vim/plugged`.*

