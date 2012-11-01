Installation Notes
------------------

    git clone git@github.com:tobinvanpelt/dotfiles.git ~/.dot

Create symlinks:

    ln -s ~/.dot/profile ~/.profile
    ln -s ~/.dot/zshrc ~/.zshrc
    ln -s ~/.dot/oh-my-zsh ~/.oh-my-zsh
    
    ln -s ~/.dot/vim ~/.vim
    ln -s ~/.dot/vimrc ~/.vimrc
    ln -s ~/.dot/gvimrc ~/.gvimrc

    ln -s ~/.dot/tmux.conf ~/.tmux.conf

Switch to the `~/.dot` directory, and fetch submodules:

    cd ~/.dot
    git submodule init
    git submodule update

Updating a specific submodule (example):

    cd ~/.dot/vim/bundle/fugitive
    git pull origin master

Updating all submodules:

    git submodule foreach git pull origin master