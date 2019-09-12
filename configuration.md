## dev env installation:

### ssh
`touch ~/.ssh/rc`
```
echo "if [ ! -S ~/.ssh/ssh_auth_sock ] && [ -S "$SSH_AUTH_SOCK" ]; then
        ln -sf $SSH_AUTH_SOCK ~/.ssh/ssh_auth_sock
     fi" >> ~/.ssh/rc
```

### git
`sudo apt install git`

### nginx
`sudo apt install nginx`

###fzf
`ln -s ~/.fzf/shell/key-bindings.fish ~/.config/fish/functions/fzf_key_bindings.fish`

### dotfiles
`git clone git@github.com:P1X3L/dotfiles.git ~/.dotfiles`

### symlinks
`ln -s ~/.dotfiles/aliases ~/.aliases`
`ln -s ~/.dotfiles/vim ~/.vim`
`ln -s ~/.dotfiles/vimrc ~/.vimrc`
`ln -s ~/.dotfiles/tmux.conf ~/.tmux.conf`
`ln -s ~/.dotfiles/config/fish/config.fish ~/.config/fish/config.fish`

### vim
`sudo apt install vim`
`vim +'PlugInstall --sync' +qa`

### vim plugins
`python3 ~/.vim/plugged/YouCompleteMe/install.py`

### tmux
`sudo apt install tmux`

### asdf
```
sudo apt install \
  automake autoconf libreadline-dev \
  libncurses-dev libssl-dev libyaml-dev \
  libxslt-dev libffi-dev libtool unixodbc-dev \
  unzip curl
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.7.1
```

### powerline
`pip3 install powerline-status psutil`

### fish
```
sudo apt-add-repository ppa:fish-shell/release-3
sudo apt-get update
sudo apt-get install fish
```

### fisher
`curl https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish`
`fisher add jethrokuan/z`

## languages installation

### ruby
`asdf plugin-add ruby`
`asdf install ruby 2.4.1`
`asdf global ruby 2.4.1`

### postgres
`asdf plugin-add postgres`
`asdf install postgres 11.1`
`asdf global postgres 11.1`

### nodejs
`asdf plugin-add nodejs`
`bash ~/.asdf/plugins/nodejs/bin/import-release-team-keyring`
`asdf install nodejs 10.15.0`
`asdf install nodejs 10.15.1`
`asdf global nodejs 10.15.1`

### erlang
`asdf plugin-add erlang`
`asdf install erlang 21.3.3`
`asdf global erlang 21.3.3`

### elixir
`asdf plugin-add elixir`
`asdf install elixir 1.7.3-otp-21`
`asdf global elixir 1.7.3-otp-21`

### rust
`asdf plugin-add rust`
`asdf install rust 1.34.0`
`asdf global rust 1.34.0`
`rustup default stable`

## projects installation

### create project folder
`mdkir -p ~/workspace/wttj`

### wk
`cd ~/workspace/wttj && git clone git@github.com:WTTJ/wk.git`
