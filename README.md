# vimGirl
All of the code I created for my Youtube Channel. Shout out to #GarageScript for helping me on my journey towards becoming a great software engineer!

<h1> To set up Vim & Tmux: </h1>
<h2>Vim - .vimrc</h2>

1. Clone the settings file and move it to an appropriate file. I put mine in ~/Documents.
`cd ~/Documents/ && git clone https://github.com/llipio/DevSettings`
2. Symlink your home settings to your new location.
For vim: `ln -s ~/Documents/DevSettings/.vimrc ~/.vimrc`
3. Install YARN: `brew install yarn`
4. Install Vundle: `git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
5. Install Tmux: `brew install tmux`
Setup tmux colors: `echo 'set -g default-terminal "screen-256color"' > ~/.tmux.conf`
6. Lastly, to install all the plugins specified in `.vimrc` file, open Vim: `vim` and then press `Ctrl` + `I`. Installation progress and result will show up on the left pane of Vim.

<h2>Bashprofile</h2>

7. Add to your bash profile: `vim ~/.bash_profile` or `vim ~/.bashrc`
`if [ -f ~/.devBash ]; then
  source ~/.devBash
fi`
8. Symlink devBash to this location: `ln -s ~/Documents/DevSettings/.devBash ~/.devBash`
9. Refresh: `source ~/.bash_profile`
