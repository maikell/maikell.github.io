---
title: "Sort and grep fu"
date: 2022-05-10
menu: "CLI"
weight: 1 

---
# Sort and grep fu

## Get from line $A to line $B in a large file
```
awk 'NR >= 2459499 && NR <= 2462053' FILE >FILE_CUT
```
>= is from line and <= to line. File is the source file and FILE_CUT is the selected lines.


