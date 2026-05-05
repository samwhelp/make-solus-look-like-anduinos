

# Requirement

* [Requirement for Install Gnome Extensions](#requirement-for-install-gnome-extensions)
* [Requirement for ArcMenu](#requirement-for-arcmenu)
* [Requirement for Install fluent-gtk-theme](#requirement-for-install-fluent-gtk-theme)




## Requirement for Install Gnome Extensions

| Requirement | Note |
| ----------- | ---- |
| [pipx](https://github.com/pypa/pipx) | for install gnome-extensions-cli |
| [gnome-extensions-cli](https://github.com/essembeh/gnome-extensions-cli) | for install extension |

> run to install [pipx](https://github.com/getsolus/packages/tree/main/packages/p/pipx) at solus

``` sh
sudo eopkg install pipx
```

> run to install gnome-extensions-cli (gext)

``` sh
sudo pipx install gnome-extensions-cli --global
```




## Requirement for ArcMenu

| Requirement | Note |
| ----------- | ---- |
| [libgnome-menus](https://github.com/getsolus/packages/tree/main/packages/l/libgnome-menus) | for [ArcMenu](https://extensions.gnome.org/extension/3628/arcmenu/) |

> run to install [libgnome-menus](https://github.com/getsolus/packages/tree/main/packages/l/libgnome-menus) at solus

``` sh
sudo eopkg install libgnome-menus
```

> ArcMenu Requires GMenu Package:

| Distro           | Package                                   |
| ---------------- | ----------------------------------------- |
| Debian / Ubuntu  | libgnome-menu-3-0, gir1.2-gmenu-3.0       |
| Fedora           | gnome-menus                               |
| Arch / Manjaro   | gnome-menus                               |
| OpenSUSE         | libgnome-menu-3-0, typelib-1_0-GMenu-3_0  |




## Requirement for Install fluent-gtk-theme

> run to install [sassc](https://github.com/getsolus/packages/tree/main/packages/s/sassc) at solus

``` sh
sudo eopkg install sassc
```
