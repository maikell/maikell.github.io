---
title: "Generic shell command fu"
date: 2022-05-13
menu: "CLI"
weight: 1 
---

####  Make a file inmutable 
```
sudo chattr +i $file
```

### Undo inmutable state
```
sudo chattr -i $file
```

### umount lazy and all cif mountpoints
```
sudo umount -l -a -t cifs
```
