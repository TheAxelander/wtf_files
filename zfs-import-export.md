# ZFS Import / Export

| Command | Description |
| --- | --- |
| `zpool import` | List pools available for import |
| `zpool import -a` | Imports all pools found in the search directories |
| `zpool import -d` | To search for pools with block devices not located in /dev/dsk |
| `zpool import -d /zfs datapool` | Search for a pool with block devices created in /zfs |
| `zpool import oldpool newpool` | Import a pool originally named oldpool under new name newpool |
| `zpool import 3987837483` | Import pool using pool ID |
| `zpool export datapool` | Deport a ZFS pool named mypool |
| `zpool export -f datapool` | Force the unmount and deport of a ZFS pool |
