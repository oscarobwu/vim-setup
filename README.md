# Vim

# Description
感謝 Wei Lee 的分享 這是由他哪邊提供出來的 
My vim plug-ins and settings in .vimrc.  
The snippets directory is for my custom snippets.

# Installation
1. Clone this repo and copy .vimrc to home directory

    ```sh
    git clone https://github.com/oscarobwu/vim-setup.git
    cd vim-setting 
    cp .vimrc ~/
    ```
2. Install `ag` and `fzf`


    ```sh
    apt install silversearcher-ag fzf -y
    ```
3. Start vi and it will automatically install `vim-plug` (package management for vim)  
It might display plenty of *error message* since there are settings for plug-in that not yet been installed.  
*You can simply ignore them*  
3. Restart vi and install packages  
Enter the command `:PlugInstall` in normal mode after you start vi  
4. Restart vi again  
5. Done!  
6. \(Optional\) Copy the snippets I define into snippets/  
    `cp snippets/* ~/.vim/bundle/vim-snippets/snippets/`

# What is in this vimrc? (Plug-in List)
### File management
- NERDTree  
    `<F2>`: Toogle NERDTree

### Snippets
- vim-snippets

### Git
- vim-gitgutter

### Development
- vim-autoclose  
    matching brackets e.g. {}
- tcomment_vim  
    *`* : comment out all the selected words
- vim-airline
- rainbow_parentheses.vim  
    讓多層的括號以不同的顏色顯示
- indentLine  
    用直線標註同indent的區塊
- vim-trailing-whitespace  
    標註每行最後面沒用到的空白
- tagbar  
    `<F10>`
- vim-indent-object  
    `v` `i` `{` : 選取大括號內的文字  
    `v` `i` `i` : 選取同indent內的文字  
    `v` `a` `i` : 選取同indent內的文字,同時包含上一級  

### Syntax
- syntastic  
    automatically check syntax error
- python-mode  
    整合各種python套件
- jedi-vim  
    python autocomplete
- c.vim
    加強C/C++的各種功能  
    在github上沒有最新版,目前是下載vim.org的最新版\(version 6.1\) 放在我的github上，必須手動更新  
    `<F9>` : compile  
- cpp-vim  
    strengthen c++ syntax highlight
- vim-cpp-enhanced-highlight
- html5.vim  
    html5 syntax highlight
- emmet-vim  
    zen coding
- vim-markdown  
    markdown syntax highlight

### Tool
- vim-easymotion  
    快速搜尋文字並移動
- vim-multiple-cursors  
    如同sublime支援多重游標
    在normal mode按ctrl + n ，再選取，最後再按一次ctrl + n
- vim-sdcv  
    use sdcv to search vocabulary
    `<F3>` : search
- vimspell  
    spell checking

### Theme
- desert

# Author
[Lee-W](https://github.com/Lee-W/)
