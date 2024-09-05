# vim-default-settings

Criar na home o arquivo .vimrc e colar o script a seguir:

set expandtab </br>
" espacos em branco em vez de tabulacao "</br>
set tabstop=4</br>
" Numero de espacos para a tabulacao "</br>
set shiftwidth=4</br>
" Espacos usados para operacao de recuo automatico "</br>
set autoindent</br>
" Identacao automatica "</br>
set smartindent</br>
" Identacao inteligente para linguagem de programacao "</br>
set cursorline</br>
" linha sob cursor atual "</br>
set number</br>
" Ativa a enumeracao "</br>
set undofile</br>
" Funcao desfazer persistencia "</br>
if !isdirectory(expand("$HOME/.vim/undodir"))</br>
    call mkdir(expand("$HOME/.vim/undodir"),"p")</br>
endif</br>
set undodir=$HOME/.vim/undodir
