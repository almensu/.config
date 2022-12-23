22222:

syntax on
set dictionary+=/usr/share/dict/words
set relativenumber

"leader key
let mapleader = " "

"very good command and useful with the d command
set relativenumber

"backup settings
set backupdir=$HOME/.config/nvim/tmp/backup,.
set directory=$HOME/.config/nvim/tmp/backup,.
set backup

"tab settings
set tabstop=4 "tabs expand to 4 spaces
set shiftwidth=4
set softtabstop=4
set expandtab

"stop auto commenting, this is hurtful more then it is useful
set formatoptions-=cro


"split settings so they are not stupid like defaults
set splitbelow splitright

"persistent undo between opening and closing
set undofile

"very useful for yaml files
autocmd Filetype yaml set cursorcolumn
autocmd Filetype yml set cursorcolumn

autocmd Filetype python set cursorcolumn

"smart search
set ignorecase
set smartcase

"search as characters are entered
set incsearch

"search as characters are entered
set formatoptions=qrn1

"search as characters are entered
"smart wrapping
set wrap
set textwidth=79
set formatoptions=qrn1

"Control the position of the new window
set splitright
set splitbelow

" ==================== Basic Mappings ====================
let mapleader=" "
noremap ; :
nnoremap Q :q<CR>
nnoremap S :w<CR>

map R :source $MYVIMRC<CR>
map Q :wq<CR>


call plug#begin('~/local/share/nvim/plugged')
" The default plugin directory will be as follows:
"   - Vim (Linux/macOS): '~/.vim/plugged'
"   - Vim (Windows): '~/vimfiles/plugged'
"   - Neovim (Linux/macOS/Windows): stdpath('data') . '/plugged'
" You can specify a custom plugin directory by passing it as the argument
"   - e.g. `call plug#begin('~/.vim/plugged')`
"   - Avoid using standard Vim directory names like 'plugin'

" Make sure you use single quotes

" Shorthand notation; fetches https://github.com/junegunn/vim-easy-align
Plug 'junegunn/vim-easy-align'

" Any valid git URL is allowed
Plug 'https://github.com/junegunn/vim-github-dashboard.git'

" Multiple Plug commands can be written in a single line using | separators
Plug 'SirVer/ultisnips' | Plug 'honza/vim-snippets'

" On-demand loading
Plug 'scrooloose/nerdtree', { 'on':  'NERDTreeToggle' }
Plug 'tpope/vim-fireplace', { 'for': 'clojure' }

" Using a non-default branch
Plug 'rdnetto/YCM-Generator', { 'branch': 'stable' }

" Using a tagged release; wildcard allowed (requires git 1.9.2 or above)
Plug 'fatih/vim-go', { 'tag': '*' }

" Plugin options
Plug 'nsf/gocode', { 'tag': 'v.20150303', 'rtp': 'vim' }

" Plugin outside ~/.vim/plugged with post-update hook
Plug 'junegunn/fzf', { 'dir': '~/.fzf', 'do': './install --all' }

" Unmanaged plugin (manually installed and updated)
Plug '~/my-prototype-plugin'

" Use release branch (recommend)
Plug 'neoclide/coc.nvim', {'branch': 'release'}

" color 
Plug 'EdenEast/nightfox.nvim'

" Initialize plugin system
" - Automatically executes `filetype plugin indent on` and `syntax enable`.
call plug#end()
" You can revert the settings after the call like so:
"   filetype indent off   " Disable file-type-specific indentation
"   syntax off            " Disable syntax highlighting

# coc.nvim
let g:coc_global_extensions = ['coc-json', 'coc-git']

" Use <c-space> to trigger completion
if has('nvim')
  inoremap <silent><expr> <c-space> coc#refresh()
else
  inoremap <silent><expr> <c-@> coc#refresh()
endif



