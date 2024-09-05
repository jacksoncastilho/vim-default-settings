# vim-default-settings

Criar na home o arquivo .vimrc e colar o script a seguir:

```
set expandtab                    
" espacos em branco em vez de tabulacao "
set tabstop=4
" Numero de espacos para a tabulacao "
set shiftwidth=4
" Espacos usados para operacao de recuo automatico "
set autoindent
" Identacao automatica "
set smartindent
" Identacao inteligente para linguagem de programacao "
set cursorline
" linha sob cursor atual "
set number
" Ativa a enumeracao "
set undofile
" Funcao desfazer persistencia "
if !isdirectory(expand("$HOME/.vim/undodir"))
    call mkdir(expand("$HOME/.vim/undodir"),"p")
endif
set undodir=$HOME/.vim/undodir
```
