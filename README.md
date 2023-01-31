# vimconf

## Some articels here:

- https://www.redhat.com/sysadmin/five-vim-plugins
- https://opensource.com/article/19/1/vim-plugins-developers
- https://www.fullstackpython.com/vim.html
- https://medium.com/nerd-for-tech/vim-as-an-ide-for-python-2021-f922da6d2cfe


## create vim plugin dir
```
mkdir -p ~/.vim/pack/git-plugins/start
```

The -p flag will create nested directories, but only if they don't exist already.


## Linting 
https://github.com/dense-analysis/ale

```
git clone --depth 1 https://github.com/dense-analysis/ale.git ~/.vim/pack/git-plugins/start/ale
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
