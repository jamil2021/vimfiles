set nocompatible              " required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim

" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

call vundle#begin()

" let Vundle manage Vundle, required
Plugin 'gmarik/Vundle.vim'

" Add all your plugins here (note older versions of Vundle used Bundle instead of Plugin)
" Vim plugin providing simple, correct folding for Python
Plugin 'tmhedberg/SimpylFold'
" jedi-vim - awesome Python autocompletion with VIM
Plugin 'davidhalter/jedi-vim'
" Perform all your vim insert mode completions with Tab
Plugin 'ervandew/supertab'
" An alternative indentation script for python
Plugin 'vim-scripts/indentpython.vim'
" YouCompleteMe: a code-completion engine for Vim
"Bundle 'Valloric/YouCompleteMe'
" Syntastic is a syntax checking plugin for Vim 
Plugin 'scrooloose/syntastic'
" Flake8-vim is a Vim plugin that checks python sources for errors.
" It's based on pylint-mode plugin by Kirill Klenov.
Plugin 'nvie/vim-flake8'
"Color Schemes:
"
" A dark GitHub theme for Vim and NeoVim.
Plugin  'wojciechkepka/vim-github-dark' 
" Low contrast colour scheme for low light conditions
Plugin 'jnurmine/Zenburn'
" mirror of the vim colors from http://ethanschoonover.com/solarized 
Plugin 'altercation/vim-colors-solarized'
" Collection of awesome color schemes for Vim, merged for quick use.
Plugin 'flazz/vim-colorschemes'
"
" The NERD tree allows you to explore your filesystem
" and to open files and directories.
Plugin 'scrooloose/nerdtree'
" This plugin aims at making NERDTree feel like a true panel,
" independent of tabs.
Plugin 'jistr/vim-nerdtree-tabs'
" In contrast to a file tree, CtrlP is a fuzzy file finder. As the name
" implies, the plugin will try to find files for you so that you can work on
" them.
Plugin 'kien/ctrlp.vim'
" Fugitive is the premier Vim plugin for Git
Plugin 'tpope/vim-fugitive'
" Powerline is a statusline plugin for vim, and provides statuslines and
" prompts for several other applications, including zsh, bash, fish, tmux,
" IPython, Awesome, i3 and Qtile.
Plugin 'Lokaltog/powerline', {'rtp': 'powerline/bindings/vim/'}
" Insert or delete brackets, parens, quotes in pair. 
Plugin 'jiangmiao/auto-pairs'
" Highlight matching parenthesis(), brackets[], and braces{}
Plugin 'frazrepo/vim-rainbow'
" A light and configurable statusline/tabline plugin for Vim
Plugin 'itchyny/lightline.vim'
" Comment functions so powerful—no comment necessary
Plugin 'preservim/nerdcommenter'
" Run your favorite search tool from Vim, with an enhanced results list
" ack can be used as a replacement for 99% of the uses of grep
Plugin 'mileszs/ack.vim'
" List the current file's tags in a sidebar, ordered by class etc
Plugin 'preservim/tagbar'

call vundle#end()            " required


" Vim Splits
set splitbelow
set splitright

"split navigations
nnoremap <C-J> <C-W><C-J>
nnoremap <C-K> <C-W><C-K>
nnoremap <C-L> <C-W><C-L>
nnoremap <C-H> <C-W><C-H>

" Enable Folding
set foldmethod=indent
set foldlevel=99

" Enable folding with the spacebar
" Opens and closes folds with Space bar
" nnoremap <space> za

" SimplyFold Settings
" to enable docstring preview in fold text
let g:SimpylFold_docstring_preview=1


"Jedi-vim settings
let g:jedi#force_py_version = 3
let g:jedi#auto_initialization = 1
" disable jedi-vim autocompletion
let g:jedi#completions_enabled = 0
let g:jedi#auto_vim_configuration = 0
let g:jedi#smart_auto_mappings = 0
let g:jedi#popup_on_dot = 0
let g:jedi#completions_command = ""
let g:jedi#show_call_signatures = "1"
let g:jedi#show_call_signatures_delay = 0
let g:jedi#use_tabs_not_buffers = 0
let g:jedi#show_call_signatures_modes = 'i'  " ni = also in normal mode
let g:jedi#enable_speed_debugging=0

" match BadWhitespace /\s\+$/
" set ttimeout        " time out for key codes
" set ttimeoutlen=100 " wait up to 100ms after Esc for special key
set ttimeoutlen=5

filetype plugin indent on    " required
"au BufNewFile,BufRead *.py
set tabstop=4
set softtabstop=4
set shiftwidth=4
set textwidth=79
set expandtab
set autoindent
set fileformat=unix
set clipboard=unnamedplus

set encoding=utf-8
set nu
let python_highlight_all=1
syntax on

" To display the status line always, set the following option in your vimrc:
" :set laststatus=2
" The advantage of having the status line displayed always is, you can see the current mode,
" file name, file status, ruler, etc. 
set laststatus=2

" To enable 256 colors in vim, put this your .vimrc before setting the colorscheme:
" set t_Co=256
if !has('gui_running')
  set t_Co=256
endif


" YouCompleteMe settings (not using at the moment, using jedi instead)
" let g:ycm_server_python_interpreter = '/usr/bin/python3'
" let g:ycm_autoclose_preview_window_after_completion=1
" map <leader>g  :YcmCompleter GoToDefinitionElseDeclaration<CR>
"disable youcompleteme at startup
" let g:ycm_filetype_specific_completion_to_disable = {'*': 1}


"python with virtualenv support
"py << EOF
"import os
"import sys
"if 'VIRTUAL_ENV' in os.environ:
"  project_base_dir = os.environ['VIRTUAL_ENV']
"  activate_this = os.path.join(project_base_dir, 'bin/activate_this.py')
"  execfile(activate_this, dict(__file__=activate_this))
"EOF


" if has('gui_running')
"    set background=dark
"    colorscheme solarized
" else
"    colorscheme zenburn
" endif

"call togglebg#map("<F5>")

" NERDTree settings
let NERDTreeIgnore=['\.pyc$', '\~$'] "ignore files in NERDTree
" Set a language to use its alternate delimiters by default
let g:NERDAltDelims_java = 1

"set auto-pairs options
let g:AutoPairsFlyMode = 1
let g:AutoPairsShortcutBackInsert = '<M-b>'
let g:rainbow_active = 1

" colorschemes/favorite color themes
"colorscheme wombat
"colorscheme molokai
"colorscheme abyss
"colorscheme solarized8_dark_low 
"colorscheme solarized8_light_high
set background=dark
"colorscheme hybrid
colorscheme gruvbox

"lightline settings
"put a bar at the bottom of the screen to show you what file you are working
"on, where you are in the file, what type of file it is, etc. Each of these
"plugins has advantages and disadvantages, and after briefly weighing them, I
"chose lightline. It's relatively small, easy to set up, quite extensible if
"you are into that kind of thing, and doesn't require any other tooling or
"plugins.
let g:lightline = {
      \ 'colorscheme': 'wombat',
      \ 'active': {
      \   'left': [ [ 'mode', 'paste' ],
      \             [ 'readonly', 'filename', 'modified', 'charvaluehex' ] ]
      \ },
      \ 'component': {
      \   'charvaluehex': '0x%B'
      \ },
      \ }

" Configuring `set noshowmode` stop displaying the Vim's default mode information
set noshowmode

" Tagbar settings
"Tagbar is a Vim plugin that provides an easy way to browse
"the tags of the current file and get an overview of its structure
nmap <F8> :TagbarToggle<CR>
