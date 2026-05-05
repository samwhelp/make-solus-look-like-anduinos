

# Issue


## Content

run

``` sh
sudo pipx install gnome-extensions-cli --global
```

show

```
  installed package gnome-extensions-cli 0.11.0, installed using Python 3.12.11
  These apps are now globally available
    - gext
    - gnome-extensions-cli
⚠️  Note: '/usr/local/bin' is not on your PATH environment variable. These apps will not be
    globally accessible until your PATH is updated. Run `pipx ensurepath` to automatically add
    it, or manually modify your PATH in your shell's config file (e.g. ~/.bashrc).
done! ✨ 🌟 ✨

```


## Explore

run

``` sh
file /etc/profile
```

show

```
/etc/profile: symbolic link to /usr/share/defaults/etc/profile
```




run

``` sh
cat /usr/share/defaults/etc/profile.d/10-path.sh
```

show

``` sh
# Begin /usr/share/defaults/etc/profile.d/10-path.sh

export PATH="/usr/sbin:/usr/bin"
if [ -d "/usr/local/sbin" ]; then
  export PATH="$PATH:/usr/local/sbin"
fi

if [ -d "/usr/local/bin" ]; then
  export PATH="$PATH:/usr/local/bin"
fi

if [ -d "$HOME/bin" ]; then
  export PATH="$HOME/bin:$PATH"
fi

if [ -d "$HOME/.local/bin" ]; then
  export PATH="$HOME/.local/bin:$PATH"
fi

# End /usr/share/defaults/etc/profile.d/10-path.sh
```



## Howto

create dir `/usr/local/bin`

``` sh
sudo mkdir -p /usr/local/bin
```

then logout

``` sh
gnome-session-quit
```

``` sh
gnome-session-quit --logout
```

then login

``` sh
echo $PATH
```
