## List installed packages
```bash
$ apt list --installed
```

## Show policy settings
```bash
$ apt policy
```
## Show all packages not from the Debian repositories (including manually installed .deb)
```bash
$ aptitude search '?narrow(?installed, !?origin(debian))'
```
## Search available packages by name
```bash
aptitude search 'linux-image'
```
## Search specific package (only installed!)
```bash
aptitude search 'gedi ~i'
```
