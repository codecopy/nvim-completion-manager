
# Complete Manager for neovim 

This is my experimental completion framework for neovim, which offers great
flexibility for writing your own completion source, including async support.

There's no guarantee that this plugin will be compatible with other completion
plugin in the same buffer. Use `let g:cm_enable_for_all=0` and `call
cm#enable_for_buffer()` to use this plugin for specific buffer.


## Requirements

- neovim python3 support. `:help provider-python`. For lazy linux users, I
  recommend this plugin
  [python-support.nvim](https://github.com/roxma/python-support.nvim).
  (Note: Self promotion)

## How to extend this framework?

see [autoload/cm/sources/ultisnips.vim](autoload/cm/sources/ultisnips.vim)

```vim

    "  don't give |ins-completion-menu| messages.  For example,
	"	'-- XXX completion (YYY)', 'match 1 of 2', 'The only match',
    set shortmess+=c

```

## Todo:

- documentation

## Done:

- simply bufkeyword code
- jedi support markdown
- simplify plugin framework
