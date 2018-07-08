# ks
CentOS kickstart files

The virtualbox VMs where this kickstart scripts are tested have toy sized hard disks (4GB), bios booting mostly.

- c7-GA: installing from the General Availability (7.x.YYMM) release, without updates during the installation
- c7: CentOS-7 with all the available updates applied during the installation
- default partition is a RAID1 /dev/md0 (/dev/sd[ab]1) for /
- +boot: mdadm RAID1 /dev/md0 (sd[ab]1) for /boot and mdadm RAID1 /dev/md1 (sd[ab]2) 

# files
- /dev/md0 for /: c7-GA-raid1.cfg c7-raid1.cfg
- /dev/md0 as /boot and /dev/md1 as /: c7-GA-raid1+boot.cfg c7-raid1+boot.cfg

