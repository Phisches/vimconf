# vimconf

## Some articels here:

- https://www.redhat.com/sysadmin/five-vim-plugins
- https://opensource.com/article/19/1/vim-plugins-developers
- https://www.fullstackpython.com/vim.html
- https://medium.com/nerd-for-tech/vim-as-an-ide-for-python-2021-f922da6d2cfe
- https://realpython.com/vim-and-python-a-match-made-in-heaven/


## create vim plugin dir
```
mkdir -p ~/.vim/pack/git-plugins/start
```

The -p flag will create nested directories, but only if they don't exist already.


## Linting 
https://github.com/dense-analysis/ale

```bash
git clone --depth 1 https://github.com/dense-analysis/ale.git ~/.vim/pack/git-plugins/start/ale
```

```bash
vim ~/.vimrc
```

```
" Enable completion where available.
" This setting must be set before ALE is loaded.
"
" You should not turn this setting on if you wish to use ALE as a completion
" source for other completion plugins, like Deoplete.
let g:ale_completion_enabled = 1
let g:ale_linters = {
\   'python': ['flake8', 'mypy', 'pylsp'],
\}
```


## Autocomplete
pip install python-language-server
https://github.com/davidhalter/jedi-vim

 ```
 git clone --depth=1  https://github.com/davidhalter/jedi-vim.git ~/.vim/pack/git-plugins/start/jedi-vim
 ```
 
 ## Statusbar
 
 https://github.com/vim-airline/vim-airline
 
 ```
 git clone https://github.com/vim-airline/vim-airline ~/.vim/pack/dist/start/vim-airline
 ```
 
 Remember to run :helptags ~/.vim/pack/dist/start/vim-airline/doc to generate help tags
 
 ## Tagbar
 
 https://github.com/preservim/tagbar
 
 Requires an installation of Universal CTAGS. Eg. via apt:
 ```
 sudo apt install universal-ctags 
 ```
 
 ```
  git clone https://github.com/preservim/tagbar ~/.vim/pack/dist/start/tagbar
 ```
 
 How to use it: https://www.pavedroad.io/part-4-code-navigation-with-tagbar/
