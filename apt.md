## Administration
### Show policy settings
```bash
$ apt policy
```
### Get info on package
```bash
$ apt show 'gedit'
```
### Remove package and configuration + other packages which were required by this package but not required by any remaining packages
```bash
# aptitude purge <package name>
```
### Find packages requiring current package (recursive dependencies)
```bash
$ apt rdepends gedit
```
### Install from backports
```bash
# apt install -t buster-backports gedit
```
### Include packages from usb iso
Add the following to `/etc/apt/sources.list`
```bash
deb [trusted=yes] file:/media/usb0/ buster main contrib non-free
```

## Searching
### List installed packages
```bash
$ apt list --installed
```
### Show all packages not from the Debian repositories (including manually installed .deb)
```bash
$ aptitude search '?narrow(?installed, !?origin(debian))'
```
### Search available packages by name
```bash
$ aptitude search 'linux-image'
```
### Search specific package (only installed!)
```bash
$ aptitude search 'gedi ~i'
```
