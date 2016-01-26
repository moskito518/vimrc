# vimrc

```
cd ~/workspace
git clone git@github.com:moskito518/vimrc.git
cd ~/.config
curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
cd nvim
ln -s ~/workspace/vimrc/cache_dir cache_dir
ln -s ~/workspace/vimrc/colors colors
ln -s ~/workspace/vimrc/init.vim init.vim
ln -s ~/workspace/vimrc/ycm_extra_conf.py ycm_extra_conf.py
mkdir .backup
mkdir .swp
nvim
:PlugInstall

```
