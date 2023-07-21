# Play-w-lvm
Help you to play with lvm in linux

# To resize the space in / ,if you are short in space
## First, check the partitions on your disk:
```
sudo fdisk -l
```
## Display information about your current volumes and volume groups:
```
sudo lvdisplay
sudo vgdisplay
```
## Resize the logical volume:
```
sudo lvextend -L +<Free Space> <LV Path>
```
in my case it's
```
sudo lvextend -L +50G /dev/ubuntu-vg/ubuntu-lv
```
## Resize the filesystem:
```
sudo resize2fs /dev/ubuntu-vg/ubuntu-lv
```

## have a look on size resize:
```
df -h /
```
