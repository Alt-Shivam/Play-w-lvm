# Snapshots in ubuntu

## Install timeshift
```
sudo apt-get install timeshift
```

## Create a Snapshot
```
sudo timeshift --create --comments "Description" --tags D --snapshot-device <Storage-volume-name>
```
In my case it's
```
sudo timeshift --create --comments "Initial with flexran and patch" --tags D --snapshot-device /dev/ubuntu-vg/lvbackup
```
# Known Issues
![image](https://github.com/Alt-Shivam/Play-w-lvm/assets/81817735/7fcd7750-02a3-4bc7-85a5-986ff2c5f496)

You have to expand the storage volume.
## List vgs
![image](https://github.com/Alt-Shivam/Play-w-lvm/assets/81817735/336e0444-6b33-4ff5-83e7-76187cb6c570)
## Create a new volume
![image](https://github.com/Alt-Shivam/Play-w-lvm/assets/81817735/d72c6d86-587a-4ae9-8404-52c8a429a830)
## Format it in ext4
![image](https://github.com/Alt-Shivam/Play-w-lvm/assets/81817735/442d9941-7588-43ba-a27d-cc689bbc4796)
## Create a snapshot
![image](https://github.com/Alt-Shivam/Play-w-lvm/assets/81817735/9176bf81-8d95-4231-851a-1e0e8eb19fe5)


