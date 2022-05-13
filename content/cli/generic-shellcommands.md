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

### Find files and change all permissions
```
find . -type f -exec chmod 664 {} \;
```

### Find directories and change all permissions
```
find . -type d -exec chmod 755 {} \;
```

### Find and remove files older than
In this example older than 5 day's
```
find . -mtime +5 -exec echo {} ; 
```
