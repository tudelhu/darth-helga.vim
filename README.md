# vim-hybrid-material
Material color scheme for Vim based on [kristijanhusak/vim-hybrid-material](https://github.com/kristijanhusak/vim-hybrid-material) and [flrnd/plastic.vim](https://github.com/flrnd/plastic.vim) color scheme.

### Installation
*  [Pathogen](https://github.com/tpope/vim-pathogen)
  *  `git clone https://github.com/tudelhu/darth-helga.vim ~/.vim/bundle/darth-helga.vim`
  *  Remember to run `:Helptags` to generate help tags
*  [NeoBundle](https://github.com/Shougo/neobundle.vim)
  *  `NeoBundle 'tudelhu/darth-helga.vim'`
*  [Vundle](https://github.com/gmarik/vundle)
  *  `Plugin 'tudelhu/darth-helga.vim'`
*  [Plug](https://github.com/junegunn/vim-plug)
  *  `Plug 'tudelhu/darth-helga.vim'`
*  manual
  *  copy all of the files from `colors` directory into your `~/.vim/colors` directory

### Options

If you would like some of the code to be bolded, like functions and language controls, add this option to vimrc:

```vimL
let g:enable_bold_font = 1
```

If you want comments to be in italic, also add this:
```vimL
let g:enable_italic_font = 1
```

To use transparent background, add this option:
```vimL
let g:hybrid_transparent_background = 1
```

**Note**: Options must be set before `colorscheme hybrid_material` statement.

#### Darth Helga

Add screenshot

True colors are a requirement for this color scheme to work properly. To enable this, place the following in your `~/.vimrc` or `~/.config/nvim/init.vim` file:

```vim
if (has("nvim"))
  "For Neovim 0.1.3 and 0.1.4 < https://github.com/neovim/neovim/pull/2198 >
  let $NVIM_TUI_ENABLE_TRUE_COLOR=1
endif

"For Neovim > 0.1.5 and Vim > patch 7.4.1799 < https://github.com/vim/vim/commit/61be73bb0f965a895bfb064ea3e55476ac175162 >
"Based on Vim patch 7.4.1770 (`guicolors` option) < https://github.com/vim/vim/commit/8a633e3427b47286869aa4b96f2bfc1fe65b25cd >
" < https://github.com/neovim/neovim/wiki/Following-HEAD#20160511 >
if (has("termguicolors"))
  set termguicolors
endif
```

##### GVim/MacVim
Only add this to .vimrc after installation:

```vimL
set background=dark
colorscheme darth_helga
```

### Thanks to
* [kristijanhusak/vim-hybrid-material](https://github.com/kristijanhusak/vim-hybrid-material)
* [flrnd/plastic.vim](https://github.com/flrnd/plastic.vim)
