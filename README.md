# gnome-network-stats
Gnome extension for showing network upload, download speed and per day data usage.

<div>
<p><a href="#"><img src="assets/logo.svg" height=80px alt="NSS Logo"/></a></p>
<h1>Network Stats</h1>
<p><img src='assets/screenshot.png' width="400px"  alt="Screenshot"/>
</div>

## Installation

### install from https://extensions.gnome.org

The latest reviewed version can be found at
<div>
<a href="https://extensions.gnome.org/extension/4308/network-stats/" >
<img src="assets/get-it-on-ge.svg" height="100" alt="Get it on GNOME Extensions">
</a>
</div>

### donwload from github.com and install yourself

The latest development version can be installed manually with these commands:

```
git clone https://github.com/noroadsleft000/gnome-network-stats.git

cd gnome-network-stats

./commands.sh build

./commands.sh install
```

Then go to https://extensions.gnome.org/local/ to turn on the extension or use
gnome-tweak-tool to enable it.


## Commands
### build extension
```
./commands.sh build
```
### install extension
```
./commands.sh install
```
### uninstall extension
```
./commands.sh uninstall
```
### enable extension
```
./commands.sh enable
```
### disable extension
```
./commands.sh disable
```
### pack the extension to zip file
```
./commands.sh pack
```
### launch a nested wayland session for debugging the extension
```
./commands.sh launch_debug
```

## ERROR while updating extension from store.
Universal solution of all problems `"Restart your machine"` will work.

If you are on X11 and not of wayland, reload shell `"Alt + F2", "r + Enter"` would be sufficient.

still facing some error? report it by creating a bug.

## Reporting a Bug

When reporting a bug, please include debugging output from `gnome-shell`.

You can capture the logs with this command:
```
journalctl /usr/bin/gnome-shell | grep network-stats

journalctl -f -o cat /usr/bin/gnome-shell
```

## Developer resources
- [Basic Gnome extension guide](https://gjs.guide/extensions/development/creating.html#gnome-extensions-tool)
- [Gnome JS API documentation](https://gjs-docs.gnome.org/)
- [JS API documentaion - Unofficial](https://www.roojs.com/seed/gir-1.2-gtk-3.0/seed)
- [Gnome JS API source code](https://github.com/GNOME/gnome-shell/tree/main/js)

## Contibutors
Contributions are always welcome, fork this repository make your changes.
and then generate a pull request.


## License

GNOME Shell Extensions are distributed under the terms of the GNU General
Public License. This extension is shipped under MIT License.
