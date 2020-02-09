### GET DISK SIZE 
```
sudo fdisk -l | egrep 'Disk.*bytes' | awk '{ sub(/,/,""); sum +=$3; print $2" "$3" "$4 } END { print "—————–"; print "total: " sum " GB"}'
```
