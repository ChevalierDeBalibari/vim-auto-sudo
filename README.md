# vim-auto-sudo

Small wrapper script around vim editor. It will automatically ask for sudo password
when editing some root owned configuration files.

Simply said, it saves both time and nerves.

## Installation 

Set up `VIM_PATH` variable in your `.bashrc` or `.zshrc` file:

```shell
echo export VIM_PATH=$(which vim) >> ~/.zshrc
```

Use `curl` or `wget` command to download and install vim script:

```shell
curl -o ~/.local/bin/vim https://raw.githubusercontent.com/ChevalierDeBalibari/vim-auto-sudo/master/vim
```

or

```shell
wget -O ~/.local/bin/vim https://raw.githubusercontent.com/ChevalierDeBalibari/vim-auto-sudo/master/vim
```

Next, make it executable:

```shell
chmod +x ~/.local/bin/vim
```

## Installation for non-vim users


If by chance you don't know how to exit vim and really want to use nano or some other obscure editor, change 
name of the script to match your favorite crappy editor:

```shell
which nano 
mv ~/.local/bin/vim ~/.local/bin/nano
```

Change `VIM_PATH` variable to point to path obtained by nano command like:

```shell
export VIM_PATH=/usr/bin/nano
```

That is all!


