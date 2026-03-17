# LVM (Logical Volume Management)

## Create Physical Volume
pvcreate /dev/sdb

## Create Volume Group
vgcreate my_vg /dev/sdb

## Create Logical Volume
lvcreate -L 1G -n my_lv my_vg

## Format the Volume
mkfs.ext4 /dev/my_vg/my_lv

## Mount the Volume
mount /dev/my_vg/my_lv /mnt

## Check LVM
pvs
vgs
lvs

## Extend Volume
lvextend -L +1G /dev/my_vg/my_lv
resize2fs /dev/my_vg/my_lv
