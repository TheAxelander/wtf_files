# ZFS Snapshot

| Command | Description |
| --- | --- |
| `zfs snapshot datapool/fs1@12jan2014` | Create a snapshot named 12jan2014 of the fs1 filesystem |
| `zfs list -t snapshot` | List snapshots |
| `zfs rollback -r datapool/fs1@10jan2014` | Roll back to 10jan2014 (recursively destroy intermediate snapshots) |
| `zfs rollback -rf datapool/fs1@10jan2014` | Roll back must and force unmount and remount |
| `zfs destroy datapool/fs1@10jan2014` | Destroy snapshot created earlier |
| `zfs send datapool/fs1@oct2013 > /geekpool/fs1/oct2013.bak` | Take a backup of ZFS snapshot locally |
| `zfs receive anotherpool/fs1 < /geekpool/fs1/oct2013.bak` | Restore from the snapshot backup backup taken |
| `zfs send datapool/fs1@oct2013 \| zfs receive anotherpool/fs1` | Combine the send and receive operation |
| `zfs send datapool/fs1@oct2013 \| ssh node02 "zfs receive testpool/testfs"` | Send the snapshot to a remote system node02 |
