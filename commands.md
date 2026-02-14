# Commands

| Command | Description | Parameter | Parameter Description |
| --- | --- | --- | --- |
| `chown <User> <Path>` | Change Owner | `-R` | rekursiv |
| `chmod <<owner/group/all>> <Path>` | Change rights | `1` | execute |
| | | `2` | write |
| | | `4` | read |
| | | `g+w` | add write only for group |
| | | `g-w` | remove write only for group |
| | | | u User // g Group // o Owner // a All // + grant // - remove |
| | | `-R` | recursiv |
| `find` | Search | `-name` | Suchen nach Name (z.B. "\*.txt") |
| `exa` | Folder view | `-T` | Tree view with subfolders |
| `apt install <dpkg package>` | Install dpkg Package installieren | | |
| `df` | Show free space | `-h` | With units (M, G) |
| `du <Path>` | Folder size | `-sh` | only folder size / with units (M,G) |
| `tar -xf <File>` | Extract TAR / bz2 file | `-xf` | extract |
| `gunzip file.gz` | Extract GZ | | |
| `unzip file.zip` | Extract ZIP | | |
| `netstat -tupan` | Show open Ports and Connections | | |
| `scp -r -P 49299 user@host:/path/to/folder/ local-copy-of-folder` | Copy folder from Remote to Host | | |
