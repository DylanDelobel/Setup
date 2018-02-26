# Install mysql5.6 on ArchLinux

Add custom repository : 

`sudo nano /etc/pacman.conf`

Add at the end

```
[muflone-mysql]
SigLevel = Required
Server = https://www.muflone.com/repositories/archlinux/$repo/$arch
```

Update package list

`sudo pacman -Sy`

Throught the packet manager look for `mysql56` and install

Launch the server with

`systemctl start mysqld.service`

To launch the server at startup, run

`sudo systemctl enable mysqld.service`

## zsh

Create a folder for custom plugins

`sudo mkdir .zshplugins`

Go into `cd .zshplugins`

Clone

`git clone https://github.com/voronkovich/mysql.plugin.zsh.git`

Edit zsh conf `sudo nano ~/.zshrc`

Add `plugins=(... mysql)`

`source .zshplugins/mysql.plugin.zsh/mysql.plugin.zsh`

