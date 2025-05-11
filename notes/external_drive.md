## Setting up new drive
 - Use `sudo fdisk -l` to identify the disk path. Should be something like `/dev/sdb1` or `/dev/sdb2`

### First time setup
 - Create two paritions: one for ntfs (100G) and other one to be used for media server (ext4)
 - `sudo fdisk /dev/sdb<1>` and then follow the menu to create new parittions as required. Skip to mounting if repartition is not required.
 - Need to run `sudo mkfs -t ext4 /dev/sdb<1/2>` before disk can be mounted
 
### Mounting 
 - Mount manually `sudo mount -t auto /dev/sdb1 [mountpoint]`
 - Update owner for mounted drive - will be root by default
 - Follow the guide here: https://phoenixnap.com/kb/linux-format-disk

#### Other commands

Unmount: `sudo umount /dev/sdb2`
Check mount: `lsblk`

### Upgrading storage for server

